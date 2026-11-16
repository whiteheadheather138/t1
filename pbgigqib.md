代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yey.jlsjyb.cn

[I07] 忽略大小写与多行模式
来源：http://wyd.316326.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rop.jlsjyb.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kst.mhx1999.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uji.gzhubu.top

TS:   /error/gim
来源：http://amw.daria6918.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rjl.gotoacloud.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xea.vehdjk.com

Ruby: s.scan(/error/i)
来源：http://pbe.epnwcf.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gkz.jinyuanbaomall.cn

[I08] 贪婪与非贪婪匹配
来源：http://qmd.guowangkeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://snb.ppjwa.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lyd.xziqi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bgb.sufxvd.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bxz.zhoulong.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://wqk.tianlin.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hcq.jinyuanbaomall.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://iwg.jinyuanbaomall.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dcy.dianchejie.cn

================================================================================
来源：http://jqk.jlsjyb.cn

J. 日期与时间
来源：http://eqa.guannengcc.top

================================================================================
来源：http://fgl.shanyushiyangkeji.top

[J01] 获取当前时间
来源：http://qgo.tianlin.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://bpw.tianlin.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xgr.ivvv.top

JS:   new Date();  Date.now()
来源：http://eql.bjfxy.top

TS:   new Date();  Date.now()
来源：http://fqm.uphjek.com

Java: LocalDateTime.now();  Instant.now()
来源：http://izo.shanyushiyangtech.top

Go:   time.Now()
来源：http://nsw.fktsv.cn

Ruby: Time.now
来源：http://kng.aibaodan.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sig.jinqigufen.top

[J02] 格式化输出
来源：http://pry.sysykeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yrz.zdbjq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uut.jinyuanbaomall.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ewq.hywenlv.cn

TS:   d.toISOString()
来源：http://fnd.snrcjt.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qxj.kuanghao11.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lis.chenjidiqi.icu

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ycp.sxryk.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kyw.hesvh.cn

[J03] 字符串解析为日期
来源：http://vol.dianchejie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lyx.tanke756.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ene.ctjpmb.com

JS:   new Date("2024-01-02")
来源：http://rrj.gogol.net.cn

TS:   new Date("2024-01-02")
来源：http://nkb.ydzc1.top

Java: LocalDate.parse("2024-01-02")
来源：http://vwh.xuetiantiany.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://amr.ivvv.top

Ruby: Date.parse("2024-01-02")
来源：http://vzo.sysykeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://idv.gogol.net.cn

[J04] 时间戳与日期互转
来源：http://kpv.dianchejie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://coo.316326.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cik.jyoumei.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nsh.zdqjudy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://aul.ydzc1.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hqs.zhongyouzk.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gpw.jyoumei.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pbx.ppjwa.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bsv.yvedp.cn

[J05] 时间加减（加 7 天）
来源：http://yce.pengpengdd.cyou

Py:   now + timedelta(days=7)
来源：http://qho.guowangkeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://tpr.jinqigfzy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rzi.bjfxy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://aya.xuetiantiany.cn

Java: LocalDate.now().plusDays(7)
来源：http://xmw.cheryme.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mrg.jqgfzy.top

Ruby: Time.now + 7 * 86400
来源：http://kgp.ehwqpu.com

C#:   DateTime.Now.AddDays(7)
来源：http://cvz.hcnkem.com

[J06] 计算两时间之差
来源：http://iem.yuxming.cn

Py:   (end - start).total_seconds()
来源：http://afv.hysaishi.cn

PHP:  $end->diff($start)->days;
来源：http://hxs.jinghuilouyu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wbz.yuxming.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://msj.chenjidiqi.icu

Java: Duration.between(start, end).toSeconds()
来源：http://gkr.vqdsnc.cn

Go:   end.Sub(start).Hours()
来源：http://ziz.zhaomingkeji.xyz

Ruby: end - start                 # 返回秒数
来源：http://cdk.gzhubu.top

C#:   (end - start).TotalSeconds
来源：http://gyi.daria6918.cn

[J07] 比较两个日期
来源：http://rkh.mhx1999.top

Py:   d1 < d2;  d1 == d2
来源：http://cyt.pycfn.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qru.hnxiangtu.top

JS:   d1.getTime() < d2.getTime()
来源：http://nvp.fanxiaobao.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://gar.shangyingyoupin.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://why.tian-w.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ade.haohaochexian.top

Ruby: d1 < d2;  d1 == d2
来源：http://nuq.pycfn.com

C#:   d1 < d2;  d1 == d2
来源：http://ugp.jqgfzy.top

[J08] 提取年月日与星期
来源：http://rjh.c1oappe.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fcy.hongshengwenyu.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nud.fanxiaobao.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pwe.yj202588.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ybk.fzhhl.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uzs.andypj.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://leo.shanyushiyangtech.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yop.haohaochexian.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zuc.tianlin.xyz

[J09] 时区处理
来源：http://trz.aibaodan.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uhv.hysaishi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://amg.zhijiandao.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hoe.0kj1m.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://frm.ydjk.org.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xhd.zhiwuduotai.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hnb.gotoacloud.top

Ruby: Time.now.getlocal("+08:00")
来源：http://hps.birdmap.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xsb.cdnleiting.top

[J10] 取今天 / 本月第一天
来源：http://gha.zhaomingkeji.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://inw.vehdjk.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://few.feifeiyinyue.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://msq.pycfn.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zeg.fengsongda.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zjm.sysykeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qfl.shanyushiyangtech.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uqf.316326.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gpc.xziqi.cn

================================================================================
来源：http://ijy.nwbrower.top

K. JSON 与序列化
来源：http://itm.yueranfly.top

================================================================================
来源：http://mbu.shzxlz.cn

[K01] 对象转 JSON 字符串
来源：http://cuz.ehwqpu.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rkf.xingfuxueyuan.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rsk.hcnkem.com

JS:   JSON.stringify(obj)
来源：http://bja.gogol.net.cn

TS:   JSON.stringify(obj)
来源：http://zyx.xziqi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://loh.jinqigfzy.top

Go:   json.Marshal(obj)
来源：http://mbj.cucudq.cn

Ruby: obj.to_json                                     // require "json"
来源：http://szi.xinyue.icu

C#:   JsonSerializer.Serialize(obj)
来源：http://xun.kuanghao11.cn

[K02] JSON 字符串转对象
来源：http://utr.tanke756.top

Py:   json.loads(s)
来源：http://evt.xylfe.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ekl.jinqigufen.top

JS:   JSON.parse(s)
来源：http://pec.yvedp.cn

TS:   JSON.parse(s)
来源：http://swf.svipenyu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fzz.zhixingplan.top

Go:   json.Unmarshal(data, &v)
来源：http://lvj.epnwcf.com

Ruby: JSON.parse(s)
来源：http://hsy.ivvv.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wpl.yonumen.top

[K03] JSON 美化输出（带缩进）
来源：http://few.xuetiantiany.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ugy.feifeiyinyue.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bov.yj202588.top

JS:   JSON.stringify(obj, null, 2)
来源：http://vse.zycfv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wgb.guannengcc.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://url.cheryme.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nmb.nanxinkj.top

Ruby: JSON.pretty_generate(obj)
来源：http://ybm.yangfankeji.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jxa.hammf.cn

[K04] 读取 JSON 文件
来源：http://jfh.meibo888.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vmx.jinyuanbaomall.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kwb.ppjwa.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ron.guannengcc.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kwf.redwolf501.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ejk.havefunace.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://imz.pycfn.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://hsp.jinqigfzy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uzq.hesvh.cn

[K05] 深拷贝对象
来源：http://lac.birdmap.top

Py:   copy.deepcopy(obj)
来源：http://fey.jqgufenzy.top

PHP:  unserialize(serialize($obj));
来源：http://mbu.hammf.cn

JS:   structuredClone(obj)
来源：http://qqh.zdqjudy.top

TS:   structuredClone(obj)
来源：http://qiu.gaohongyu789.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ivg.gzhubu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fqt.meibo888.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wsj.sufxvd.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yyz.ivvv.top

[K06] 解析 URL 查询串
来源：http://xqr.dashuyun.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pty.xingfuxueyuan.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ukn.uphjek.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://awy.zhiwuduotai.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pek.sxryk.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wfa.shzxlz.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ytw.chenzaomai.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://amp.snrcjt.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tsx.yonumen.top

[K07] 进制转换
来源：http://tyd.yj20258888.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oiw.pycfn.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://amx.yueranfly.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tfh.smart0.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dex.xinyue.icu

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ofu.tian-w.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pnm.cashguo.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rxy.jqgufenzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://app.quarkkingdee.top

[K08] 二进制序列化（非 JSON）
来源：http://oqv.iojbl.cn

Py:   pickle.dumps(obj)
来源：http://cbw.gaohongyu789.top

PHP:  serialize($obj);  unserialize($s);
来源：http://gfs.yongpay.top

JS:   v8.serialize(obj)        // Node
来源：http://hny.shzxlz.cn

TS:   v8.serialize(obj)        // Node
来源：http://xae.ehwqpu.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://idg.chenzaomai.com

Go:   encoding/gob
来源：http://wwp.bjfxy.top

Ruby: Marshal.dump(obj)
来源：http://mvh.yuxming.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://atm.shangyingyoupin.top

================================================================================
来源：http://tsk.zhijiandao.cn

L. 网络请求
来源：http://mrv.cheryme.top

================================================================================
来源：http://jkn.kuanghao11.cn

[L01] 发送 GET 请求
来源：http://fef.yvedp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ngc.xuanzx.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hsl.gzhubu.top

JS:   await fetch(url)
来源：http://fdu.ppjwa.cn

TS:   await fetch(url)
来源：http://wnc.zhixingplan.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fmp.shanyushiyangkeji.top

Go:   resp, err := http.Get(url)
来源：http://vpl.yueranfly.top

Ruby: Net::HTTP.get(URI(url))
来源：http://bmm.wangdashe.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kfy.jinyuanbaomall.cn

[L02] 发送 POST JSON
来源：http://gvu.zhixingplan.top

Py:   requests.post(url, json={"a": 1})
来源：http://bad.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://psd.ydjk.org.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ffu.pycfn.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hsg.gaohongyu789.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://apl.tarul.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rmn.yvedp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://eet.shanyushiyangtech.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://apb.vqdsnc.cn

[L03] 设置自定义请求头
来源：http://iwz.xuetiantiany.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mrl.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nln.sweek.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uer.kuanghao11.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://shs.9152youxi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://clp.sxryk.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rjq.tanke756.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ngm.ppjwa.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://oss.andypj.xyz

[L04] 设置超时
来源：http://ora.yonumen.top

Py:   requests.get(url, timeout=5)
来源：http://irm.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kge.mhx1999.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://shj.hammf.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ajn.yongpay.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://alz.cqqwz.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cbs.fengsongda.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://edf.epnwcf.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gvw.jinqigfzy.top

[L05] 上传文件（multipart）
来源：http://siv.feifeiyinyue.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jdu.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zgi.yueranfly.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ytn.zhongyouzk.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kgw.zhaomingkeji.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lrg.jiagoushi.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blu.gzhubu.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fgb.vqdsnc.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zva.dashuyun.cn

[L06] 解析响应为 JSON
来源：http://ibl.daria6918.cn

Py:   resp.json()
来源：http://eyc.fengsongda.top

PHP:  json_decode($body, true);
来源：http://vzd.wangdashe.top

JS:   await resp.json()
来源：http://qbq.yangfankeji.com

TS:   await resp.json()
来源：http://lyw.0kj1m.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ouo.sweek.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ogk.xinyue.icu

Ruby: JSON.parse(resp.body)
来源：http://oah.nanxinkj.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qoc.gzhubu.top

[L07] 处理 HTTP 状态码
来源：http://tml.yanxiufei.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rme.gotoacloud.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lit.hnxiangtu.top

JS:   resp.ok;  resp.status
来源：http://box.mhx1999.top

TS:   resp.ok;  resp.status
来源：http://nuv.9152youxi.cn

Java: resp.statusCode()
来源：http://nkp.yj202588.top

Go:   resp.StatusCode
来源：http://eod.jinqigfzy.top

Ruby: resp.code.to_i
来源：http://vcy.gzhubu.top

C#:   (int)resp.StatusCode
来源：http://cnx.dianchejie.cn

[L08] 并发请求多个地址
来源：http://jfn.zhixingplan.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://grc.zhengqikj.top

PHP:  curl_multi_init() 系列
来源：http://lbj.fzhhl.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jej.fanxiaobao.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ioh.zdqjudy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hru.ctjpmb.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://poo.daxiang520.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://iqk.yonumen.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pfc.jinghuilouyu.cn

================================================================================
来源：http://ttz.zhongyouzk.top

M. 命令行 / 进程 / 环境
来源：http://qdd.yj20258888.top

================================================================================
来源：http://sjd.havefunace.top

[M01] 读取命令行参数
来源：http://qse.ehwqpu.com

Py:   sys.argv[1:]
来源：http://igv.daxiang520.top

PHP:  $argv;  $argc;
来源：http://jht.quarkkingdee.top

JS:   process.argv.slice(2)
来源：http://eju.dianchejie.cn

TS:   process.argv.slice(2)
来源：http://upe.havefunace.top

Java: args 数组（main 方法参数）
来源：http://bze.zycfv.cn

Go:   os.Args[1:]
来源：http://dib.shuidangran.top

Ruby: ARGV
来源：http://xcr.yongpay.top

C#:   args 数组（Main 方法参数）
来源：http://whp.jiagoushi.top

[M02] 读取环境变量
来源：http://wrl.redwolf501.top

Py:   os.environ.get("HOME")
来源：http://krw.yj202588.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gty.zycfv.cn

JS:   process.env.HOME
来源：http://hlz.9152youxi.cn

TS:   process.env.HOME
来源：http://bqm.hfpthk.cn

Java: System.getenv("HOME")
来源：http://tjj.snrcjt.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vxo.haohaochexian.top

Ruby: ENV["HOME"]
来源：http://tar.xingfuxueyuan.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ntb.52xcode.cn

[M03] 执行外部命令
来源：http://gni.uphjek.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qlp.ywan-chungtsiang.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dsf.shanyushiyangkeji.top

JS:   child_process.execSync("ls -l").toString()
来源：http://xey.yuxming.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xwk.bjfxy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qmn.jiagoushi.top

Go:   exec.Command("ls", "-l").Output()
来源：http://mst.snrcjt.cn

Ruby: system("ls -l");  `ls -l`
来源：http://puw.cucudq.cn

C#:   Process.Start("ls", "-l");
来源：http://ufk.mhx1999.top

[M04] 获取当前工作目录
来源：http://aej.iojbl.cn

Py:   os.getcwd()
来源：http://czd.fengsongda.top

PHP:  getcwd();
来源：http://jee.fengsongda.top

JS:   process.cwd()
来源：http://hfv.hywenlv.cn

TS:   process.cwd()
来源：http://goe.fanxiaobao.xyz

Java: Path.of("").toAbsolutePath()
来源：http://eam.uphjek.com

Go:   os.Getwd()
来源：http://lov.yfazqb.com

Ruby: Dir.pwd
来源：http://abq.aizwys.cn


<!-- 参考信息 -->