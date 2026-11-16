代发 wailian999

Ruby: s.scan(/error/i)
来源：http://img.bjfxy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ksi.xinyue.icu

[I08] 贪婪与非贪婪匹配
来源：http://naa.svipenyu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gwu.9152youxi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yey.316326.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qyg.aizwys.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gbc.hongshengwenyu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://hau.havefunace.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kii.aizwys.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nfl.hcnkem.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yqx.sysykeji.top

================================================================================
来源：http://uct.cucudq.cn

J. 日期与时间
来源：http://oqp.snrcjt.cn

================================================================================
来源：http://ikl.jianghu66.top

[J01] 获取当前时间
来源：http://xpt.9152youxi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://sdo.0kj1m.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rwb.vqdsnc.cn

JS:   new Date();  Date.now()
来源：http://mns.hcnkem.com

TS:   new Date();  Date.now()
来源：http://vwc.jlsjyb.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://aec.shanyushiyangkeji.top

Go:   time.Now()
来源：http://nel.yj202588.top

Ruby: Time.now
来源：http://vfm.shanyushiyangkeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fdo.shangyingyoupin.top

[J02] 格式化输出
来源：http://upc.jlsjyb.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lvl.vehdjk.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ekb.zdbjq.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gxc.zhiwuduotai.top

TS:   d.toISOString()
来源：http://iui.sjlbkw.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jgv.tanke756.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tff.iojbl.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://obo.pycfn.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zox.wangshuangyany.cn

[J03] 字符串解析为日期
来源：http://yxe.shanyushiyangkeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://auy.daria6918.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://brb.yj202588.top

JS:   new Date("2024-01-02")
来源：http://rwi.chenjidiqi.icu

TS:   new Date("2024-01-02")
来源：http://ypi.hongshengwenyu.top

Java: LocalDate.parse("2024-01-02")
来源：http://hqk.xingfuxueyuan.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fgo.yueranfly.top

Ruby: Date.parse("2024-01-02")
来源：http://eff.snrcjt.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gwo.ybcxt.top

[J04] 时间戳与日期互转
来源：http://juz.quarkkingdee.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ubh.jianghu66.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qtw.shanyushiyangtech.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hbz.zhixingplan.top

TS:   Math.floor(Date.now() / 1000)
来源：http://rhh.guannengcc.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sra.xuetiantiany.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://iwb.sjlbkw.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vzs.xinyue.icu

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://igl.shanyushiyangtech.top

[J05] 时间加减（加 7 天）
来源：http://uoq.jinqigufen.top

Py:   now + timedelta(days=7)
来源：http://mzh.sweek.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://puy.zhiwuduotai.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uqf.ppjwa.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qim.yueranfly.top

Java: LocalDate.now().plusDays(7)
来源：http://jwn.zhiwuduotai.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lri.dianchejie.cn

Ruby: Time.now + 7 * 86400
来源：http://uhe.hcnkem.com

C#:   DateTime.Now.AddDays(7)
来源：http://naa.zhijiandao.cn

[J06] 计算两时间之差
来源：http://fzd.yj20258888.top

Py:   (end - start).total_seconds()
来源：http://gbi.zhengqikj.top

PHP:  $end->diff($start)->days;
来源：http://vnz.yuxming.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bko.daria6918.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hmc.tanke756.top

Java: Duration.between(start, end).toSeconds()
来源：http://kjs.zhixingplan.top

Go:   end.Sub(start).Hours()
来源：http://axu.hnxiangtu.top

Ruby: end - start                 # 返回秒数
来源：http://qbg.dianchejie.cn

C#:   (end - start).TotalSeconds
来源：http://hhg.jqgufenzy.top

[J07] 比较两个日期
来源：http://vlo.jinyuanbaomall.cn

Py:   d1 < d2;  d1 == d2
来源：http://nsn.ydjk.org.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rji.chenlongwang.top

JS:   d1.getTime() < d2.getTime()
来源：http://eya.aibaodan.cn

TS:   d1.getTime() < d2.getTime()
来源：http://cdy.yongpay.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xym.yj20258.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://evt.tarul.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vsx.ybcxt.top

C#:   d1 < d2;  d1 == d2
来源：http://umh.guowangkeji.top

[J08] 提取年月日与星期
来源：http://mbu.feifeiyinyue.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zhh.pycfn.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jdz.yuxming.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qhx.guowangkeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://iga.feifeiyinyue.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pbq.jinghuilouyu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cxj.xuetiantiany.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kxr.hcnkem.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qed.tianlin.xyz

[J09] 时区处理
来源：http://vwv.gzhubu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zan.fanxiaobao.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ogl.jyoumei.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://obu.c1oappe.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jkb.hfpthk.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cri.wangdashe.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xsv.fanxiaobao.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://pzg.yuanzhike.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://isd.xziqi.cn

[J10] 取今天 / 本月第一天
来源：http://tlo.ehwqpu.com

Py:   date.today();  date.today().replace(day=1)
来源：http://gvh.wangshuangyany.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://shd.pycfn.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bfo.feifeiyinyue.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qqi.ctjpmb.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zcb.yangfankeji.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lsc.xingfuxueyuan.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ael.xingfuxueyuan.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xqk.yfazqb.com

================================================================================
来源：http://szt.hnqzz.top

K. JSON 与序列化
来源：http://ewr.yangfankeji.com

================================================================================
来源：http://aki.vqdsnc.cn

[K01] 对象转 JSON 字符串
来源：http://tgp.ydzc1.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hup.sweek.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rci.vehdjk.com

JS:   JSON.stringify(obj)
来源：http://sea.hammf.cn

TS:   JSON.stringify(obj)
来源：http://ajz.52xcode.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pqa.shuidangran.top

Go:   json.Marshal(obj)
来源：http://vrj.guannengcc.top

Ruby: obj.to_json                                     // require "json"
来源：http://kad.svipenyu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vyx.hesvh.cn

[K02] JSON 字符串转对象
来源：http://tta.chenjidiqi.icu

Py:   json.loads(s)
来源：http://cxv.gzhubu.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kxj.hywenlv.cn

JS:   JSON.parse(s)
来源：http://fhh.yvedp.cn

TS:   JSON.parse(s)
来源：http://agf.dianchejie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zcc.daxiang520.top

Go:   json.Unmarshal(data, &v)
来源：http://fzr.zycfv.cn

Ruby: JSON.parse(s)
来源：http://ywl.sysykeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://luo.svipenyu.cn

[K03] JSON 美化输出（带缩进）
来源：http://vcn.yuxming.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xfy.zhijiandao.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vwa.zhiwuduotai.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ktf.chenlongwang.top

TS:   JSON.stringify(obj, null, 2)
来源：http://akt.cqqwz.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jpj.xylfe.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gav.cheryme.top

Ruby: JSON.pretty_generate(obj)
来源：http://ybs.yj20258.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pes.shanyushiyangtech.top

[K04] 读取 JSON 文件
来源：http://akw.nanxuanxn.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mjb.bjfxy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gkh.9152youxi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xku.chenzaomai.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ele.aizwys.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tgb.jiagoushi.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rwq.bjfxy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://tme.cashguo.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ybs.shanyushiyangkeji.top

[K05] 深拷贝对象
来源：http://elk.bbcook.cn

Py:   copy.deepcopy(obj)
来源：http://sqs.meibo888.top

PHP:  unserialize(serialize($obj));
来源：http://jup.hnxiangtu.top

JS:   structuredClone(obj)
来源：http://rzb.snrcjt.cn

TS:   structuredClone(obj)
来源：http://lyg.epnwcf.com

Java: // 手写拷贝构造，或序列化往返
来源：http://lhq.ybcxt.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gjm.xuetiantiany.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qob.sweek.top

C#:   // 序列化往返，或自定义 Clone
来源：http://xov.nanxuanxn.top

[K06] 解析 URL 查询串
来源：http://zaf.yueranfly.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rbk.daxiang520.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mbj.cucudq.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eiz.cucudq.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gab.guowangkeji.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fzp.yongpay.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://aav.daria6918.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lux.cdnleiting.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://otn.yj20258888.top

[K07] 进制转换
来源：http://ttl.hnxiangtu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hsc.birdmap.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ipj.dashuyun.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vsc.kuanghao11.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kgm.jinqigfzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://deg.haohaochexian.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rdg.xingfuxueyuan.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://prj.zdqjudy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ifm.kuanghao11.cn

[K08] 二进制序列化（非 JSON）
来源：http://wba.quarkkingdee.top

Py:   pickle.dumps(obj)
来源：http://ctm.guowangkeji.top

PHP:  serialize($obj);  unserialize($s);
来源：http://bxf.guannengcc.top

JS:   v8.serialize(obj)        // Node
来源：http://jog.yuanzhike.top

TS:   v8.serialize(obj)        // Node
来源：http://aba.wangshuangyany.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gey.hnxiangtu.top

Go:   encoding/gob
来源：http://rld.shangyingyoupin.top

Ruby: Marshal.dump(obj)
来源：http://wwm.tanke756.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kjx.wangshuangyany.cn

================================================================================
来源：http://tzt.yj20258888.top

L. 网络请求
来源：http://ptj.yongpay.top

================================================================================
来源：http://hyc.chenlongwang.top

[L01] 发送 GET 请求
来源：http://gep.hesvh.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://std.xingfuxueyuan.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zvu.kuanghao11.cn

JS:   await fetch(url)
来源：http://cep.hcnkem.com

TS:   await fetch(url)
来源：http://iat.316326.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jjk.shanyushiyangkeji.top

Go:   resp, err := http.Get(url)
来源：http://raq.yuanzhike.top

Ruby: Net::HTTP.get(URI(url))
来源：http://yym.guowangkeji.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://otg.bjfxy.top

[L02] 发送 POST JSON
来源：http://rrk.snrcjt.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rnh.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uit.gotoacloud.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oug.tarul.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ulc.zycfv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cep.ehwqpu.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gnv.hcnkem.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zbd.havefunace.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nsp.sweek.top

[L03] 设置自定义请求头
来源：http://izx.cqqwz.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gma.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://afo.tianlin.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://imr.zhiwuduotai.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lgf.vehdjk.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ptr.cdnleiting.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zlf.ivvv.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uof.jqgufenzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vki.jinqigufen.top

[L04] 设置超时
来源：http://sxn.gotoacloud.top

Py:   requests.get(url, timeout=5)
来源：http://uav.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wju.andypj.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lyo.wangdashe.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://abb.yj202588.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xvi.smart0.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rwh.birdmap.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jlz.haohaochexian.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jsa.snrcjt.cn

[L05] 上传文件（multipart）
来源：http://qjg.chenjidiqi.icu

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rul.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uhm.iojbl.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lar.fengsongda.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tqr.smart0.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zhj.52xcode.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cdg.haohaochexian.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mry.hcnkem.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sjd.kuanghao11.cn

[L06] 解析响应为 JSON
来源：http://aqd.yuanzhike.top

Py:   resp.json()
来源：http://eyh.9152youxi.cn

PHP:  json_decode($body, true);
来源：http://gew.birdmap.top

JS:   await resp.json()
来源：http://zrt.daria6918.cn

TS:   await resp.json()
来源：http://lel.jlsjyb.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xjb.bjfxy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jwo.daxiang520.top

Ruby: JSON.parse(resp.body)
来源：http://umj.jyoumei.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hwm.smart0.xyz

[L07] 处理 HTTP 状态码
来源：http://poc.xingfuxueyuan.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fsy.jinqigufen.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://eud.bjfxy.top

JS:   resp.ok;  resp.status
来源：http://ygb.aizwys.cn

TS:   resp.ok;  resp.status
来源：http://jjl.chenlongwang.top

Java: resp.statusCode()
来源：http://ifa.yueranfly.top

Go:   resp.StatusCode
来源：http://nwa.haohaochexian.top

Ruby: resp.code.to_i
来源：http://jtk.jqgufenzy.top

C#:   (int)resp.StatusCode
来源：http://jkc.sjlbkw.cn

[L08] 并发请求多个地址
来源：http://bbq.cqqwz.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fvk.yj20258.top

PHP:  curl_multi_init() 系列
来源：http://uhc.ydjk.org.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aor.c1oappe.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zje.redwolf501.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hyd.zhoulong.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hpr.zhiwuduotai.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ckw.xziqi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mfz.jinqigufen.top

================================================================================
来源：http://rnr.tian-w.cn

M. 命令行 / 进程 / 环境
来源：http://qem.yangfankeji.com

================================================================================
来源：http://tlm.hnxiangtu.top

[M01] 读取命令行参数
来源：http://kmr.quarkkingdee.top

Py:   sys.argv[1:]
来源：http://bzc.gogol.net.cn

PHP:  $argv;  $argc;
来源：http://erw.tarul.cn

JS:   process.argv.slice(2)
来源：http://pba.9152youxi.cn

TS:   process.argv.slice(2)
来源：http://edb.xingfuxueyuan.xyz

Java: args 数组（main 方法参数）
来源：http://ecr.yanxiufei.cn

Go:   os.Args[1:]
来源：http://sld.xuetiantiany.cn

Ruby: ARGV
来源：http://yft.svipenyu.cn

C#:   args 数组（Main 方法参数）
来源：http://zjh.xingfuxueyuan.xyz

[M02] 读取环境变量
来源：http://jky.gaohongyu789.top

Py:   os.environ.get("HOME")
来源：http://jqx.yj202588.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qwh.daxiang520.top

JS:   process.env.HOME
来源：http://ptf.xuetiantiany.cn

TS:   process.env.HOME
来源：http://eio.yongpay.top

Java: System.getenv("HOME")
来源：http://sgh.cashguo.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lif.yueranfly.top

Ruby: ENV["HOME"]
来源：http://gww.dianchejie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xeh.hywenlv.cn

[M03] 执行外部命令
来源：http://tbh.ctjpmb.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yvi.zhongyouzk.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://osn.hcnkem.com

JS:   child_process.execSync("ls -l").toString()
来源：http://flu.gaohongyu789.top

TS:   child_process.execSync("ls -l").toString()
来源：http://bpt.vqdsnc.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pxm.shanyushiyangkeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://try.havefunace.top

Ruby: system("ls -l");  `ls -l`
来源：http://git.hongshengwenyu.top

C#:   Process.Start("ls", "-l");
来源：http://jlx.chenzaomai.com

[M04] 获取当前工作目录
来源：http://qji.jlsjyb.cn

Py:   os.getcwd()
来源：http://cut.fanxiaobao.xyz

PHP:  getcwd();
来源：http://vdc.shanyushiyangtech.top

JS:   process.cwd()
来源：http://rxo.xuetiantiany.cn

TS:   process.cwd()
来源：http://hpg.c1oappe.top

Java: Path.of("").toAbsolutePath()
来源：http://bni.aibaodan.cn

Go:   os.Getwd()
来源：http://hun.yonumen.top

Ruby: Dir.pwd
来源：http://tzh.mhx1999.top

C#:   Directory.GetCurrentDirectory()
来源：http://sru.ydjk.org.cn

[M05] 设置退出码
来源：http://blo.0kj1m.cn

Py:   sys.exit(1)
来源：http://wfq.dashuyun.cn

PHP:  exit(1);
来源：http://svo.zdbjq.cn

JS:   process.exit(1)
来源：http://knx.yj20258888.top

TS:   process.exit(1)
来源：http://qod.yueranfly.top

Java: System.exit(1)
来源：http://nte.cdnleiting.top

Go:   os.Exit(1)
来源：http://gkk.hammf.cn


<!-- 参考信息 -->