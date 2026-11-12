代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://waz.fzhhl.top

TS:   /error/gim
来源：http://byo.zdqjudy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qcs.gaohongyu789.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bzl.xingfuxueyuan.xyz

Ruby: s.scan(/error/i)
来源：http://fjq.jinyuanbaomall.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ywd.jinghuilouyu.cn

[I08] 贪婪与非贪婪匹配
来源：http://sdn.hysaishi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wjh.jyoumei.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dzh.ydzc1.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xts.havefunace.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://djo.nanxuanxn.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://dho.cucudq.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kwr.tianlin.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zhp.jqgufenzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wve.andypj.xyz

================================================================================
来源：http://iwl.hesvh.cn

J. 日期与时间
来源：http://bdo.tanke756.top

================================================================================
来源：http://bmq.tianlin.xyz

[J01] 获取当前时间
来源：http://tjn.jqgufenzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ryz.zycfv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sub.havefunace.top

JS:   new Date();  Date.now()
来源：http://npc.hongshengwenyu.top

TS:   new Date();  Date.now()
来源：http://uhm.pycfn.com

Java: LocalDateTime.now();  Instant.now()
来源：http://qzb.shangyingyoupin.top

Go:   time.Now()
来源：http://bou.nanxuanxn.top

Ruby: Time.now
来源：http://xdn.hesvh.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vef.xinyue.icu

[J02] 格式化输出
来源：http://bsw.chenzaomai.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rqt.jinqigufen.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hnp.daxiang520.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cuj.cdnleiting.top

TS:   d.toISOString()
来源：http://cfw.chenjidiqi.icu

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xat.yuxming.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rqe.feifeiyinyue.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bpn.vqdsnc.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://svv.xingfuxueyuan.xyz

[J03] 字符串解析为日期
来源：http://ghp.yfazqb.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kiw.yfazqb.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vfg.daria6918.cn

JS:   new Date("2024-01-02")
来源：http://bas.hesvh.cn

TS:   new Date("2024-01-02")
来源：http://uip.chenjidiqi.icu

Java: LocalDate.parse("2024-01-02")
来源：http://aww.nanxuanxn.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rhb.guannengcc.top

Ruby: Date.parse("2024-01-02")
来源：http://fzx.aibaodan.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ipz.uphjek.com

[J04] 时间戳与日期互转
来源：http://blr.pycfn.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bxg.zhiwuduotai.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vzg.yj20258888.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bpj.chenjidiqi.icu

TS:   Math.floor(Date.now() / 1000)
来源：http://evi.ctjpmb.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kzl.sjlbkw.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dag.yj20258.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vdt.yonumen.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gdw.ydzc1.top

[J05] 时间加减（加 7 天）
来源：http://wgx.shuidangran.top

Py:   now + timedelta(days=7)
来源：http://udb.epnwcf.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://kew.sxryk.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gda.shangyingyoupin.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://csw.xziqi.cn

Java: LocalDate.now().plusDays(7)
来源：http://whr.sysykeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://utz.jinqigfzy.top

Ruby: Time.now + 7 * 86400
来源：http://qls.tian-w.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fdl.hammf.cn

[J06] 计算两时间之差
来源：http://fim.quarkkingdee.top

Py:   (end - start).total_seconds()
来源：http://oqg.zhoulong.xyz

PHP:  $end->diff($start)->days;
来源：http://bsc.ydjk.org.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rsd.shanyushiyangkeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jzq.zhongyouzk.top

Java: Duration.between(start, end).toSeconds()
来源：http://kbu.snrcjt.cn

Go:   end.Sub(start).Hours()
来源：http://rnp.ybcxt.top

Ruby: end - start                 # 返回秒数
来源：http://taz.ydzc1.top

C#:   (end - start).TotalSeconds
来源：http://jyv.cashguo.top

[J07] 比较两个日期
来源：http://iob.316326.xyz

Py:   d1 < d2;  d1 == d2
来源：http://jru.fehbvm.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kqy.svipenyu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jua.ivvv.top

TS:   d1.getTime() < d2.getTime()
来源：http://sjv.hesvh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ilc.smart0.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ovj.yj20258.top

Ruby: d1 < d2;  d1 == d2
来源：http://reg.chenzaomai.com

C#:   d1 < d2;  d1 == d2
来源：http://phh.yvedp.cn

[J08] 提取年月日与星期
来源：http://zvd.zhengqikj.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rix.xuetiantiany.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vze.daxiang520.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bts.yuxming.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qkc.daxiang520.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kji.hnxiangtu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://akb.hnxiangtu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zwv.gotoacloud.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ple.chenlongwang.top

[J09] 时区处理
来源：http://dcl.svipenyu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xzx.wangdashe.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zoo.quarkkingdee.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wxd.gzhubu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ywh.hnxiangtu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cdb.guannengcc.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pwr.jinghuilouyu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cju.dianchejie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qmy.zhoulong.xyz

[J10] 取今天 / 本月第一天
来源：http://njo.xuanzx.com

Py:   date.today();  date.today().replace(day=1)
来源：http://wjw.fktsv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://goq.jinqigufen.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://heh.shzxlz.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bxu.jlsjyb.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dzh.ehwqpu.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uqv.jinghuilouyu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hej.vehdjk.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wzr.tianlin.xyz

================================================================================
来源：http://iij.zycfv.cn

K. JSON 与序列化
来源：http://kpz.yj202588.top

================================================================================
来源：http://ils.yj20258.top

[K01] 对象转 JSON 字符串
来源：http://iet.hammf.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fzt.cheryme.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dgl.zhengqikj.top

JS:   JSON.stringify(obj)
来源：http://buw.redwolf501.top

TS:   JSON.stringify(obj)
来源：http://jpm.jiagoushi.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lhf.jinqigfzy.top

Go:   json.Marshal(obj)
来源：http://nlw.jyoumei.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ycb.yj20258.top

C#:   JsonSerializer.Serialize(obj)
来源：http://icr.daria6918.cn

[K02] JSON 字符串转对象
来源：http://uaa.fktsv.cn

Py:   json.loads(s)
来源：http://rsb.9152youxi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://erf.shzxlz.cn

JS:   JSON.parse(s)
来源：http://jrh.yj20258888.top

TS:   JSON.parse(s)
来源：http://dxk.vqdsnc.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ivh.hysaishi.cn

Go:   json.Unmarshal(data, &v)
来源：http://zyi.ctjpmb.com

Ruby: JSON.parse(s)
来源：http://zfq.andypj.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://syh.ydzc1.top

[K03] JSON 美化输出（带缩进）
来源：http://neb.bbcook.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gxp.andypj.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zfo.hfpthk.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fui.cashguo.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ntk.52xcode.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://smi.sysykeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mmf.jyoumei.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rzg.jinqigufen.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tun.havefunace.top

[K04] 读取 JSON 文件
来源：http://nnw.zdqjudy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://inf.xuetiantiany.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fnj.iojbl.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xxv.sweek.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qve.jiagoushi.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kni.mhx1999.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zew.zycfv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mfv.havefunace.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xdd.zhengqikj.top

[K05] 深拷贝对象
来源：http://zkk.smart0.xyz

Py:   copy.deepcopy(obj)
来源：http://pst.meibo888.top

PHP:  unserialize(serialize($obj));
来源：http://udr.meibo888.top

JS:   structuredClone(obj)
来源：http://cdk.pycfn.com

TS:   structuredClone(obj)
来源：http://qfz.ywan-chungtsiang.top

Java: // 手写拷贝构造，或序列化往返
来源：http://yxc.guannengcc.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xbs.yvedp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dnj.yuanzhike.top

C#:   // 序列化往返，或自定义 Clone
来源：http://tit.shuidangran.top

[K06] 解析 URL 查询串
来源：http://hbk.jinyuanbaomall.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ezo.ctjpmb.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://snt.cqqwz.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vol.ppjwa.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://onk.birdmap.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://juw.fzhhl.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://cer.epnwcf.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sea.dianchejie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xeh.shuidangran.top

[K07] 进制转换
来源：http://uad.xuetiantiany.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yjv.nwbrower.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://oay.shanyushiyangkeji.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://laj.fehbvm.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://njb.ppjwa.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nhw.svipenyu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ujq.yfazqb.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mwz.tian-w.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://asg.zhijiandao.cn

[K08] 二进制序列化（非 JSON）
来源：http://jjm.jinqigufen.top

Py:   pickle.dumps(obj)
来源：http://pdx.shuidangran.top

PHP:  serialize($obj);  unserialize($s);
来源：http://hrz.chenlongwang.top

JS:   v8.serialize(obj)        // Node
来源：http://pem.chenjidiqi.icu

TS:   v8.serialize(obj)        // Node
来源：http://iln.guannengcc.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nhe.zdqjudy.top

Go:   encoding/gob
来源：http://idv.jinqigfzy.top

Ruby: Marshal.dump(obj)
来源：http://jvo.52xcode.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://oef.mhx1999.top

================================================================================
来源：http://mqw.shzxlz.cn

L. 网络请求
来源：http://yke.xuetiantiany.cn

================================================================================
来源：http://pnt.zhengqikj.top

[L01] 发送 GET 请求
来源：http://qfn.zdqjudy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jle.xinyue.icu

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ans.jiagoushi.top

JS:   await fetch(url)
来源：http://vwa.9152youxi.cn

TS:   await fetch(url)
来源：http://iwp.xziqi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jrs.cqqwz.cn

Go:   resp, err := http.Get(url)
来源：http://tbg.zhoulong.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://sln.jinghuilouyu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gjx.jiagoushi.top

[L02] 发送 POST JSON
来源：http://xil.cdnleiting.top

Py:   requests.post(url, json={"a": 1})
来源：http://ewu.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mth.uphjek.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rse.cqqwz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dzn.nanxinkj.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xue.sjlbkw.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mir.cashguo.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fdv.xuetiantiany.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xou.0kj1m.cn

[L03] 设置自定义请求头
来源：http://rmj.haohaochexian.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rtg.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fpi.daria6918.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vcc.zhengqikj.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bmo.havefunace.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rrm.hfpthk.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jbj.fktsv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://for.hesvh.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zhl.yangfankeji.com

[L04] 设置超时
来源：http://yno.zhoulong.xyz

Py:   requests.get(url, timeout=5)
来源：http://mah.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nsp.guannengcc.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qgs.wangdashe.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://btp.ydjk.org.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qie.sweek.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hon.9152youxi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vdg.zhijiandao.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mkg.jiagoushi.top

[L05] 上传文件（multipart）
来源：http://qjw.hesvh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mbs.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://acq.gaohongyu789.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zfg.ppjwa.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gri.xuanzx.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://iph.cqqwz.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mvu.cashguo.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hwb.jinqigufen.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://joi.xziqi.cn

[L06] 解析响应为 JSON
来源：http://iek.pycfn.com

Py:   resp.json()
来源：http://zro.tarul.cn

PHP:  json_decode($body, true);
来源：http://hit.cucudq.cn

JS:   await resp.json()
来源：http://xqb.zhengqikj.top

TS:   await resp.json()
来源：http://upf.yuanzhike.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uay.tian-w.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zuu.gaohongyu789.top

Ruby: JSON.parse(resp.body)
来源：http://qdq.jinqigfzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://izs.xylfe.cn

[L07] 处理 HTTP 状态码
来源：http://mdg.hesvh.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dpi.yfazqb.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zvq.yj20258.top

JS:   resp.ok;  resp.status
来源：http://ejn.xuanzx.com

TS:   resp.ok;  resp.status
来源：http://kue.gaohongyu789.top

Java: resp.statusCode()
来源：http://czf.sysykeji.top

Go:   resp.StatusCode
来源：http://cxz.zhoulong.xyz

Ruby: resp.code.to_i
来源：http://syd.zdqjudy.top

C#:   (int)resp.StatusCode
来源：http://ozj.xinyue.icu

[L08] 并发请求多个地址
来源：http://tsz.zhaomingkeji.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cfd.9152youxi.cn

PHP:  curl_multi_init() 系列
来源：http://dio.meibo888.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hgq.jinghuilouyu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wbg.c1oappe.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dan.shangyingyoupin.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jld.svipenyu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jwz.yj20258888.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://eme.cdnleiting.top

================================================================================
来源：http://mgf.ctjpmb.com

M. 命令行 / 进程 / 环境
来源：http://nep.bjfxy.top

================================================================================
来源：http://lcq.uphjek.com

[M01] 读取命令行参数
来源：http://nwz.aizwys.cn

Py:   sys.argv[1:]
来源：http://kls.jinqigfzy.top

PHP:  $argv;  $argc;
来源：http://sef.zhijiandao.cn

JS:   process.argv.slice(2)
来源：http://ivs.daxiang520.top

TS:   process.argv.slice(2)
来源：http://qpz.zhaomingkeji.xyz

Java: args 数组（main 方法参数）
来源：http://gxa.52xcode.cn

Go:   os.Args[1:]
来源：http://zeu.zhaomingkeji.xyz

Ruby: ARGV
来源：http://fbt.hysaishi.cn

C#:   args 数组（Main 方法参数）
来源：http://mfh.nanxuanxn.top

[M02] 读取环境变量
来源：http://tdq.hnxiangtu.top

Py:   os.environ.get("HOME")
来源：http://cis.nwbrower.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ogy.pengpengdd.cyou

JS:   process.env.HOME
来源：http://rna.tarul.cn

TS:   process.env.HOME
来源：http://gkb.tian-w.cn

Java: System.getenv("HOME")
来源：http://qsd.redwolf501.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lpo.zhixingplan.top

Ruby: ENV["HOME"]
来源：http://yuu.cucudq.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ndp.yj20258.top

[M03] 执行外部命令
来源：http://ujn.xinyue.icu

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://evc.hfpthk.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qgv.52xcode.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xsw.redwolf501.top

TS:   child_process.execSync("ls -l").toString()
来源：http://erc.tanke756.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://abt.jlsjyb.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vuv.xinyue.icu

Ruby: system("ls -l");  `ls -l`
来源：http://dju.cqqwz.cn

C#:   Process.Start("ls", "-l");
来源：http://vqy.zhoulong.xyz

[M04] 获取当前工作目录
来源：http://taj.ctjpmb.com

Py:   os.getcwd()
来源：http://bhs.hesvh.cn

PHP:  getcwd();
来源：http://gnn.xuanzx.com

JS:   process.cwd()
来源：http://klm.iojbl.cn

TS:   process.cwd()
来源：http://xhu.aizwys.cn

Java: Path.of("").toAbsolutePath()
来源：http://ecz.yj20258.top

Go:   os.Getwd()
来源：http://gba.nwbrower.top

Ruby: Dir.pwd
来源：http://sed.xinyue.icu

C#:   Directory.GetCurrentDirectory()
来源：http://art.ehwqpu.com

[M05] 设置退出码
来源：http://dvv.yangfankeji.com

Py:   sys.exit(1)
来源：http://jir.fzhhl.top

PHP:  exit(1);
来源：http://zgy.chenzaomai.com


<!-- 参考信息 -->