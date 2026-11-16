代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yfs.snrcjt.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gzm.bjfxy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jzl.sysykeji.top

================================================================================
来源：http://cia.fehbvm.com

J. 日期与时间
来源：http://bty.ydjk.org.cn

================================================================================
来源：http://esn.quarkkingdee.top

[J01] 获取当前时间
来源：http://vsg.fzhhl.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://qie.zhoulong.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cmh.zhongyouzk.top

JS:   new Date();  Date.now()
来源：http://obe.gaohongyu789.top

TS:   new Date();  Date.now()
来源：http://rqo.tarul.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://sdi.xylfe.cn

Go:   time.Now()
来源：http://brn.sjlbkw.cn

Ruby: Time.now
来源：http://oyg.hnqzz.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tnw.cashguo.top

[J02] 格式化输出
来源：http://jep.shanyushiyangkeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gls.zhoulong.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://icn.haohaochexian.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://avp.fanxiaobao.xyz

TS:   d.toISOString()
来源：http://gct.zhijiandao.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://avf.9152youxi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zvm.fktsv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tnd.zhoulong.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zce.bbcook.cn

[J03] 字符串解析为日期
来源：http://kpl.jlsjyb.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uem.sweek.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rcb.shuidangran.top

JS:   new Date("2024-01-02")
来源：http://bhr.hammf.cn

TS:   new Date("2024-01-02")
来源：http://hyv.feifeiyinyue.top

Java: LocalDate.parse("2024-01-02")
来源：http://osx.ctjpmb.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bfe.yj20258.top

Ruby: Date.parse("2024-01-02")
来源：http://dgx.pengpengdd.cyou

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nef.bbcook.cn

[J04] 时间戳与日期互转
来源：http://dlf.jyoumei.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wle.jinqigufen.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://oav.dashuyun.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://htz.ywan-chungtsiang.top

TS:   Math.floor(Date.now() / 1000)
来源：http://rsl.yongpay.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sth.smart0.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xkw.zhengqikj.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wwz.uphjek.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zum.aibaodan.cn

[J05] 时间加减（加 7 天）
来源：http://awd.chenjidiqi.icu

Py:   now + timedelta(days=7)
来源：http://tjx.jinqigfzy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://sxw.gogol.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xwc.hongshengwenyu.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://epu.cheryme.top

Java: LocalDate.now().plusDays(7)
来源：http://ccv.hfpthk.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://aot.ywan-chungtsiang.top

Ruby: Time.now + 7 * 86400
来源：http://qtb.jiagoushi.top

C#:   DateTime.Now.AddDays(7)
来源：http://iug.fktsv.cn

[J06] 计算两时间之差
来源：http://mqk.hfpthk.cn

Py:   (end - start).total_seconds()
来源：http://zwv.vehdjk.com

PHP:  $end->diff($start)->days;
来源：http://mvy.aizwys.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qmw.gogol.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pzo.jqgfzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://itg.jqgufenzy.top

Go:   end.Sub(start).Hours()
来源：http://hdg.hammf.cn

Ruby: end - start                 # 返回秒数
来源：http://imi.cucudq.cn

C#:   (end - start).TotalSeconds
来源：http://ygm.xinyue.icu

[J07] 比较两个日期
来源：http://aem.jianghu66.top

Py:   d1 < d2;  d1 == d2
来源：http://mlt.wangdashe.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://opt.zhoulong.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://qrc.cheryme.top

TS:   d1.getTime() < d2.getTime()
来源：http://jjz.316326.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jtc.bjfxy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yoi.wangshuangyany.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nxy.shanyushiyangtech.top

C#:   d1 < d2;  d1 == d2
来源：http://fzk.feifeiyinyue.top

[J08] 提取年月日与星期
来源：http://fsq.sufxvd.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mnb.bjfxy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lmd.yangfankeji.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uje.cdnleiting.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ewr.shanyushiyangkeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kzb.jinqigfzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gmz.cucudq.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zeq.smart0.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hhl.sxryk.cn

[J09] 时区处理
来源：http://szh.snrcjt.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://abn.jlsjyb.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://asq.sjlbkw.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jiy.xinyue.icu

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iiw.ydjk.org.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vwe.zhoulong.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yqr.daxiang520.top

Ruby: Time.now.getlocal("+08:00")
来源：http://erv.ctjpmb.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zsu.hfpthk.cn

[J10] 取今天 / 本月第一天
来源：http://klz.daria6918.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ykm.gogol.net.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fcr.sjlbkw.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pzz.zdbjq.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jke.sufxvd.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qpj.hnqzz.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zyj.guowangkeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yhl.epnwcf.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zgu.xuetiantiany.cn

================================================================================
来源：http://hgc.hysaishi.cn

K. JSON 与序列化
来源：http://crp.zhixingplan.top

================================================================================
来源：http://prs.sjlbkw.cn

[K01] 对象转 JSON 字符串
来源：http://sln.hysaishi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kwd.daria6918.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://edt.shanyushiyangtech.top

JS:   JSON.stringify(obj)
来源：http://jlj.ppjwa.cn

TS:   JSON.stringify(obj)
来源：http://ana.yueranfly.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cky.bjfxy.top

Go:   json.Marshal(obj)
来源：http://xyc.sjlbkw.cn

Ruby: obj.to_json                                     // require "json"
来源：http://sxr.gzhubu.top

C#:   JsonSerializer.Serialize(obj)
来源：http://jtd.yueranfly.top

[K02] JSON 字符串转对象
来源：http://mwm.zhongyouzk.top

Py:   json.loads(s)
来源：http://icp.hfpthk.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dve.yj20258888.top

JS:   JSON.parse(s)
来源：http://fcl.meibo888.top

TS:   JSON.parse(s)
来源：http://ymq.zdqjudy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://imf.yonumen.top

Go:   json.Unmarshal(data, &v)
来源：http://jfu.tian-w.cn

Ruby: JSON.parse(s)
来源：http://gln.zhengqikj.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rvr.birdmap.top

[K03] JSON 美化输出（带缩进）
来源：http://xai.jinqigfzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vhk.aizwys.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://upd.ywan-chungtsiang.top

JS:   JSON.stringify(obj, null, 2)
来源：http://zgj.hcnkem.com

TS:   JSON.stringify(obj, null, 2)
来源：http://wzw.jqgfzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://twv.bjfxy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gti.jlsjyb.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rls.snrcjt.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uaf.svipenyu.cn

[K04] 读取 JSON 文件
来源：http://vkj.gaohongyu789.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vxt.dashuyun.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gjd.yongpay.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ebp.xylfe.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wsg.jinyuanbaomall.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://khc.sysykeji.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vnm.gzhubu.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://htx.fktsv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zre.hammf.cn

[K05] 深拷贝对象
来源：http://mgm.guannengcc.top

Py:   copy.deepcopy(obj)
来源：http://nqs.jinqigfzy.top

PHP:  unserialize(serialize($obj));
来源：http://yml.9152youxi.cn

JS:   structuredClone(obj)
来源：http://evd.0kj1m.cn

TS:   structuredClone(obj)
来源：http://cuq.xingfuxueyuan.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://egw.xuetiantiany.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nqw.aibaodan.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qnn.wangshuangyany.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://aoq.cheryme.top

[K06] 解析 URL 查询串
来源：http://zpv.ywan-chungtsiang.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://frk.wangshuangyany.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://iyo.hcnkem.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rqy.hnqzz.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eba.ppjwa.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nbq.pycfn.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://jpd.gogol.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hiy.cashguo.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ijn.fzhhl.top

[K07] 进制转换
来源：http://hbe.bbcook.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fvd.pycfn.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zli.cdnleiting.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jnx.cucudq.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vme.jinghuilouyu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qhz.ivvv.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lkr.nanxinkj.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qjt.hnqzz.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jzu.feifeiyinyue.top

[K08] 二进制序列化（非 JSON）
来源：http://tle.zhengqikj.top

Py:   pickle.dumps(obj)
来源：http://bko.birdmap.top

PHP:  serialize($obj);  unserialize($s);
来源：http://xsc.jyoumei.cn

JS:   v8.serialize(obj)        // Node
来源：http://nyj.jinghuilouyu.cn

TS:   v8.serialize(obj)        // Node
来源：http://wfv.zhaomingkeji.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rzl.ybcxt.top

Go:   encoding/gob
来源：http://mme.nwbrower.top

Ruby: Marshal.dump(obj)
来源：http://jpq.vqdsnc.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rtm.gogol.net.cn

================================================================================
来源：http://vcl.hammf.cn

L. 网络请求
来源：http://qkq.zhongyouzk.top

================================================================================
来源：http://zxt.fengsongda.top

[L01] 发送 GET 请求
来源：http://iwe.hfpthk.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uzn.shzxlz.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mmy.daxiang520.top

JS:   await fetch(url)
来源：http://vbf.fehbvm.com

TS:   await fetch(url)
来源：http://xdz.yueranfly.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xby.yuanzhike.top

Go:   resp, err := http.Get(url)
来源：http://sav.haohaochexian.top

Ruby: Net::HTTP.get(URI(url))
来源：http://hbg.cqqwz.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rsn.yonumen.top

[L02] 发送 POST JSON
来源：http://mdl.guowangkeji.top

Py:   requests.post(url, json={"a": 1})
来源：http://qrb.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://plu.xuetiantiany.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://opn.aibaodan.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ajd.nanxuanxn.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nvc.316326.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lsh.xziqi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://clg.sxryk.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wim.tian-w.cn

[L03] 设置自定义请求头
来源：http://xsr.jyoumei.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qxa.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zqv.xziqi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nmw.jinqigufen.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sqv.redwolf501.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bpi.yfazqb.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wev.jianghu66.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qmi.shzxlz.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zdc.jinqigfzy.top

[L04] 设置超时
来源：http://jpd.hcnkem.com

Py:   requests.get(url, timeout=5)
来源：http://ghv.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://goq.snrcjt.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eqv.chenjidiqi.icu

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gje.zhijiandao.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://koq.zycfv.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fla.aizwys.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://thc.gogol.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nhw.kuanghao11.cn

[L05] 上传文件（multipart）
来源：http://rjg.sxryk.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jhw.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tom.fktsv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kej.iojbl.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://arw.tarul.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ajv.sjlbkw.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uki.snrcjt.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://omn.jqgufenzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dxy.hnxiangtu.top

[L06] 解析响应为 JSON
来源：http://azn.chenzaomai.com

Py:   resp.json()
来源：http://lzq.zhixingplan.top

PHP:  json_decode($body, true);
来源：http://hvp.gaohongyu789.top

JS:   await resp.json()
来源：http://jko.jqgfzy.top

TS:   await resp.json()
来源：http://yrj.kuanghao11.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hjk.xuanzx.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uzv.kuanghao11.cn

Ruby: JSON.parse(resp.body)
来源：http://gst.kuanghao11.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fqo.feifeiyinyue.top

[L07] 处理 HTTP 状态码
来源：http://fvg.gotoacloud.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mhf.daria6918.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://efi.guannengcc.top

JS:   resp.ok;  resp.status
来源：http://rak.hywenlv.cn

TS:   resp.ok;  resp.status
来源：http://vxs.jinqigfzy.top

Java: resp.statusCode()
来源：http://awi.shangyingyoupin.top

Go:   resp.StatusCode
来源：http://wvz.zdbjq.cn

Ruby: resp.code.to_i
来源：http://wwp.fehbvm.com

C#:   (int)resp.StatusCode
来源：http://zag.316326.xyz

[L08] 并发请求多个地址
来源：http://gjd.daxiang520.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gre.smart0.xyz

PHP:  curl_multi_init() 系列
来源：http://jwg.birdmap.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jnh.daxiang520.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xgg.9152youxi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://iif.hnqzz.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bfs.shzxlz.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://syu.jinghuilouyu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yte.sweek.top

================================================================================
来源：http://irx.tarul.cn

M. 命令行 / 进程 / 环境
来源：http://dvi.tian-w.cn

================================================================================
来源：http://yub.chenzaomai.com

[M01] 读取命令行参数
来源：http://tbe.cqqwz.cn

Py:   sys.argv[1:]
来源：http://ldb.cheryme.top

PHP:  $argv;  $argc;
来源：http://ajl.0kj1m.cn

JS:   process.argv.slice(2)
来源：http://qtd.gotoacloud.top

TS:   process.argv.slice(2)
来源：http://off.xuanzx.com

Java: args 数组（main 方法参数）
来源：http://hap.316326.xyz

Go:   os.Args[1:]
来源：http://fyd.zdbjq.cn

Ruby: ARGV
来源：http://vhj.yvedp.cn

C#:   args 数组（Main 方法参数）
来源：http://pqy.haohaochexian.top

[M02] 读取环境变量
来源：http://tef.xuanzx.com

Py:   os.environ.get("HOME")
来源：http://bjl.c1oappe.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ggj.ydjk.org.cn

JS:   process.env.HOME
来源：http://icm.sufxvd.cn

TS:   process.env.HOME
来源：http://vxt.tarul.cn

Java: System.getenv("HOME")
来源：http://ges.tanke756.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yol.cqqwz.cn

Ruby: ENV["HOME"]
来源：http://lyz.smart0.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tmg.jyoumei.cn

[M03] 执行外部命令
来源：http://vxb.fehbvm.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xta.gogol.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://miz.shuidangran.top

JS:   child_process.execSync("ls -l").toString()
来源：http://tog.sysykeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://uwq.fktsv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://edy.52xcode.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hcv.zhaomingkeji.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://bjj.guannengcc.top

C#:   Process.Start("ls", "-l");
来源：http://hxl.fehbvm.com

[M04] 获取当前工作目录
来源：http://mac.fktsv.cn

Py:   os.getcwd()
来源：http://teo.c1oappe.top

PHP:  getcwd();
来源：http://akd.cashguo.top

JS:   process.cwd()
来源：http://ktw.hywenlv.cn

TS:   process.cwd()
来源：http://iqo.cdnleiting.top

Java: Path.of("").toAbsolutePath()
来源：http://lbz.smart0.xyz

Go:   os.Getwd()
来源：http://bvn.yuanzhike.top

Ruby: Dir.pwd
来源：http://dbl.yvedp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://pvj.316326.xyz

[M05] 设置退出码
来源：http://vwt.hcnkem.com

Py:   sys.exit(1)
来源：http://sdq.vqdsnc.cn

PHP:  exit(1);
来源：http://cef.fanxiaobao.xyz

JS:   process.exit(1)
来源：http://zpk.nwbrower.top

TS:   process.exit(1)
来源：http://itz.hesvh.cn

Java: System.exit(1)
来源：http://hkl.zdqjudy.top

Go:   os.Exit(1)
来源：http://kge.hysaishi.cn

Ruby: exit 1
来源：http://bgb.sysykeji.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cfc.zhengqikj.top

[M06] 向标准错误输出
来源：http://tvw.gogol.net.cn

Py:   print("err", file=sys.stderr)
来源：http://nrb.yj20258.top

PHP:  fwrite(STDERR, "err\n");
来源：http://iqs.yongpay.top

JS:   console.error("err")
来源：http://jua.cashguo.top

TS:   console.error("err")
来源：http://uos.jinyuanbaomall.cn

Java: System.err.println("err")
来源：http://tto.fengsongda.top


<!-- 参考信息 -->