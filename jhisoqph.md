代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xmt.cucudq.cn

TS:   /error/gim
来源：http://rmq.cashguo.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ytl.yj202588.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jho.yj20258888.top

Ruby: s.scan(/error/i)
来源：http://yvx.xuanzx.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fqc.jinqigfzy.top

[I08] 贪婪与非贪婪匹配
来源：http://euo.tian-w.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yhg.sxryk.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fdy.hfpthk.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xsp.xinyue.icu

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rkg.vqdsnc.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://yyp.xinyue.icu

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jzh.jinghuilouyu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cvj.xylfe.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://agf.jlsjyb.cn

================================================================================
来源：http://lrb.jianghu66.top

J. 日期与时间
来源：http://dkr.fengsongda.top

================================================================================
来源：http://ntz.yanxiufei.cn

[J01] 获取当前时间
来源：http://pfx.andypj.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://ngq.jyoumei.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gmx.ppjwa.cn

JS:   new Date();  Date.now()
来源：http://dxr.fktsv.cn

TS:   new Date();  Date.now()
来源：http://ply.cheryme.top

Java: LocalDateTime.now();  Instant.now()
来源：http://qrt.chenzaomai.com

Go:   time.Now()
来源：http://arf.guowangkeji.top

Ruby: Time.now
来源：http://gqb.jyoumei.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yui.ppjwa.cn

[J02] 格式化输出
来源：http://oxt.zhijiandao.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hxy.cashguo.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jib.kuanghao11.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bpt.yj20258888.top

TS:   d.toISOString()
来源：http://ast.nanxinkj.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fhj.xziqi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://uzr.wangdashe.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hjq.jinyuanbaomall.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://emt.andypj.xyz

[J03] 字符串解析为日期
来源：http://uyc.bbcook.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hli.iojbl.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yew.cheryme.top

JS:   new Date("2024-01-02")
来源：http://bzi.ivvv.top

TS:   new Date("2024-01-02")
来源：http://wfc.yongpay.top

Java: LocalDate.parse("2024-01-02")
来源：http://lek.nwbrower.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://edy.sufxvd.cn

Ruby: Date.parse("2024-01-02")
来源：http://dpy.ehwqpu.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://abv.gotoacloud.top

[J04] 时间戳与日期互转
来源：http://phz.0kj1m.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tcm.zdqjudy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pye.hesvh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tnh.dashuyun.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://roo.shzxlz.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://acm.shanyushiyangtech.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jom.jinqigufen.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tgd.yueranfly.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lks.hysaishi.cn

[J05] 时间加减（加 7 天）
来源：http://lhy.ehwqpu.com

Py:   now + timedelta(days=7)
来源：http://agp.sufxvd.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://spj.zhengqikj.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wux.zhoulong.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pxs.mhx1999.top

Java: LocalDate.now().plusDays(7)
来源：http://zyb.sufxvd.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hyv.meibo888.top

Ruby: Time.now + 7 * 86400
来源：http://eue.epnwcf.com

C#:   DateTime.Now.AddDays(7)
来源：http://cwj.jinqigfzy.top

[J06] 计算两时间之差
来源：http://xuy.iojbl.cn

Py:   (end - start).total_seconds()
来源：http://uts.shuidangran.top

PHP:  $end->diff($start)->days;
来源：http://nez.fengsongda.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yow.fehbvm.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fze.vehdjk.com

Java: Duration.between(start, end).toSeconds()
来源：http://vtn.hammf.cn

Go:   end.Sub(start).Hours()
来源：http://yhd.redwolf501.top

Ruby: end - start                 # 返回秒数
来源：http://bst.smart0.xyz

C#:   (end - start).TotalSeconds
来源：http://hob.fktsv.cn

[J07] 比较两个日期
来源：http://noe.yj20258888.top

Py:   d1 < d2;  d1 == d2
来源：http://hmw.dashuyun.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://eeu.ppjwa.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bcu.jyoumei.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vmj.jianghu66.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lsf.nanxuanxn.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wcd.yongpay.top

Ruby: d1 < d2;  d1 == d2
来源：http://yxw.hongshengwenyu.top

C#:   d1 < d2;  d1 == d2
来源：http://bjd.yuxming.cn

[J08] 提取年月日与星期
来源：http://ulq.316326.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://brb.xuetiantiany.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hcb.yj202588.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tnu.cdnleiting.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://imn.pycfn.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://drw.pycfn.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nwb.cqqwz.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hdr.jinyuanbaomall.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mdn.xingfuxueyuan.xyz

[J09] 时区处理
来源：http://sdk.jqgfzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qdd.jyoumei.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://say.xuanzx.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mlv.smart0.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://com.ehwqpu.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kyd.hammf.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vuz.wangdashe.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qbq.fzhhl.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gmq.aizwys.cn

[J10] 取今天 / 本月第一天
来源：http://jqf.yj20258888.top

Py:   date.today();  date.today().replace(day=1)
来源：http://tbx.ctjpmb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uij.snrcjt.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ert.tianlin.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ljw.316326.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zqv.0kj1m.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cuc.nwbrower.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rve.pycfn.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uwa.pycfn.com

================================================================================
来源：http://zer.svipenyu.cn

K. JSON 与序列化
来源：http://cks.iojbl.cn

================================================================================
来源：http://avn.yangfankeji.com

[K01] 对象转 JSON 字符串
来源：http://mec.zhongyouzk.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ydm.hnxiangtu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://njs.yangfankeji.com

JS:   JSON.stringify(obj)
来源：http://bmh.iojbl.cn

TS:   JSON.stringify(obj)
来源：http://efp.tarul.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lmo.yueranfly.top

Go:   json.Marshal(obj)
来源：http://kkn.xingfuxueyuan.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://kik.jianghu66.top

C#:   JsonSerializer.Serialize(obj)
来源：http://cfx.guannengcc.top

[K02] JSON 字符串转对象
来源：http://xgd.gaohongyu789.top

Py:   json.loads(s)
来源：http://yrt.fktsv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fls.yfazqb.com

JS:   JSON.parse(s)
来源：http://yjp.cashguo.top

TS:   JSON.parse(s)
来源：http://usj.yj202588.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tfb.ppjwa.cn

Go:   json.Unmarshal(data, &v)
来源：http://ddn.jinqigufen.top

Ruby: JSON.parse(s)
来源：http://rok.jinqigufen.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ldc.daxiang520.top

[K03] JSON 美化输出（带缩进）
来源：http://bhl.xuetiantiany.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://acq.shanyushiyangkeji.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xga.ivvv.top

JS:   JSON.stringify(obj, null, 2)
来源：http://xxc.jinghuilouyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ebl.guowangkeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rpi.daxiang520.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jtd.yj202588.top

Ruby: JSON.pretty_generate(obj)
来源：http://ehc.cdnleiting.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nke.bjfxy.top

[K04] 读取 JSON 文件
来源：http://zdr.dianchejie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qqi.mhx1999.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pyc.hnqzz.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vzh.redwolf501.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tka.zdqjudy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jqk.ppjwa.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pxq.ivvv.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://uaa.xinyue.icu

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pda.jyoumei.cn

[K05] 深拷贝对象
来源：http://tps.zhoulong.xyz

Py:   copy.deepcopy(obj)
来源：http://cug.mhx1999.top

PHP:  unserialize(serialize($obj));
来源：http://dgq.ctjpmb.com

JS:   structuredClone(obj)
来源：http://dvm.daxiang520.top

TS:   structuredClone(obj)
来源：http://qxf.quarkkingdee.top

Java: // 手写拷贝构造，或序列化往返
来源：http://yco.gogol.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bum.iojbl.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gns.gaohongyu789.top

C#:   // 序列化往返，或自定义 Clone
来源：http://xry.fehbvm.com

[K06] 解析 URL 查询串
来源：http://jou.bjfxy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hca.wangdashe.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xmh.kuanghao11.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mzd.zdbjq.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://teh.uphjek.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://znc.ydjk.org.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qrq.yangfankeji.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vmd.vehdjk.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sfq.shanyushiyangtech.top

[K07] 进制转换
来源：http://ayq.sxryk.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hjt.yfazqb.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://iah.yanxiufei.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://frp.sxryk.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tzo.jyoumei.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ing.jinqigufen.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lby.ydzc1.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://twa.vehdjk.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kvd.yj20258.top

[K08] 二进制序列化（非 JSON）
来源：http://skx.smart0.xyz

Py:   pickle.dumps(obj)
来源：http://ogv.havefunace.top

PHP:  serialize($obj);  unserialize($s);
来源：http://nph.pycfn.com

JS:   v8.serialize(obj)        // Node
来源：http://kfp.chenlongwang.top

TS:   v8.serialize(obj)        // Node
来源：http://ykj.jiagoushi.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rve.hysaishi.cn

Go:   encoding/gob
来源：http://tsf.hnqzz.top

Ruby: Marshal.dump(obj)
来源：http://kpe.vqdsnc.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zld.jinyuanbaomall.cn

================================================================================
来源：http://ygp.svipenyu.cn

L. 网络请求
来源：http://mvq.zdbjq.cn

================================================================================
来源：http://hdl.tanke756.top

[L01] 发送 GET 请求
来源：http://vvt.jianghu66.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kif.vqdsnc.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nby.shanyushiyangkeji.top

JS:   await fetch(url)
来源：http://uaz.ybcxt.top

TS:   await fetch(url)
来源：http://ckm.zhengqikj.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wmr.nanxuanxn.top

Go:   resp, err := http.Get(url)
来源：http://jhx.yangfankeji.com

Ruby: Net::HTTP.get(URI(url))
来源：http://fxr.ybcxt.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dmj.zhaomingkeji.xyz

[L02] 发送 POST JSON
来源：http://vtu.chenjidiqi.icu

Py:   requests.post(url, json={"a": 1})
来源：http://zzz.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://oxe.jinyuanbaomall.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cdc.xuanzx.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cuj.cqqwz.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xqm.hfpthk.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://iph.jqgufenzy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vjp.0kj1m.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://brm.ivvv.top

[L03] 设置自定义请求头
来源：http://tuw.tian-w.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dhn.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sfl.zycfv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rjk.nwbrower.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ial.jlsjyb.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jxl.zhoulong.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tfn.zhengqikj.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://clr.chenzaomai.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xbx.yangfankeji.com

[L04] 设置超时
来源：http://meh.hongshengwenyu.top

Py:   requests.get(url, timeout=5)
来源：http://cqj.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tik.yanxiufei.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vkh.jinghuilouyu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qyl.hnxiangtu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ogi.mhx1999.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pts.ctjpmb.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rcj.jqgfzy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nnz.jyoumei.cn

[L05] 上传文件（multipart）
来源：http://rjh.xylfe.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://htq.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fod.zhaomingkeji.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://khr.redwolf501.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uli.bjfxy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ftw.nanxinkj.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uxo.fanxiaobao.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xbv.fzhhl.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yls.zhijiandao.cn

[L06] 解析响应为 JSON
来源：http://uep.aizwys.cn

Py:   resp.json()
来源：http://psj.pengpengdd.cyou

PHP:  json_decode($body, true);
来源：http://juu.ywan-chungtsiang.top

JS:   await resp.json()
来源：http://jtz.fzhhl.top

TS:   await resp.json()
来源：http://khc.mhx1999.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://otc.fktsv.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fbo.yj20258.top

Ruby: JSON.parse(resp.body)
来源：http://qfh.ydjk.org.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mnd.guowangkeji.top

[L07] 处理 HTTP 状态码
来源：http://aqr.hfpthk.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://inc.jinyuanbaomall.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yig.yongpay.top

JS:   resp.ok;  resp.status
来源：http://jfg.jiagoushi.top

TS:   resp.ok;  resp.status
来源：http://pjf.shzxlz.cn

Java: resp.statusCode()
来源：http://iiv.nanxinkj.top

Go:   resp.StatusCode
来源：http://rrm.tian-w.cn

Ruby: resp.code.to_i
来源：http://jok.ivvv.top

C#:   (int)resp.StatusCode
来源：http://cae.yj20258888.top

[L08] 并发请求多个地址
来源：http://ilu.zdbjq.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jcq.xuetiantiany.cn

PHP:  curl_multi_init() 系列
来源：http://xxm.ppjwa.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zku.bjfxy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cze.hammf.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fff.yj20258888.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cif.zdqjudy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nek.xinyue.icu

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jjj.cashguo.top

================================================================================
来源：http://thk.haohaochexian.top

M. 命令行 / 进程 / 环境
来源：http://kyz.wangshuangyany.cn

================================================================================
来源：http://fdp.jqgufenzy.top

[M01] 读取命令行参数
来源：http://ssr.haohaochexian.top

Py:   sys.argv[1:]
来源：http://zaw.jianghu66.top

PHP:  $argv;  $argc;
来源：http://jvr.tian-w.cn

JS:   process.argv.slice(2)
来源：http://nek.jinqigufen.top

TS:   process.argv.slice(2)
来源：http://szf.tarul.cn

Java: args 数组（main 方法参数）
来源：http://zdb.jqgfzy.top

Go:   os.Args[1:]
来源：http://rlq.jiagoushi.top

Ruby: ARGV
来源：http://nrl.chenlongwang.top

C#:   args 数组（Main 方法参数）
来源：http://jbg.uphjek.com

[M02] 读取环境变量
来源：http://vhi.dianchejie.cn

Py:   os.environ.get("HOME")
来源：http://iqd.xziqi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zhs.zhixingplan.top

JS:   process.env.HOME
来源：http://yhr.fanxiaobao.xyz

TS:   process.env.HOME
来源：http://wmu.tarul.cn

Java: System.getenv("HOME")
来源：http://ady.yongpay.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cxu.andypj.xyz

Ruby: ENV["HOME"]
来源：http://kok.zdqjudy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wfr.xuetiantiany.cn

[M03] 执行外部命令
来源：http://dji.hnqzz.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jdn.aizwys.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://djn.shuidangran.top

JS:   child_process.execSync("ls -l").toString()
来源：http://olk.xingfuxueyuan.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://wop.jinghuilouyu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bpn.hnxiangtu.top

Go:   exec.Command("ls", "-l").Output()
来源：http://qay.shangyingyoupin.top

Ruby: system("ls -l");  `ls -l`
来源：http://omg.birdmap.top

C#:   Process.Start("ls", "-l");
来源：http://ikw.chenjidiqi.icu

[M04] 获取当前工作目录
来源：http://nqa.fanxiaobao.xyz

Py:   os.getcwd()
来源：http://dai.wangshuangyany.cn

PHP:  getcwd();
来源：http://akh.ehwqpu.com

JS:   process.cwd()
来源：http://kbv.sufxvd.cn

TS:   process.cwd()
来源：http://zot.9152youxi.cn

Java: Path.of("").toAbsolutePath()
来源：http://kdl.jinghuilouyu.cn

Go:   os.Getwd()
来源：http://vwg.tarul.cn

Ruby: Dir.pwd
来源：http://jdu.uphjek.com

C#:   Directory.GetCurrentDirectory()
来源：http://tba.hesvh.cn

[M05] 设置退出码
来源：http://kbx.meibo888.top

Py:   sys.exit(1)
来源：http://pfz.vqdsnc.cn

PHP:  exit(1);
来源：http://goz.yj202588.top


<!-- 参考信息 -->