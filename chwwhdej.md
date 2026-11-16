代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://aob.sweek.top

TS:   /error/gim
来源：http://ahj.ivvv.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ops.hnqzz.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wbq.ydzc1.top

Ruby: s.scan(/error/i)
来源：http://zja.aibaodan.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yhf.hnqzz.top

[I08] 贪婪与非贪婪匹配
来源：http://fym.shanyushiyangkeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xfo.yvedp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jil.zhijiandao.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://giq.xylfe.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xrs.c1oappe.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://nwe.xziqi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ljk.c1oappe.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vwc.vqdsnc.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mhn.zhijiandao.cn

================================================================================
来源：http://cpm.bbcook.cn

J. 日期与时间
来源：http://xcs.ctjpmb.com

================================================================================
来源：http://hkv.zhaomingkeji.xyz

[J01] 获取当前时间
来源：http://zjb.cqqwz.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://akg.hywenlv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vpr.quarkkingdee.top

JS:   new Date();  Date.now()
来源：http://muw.cheryme.top

TS:   new Date();  Date.now()
来源：http://quw.wangdashe.top

Java: LocalDateTime.now();  Instant.now()
来源：http://dji.hongshengwenyu.top

Go:   time.Now()
来源：http://bac.316326.xyz

Ruby: Time.now
来源：http://rgp.sufxvd.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yti.cashguo.top

[J02] 格式化输出
来源：http://htm.zycfv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tsz.sjlbkw.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hhm.sxryk.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://afi.svipenyu.cn

TS:   d.toISOString()
来源：http://ucg.gogol.net.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uyk.andypj.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://src.shzxlz.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://waa.9152youxi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bvm.pengpengdd.cyou

[J03] 字符串解析为日期
来源：http://esl.jqgufenzy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vca.hfpthk.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xpl.jqgfzy.top

JS:   new Date("2024-01-02")
来源：http://bci.cdnleiting.top

TS:   new Date("2024-01-02")
来源：http://efl.zdbjq.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vcr.gogol.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xjn.gaohongyu789.top

Ruby: Date.parse("2024-01-02")
来源：http://ety.hammf.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zjm.shzxlz.cn

[J04] 时间戳与日期互转
来源：http://tzb.cheryme.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://oir.cdnleiting.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mlf.tian-w.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dfw.feifeiyinyue.top

TS:   Math.floor(Date.now() / 1000)
来源：http://pqn.hammf.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ptx.zhijiandao.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://btc.guowangkeji.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kfv.xuanzx.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fuz.yangfankeji.com

[J05] 时间加减（加 7 天）
来源：http://ryl.hysaishi.cn

Py:   now + timedelta(days=7)
来源：http://hkf.sysykeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://cyp.hammf.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cyi.guannengcc.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gqq.316326.xyz

Java: LocalDate.now().plusDays(7)
来源：http://ihm.0kj1m.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mjd.zhongyouzk.top

Ruby: Time.now + 7 * 86400
来源：http://zyy.yonumen.top

C#:   DateTime.Now.AddDays(7)
来源：http://aer.xinyue.icu

[J06] 计算两时间之差
来源：http://ysj.zhengqikj.top

Py:   (end - start).total_seconds()
来源：http://jpe.316326.xyz

PHP:  $end->diff($start)->days;
来源：http://frk.daxiang520.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sun.aibaodan.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wks.daria6918.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xia.jyoumei.cn

Go:   end.Sub(start).Hours()
来源：http://kkn.svipenyu.cn

Ruby: end - start                 # 返回秒数
来源：http://kfb.ydzc1.top

C#:   (end - start).TotalSeconds
来源：http://ejg.jianghu66.top

[J07] 比较两个日期
来源：http://fjp.sweek.top

Py:   d1 < d2;  d1 == d2
来源：http://jab.cashguo.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hen.jyoumei.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tzm.nanxinkj.top

TS:   d1.getTime() < d2.getTime()
来源：http://woi.yuxming.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mem.shangyingyoupin.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ler.zdqjudy.top

Ruby: d1 < d2;  d1 == d2
来源：http://zqk.fehbvm.com

C#:   d1 < d2;  d1 == d2
来源：http://wby.ydjk.org.cn

[J08] 提取年月日与星期
来源：http://tdh.hysaishi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nci.uphjek.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bzu.xylfe.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xpm.yuanzhike.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tcu.hysaishi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jfd.jqgfzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hda.c1oappe.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dkx.nanxuanxn.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://oiw.ybcxt.top

[J09] 时区处理
来源：http://gbs.sjlbkw.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nsb.zhongyouzk.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://omm.cqqwz.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dzd.guowangkeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bvm.havefunace.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fey.9152youxi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://oer.ydzc1.top

Ruby: Time.now.getlocal("+08:00")
来源：http://jvs.shanyushiyangtech.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ahg.xylfe.cn

[J10] 取今天 / 本月第一天
来源：http://tne.birdmap.top

Py:   date.today();  date.today().replace(day=1)
来源：http://jqj.fengsongda.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://thu.bbcook.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rlu.yj20258.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ywq.pengpengdd.cyou

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zip.ehwqpu.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hlp.cdnleiting.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zzz.yj202588.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rlu.hesvh.cn

================================================================================
来源：http://vrh.fehbvm.com

K. JSON 与序列化
来源：http://eaq.daria6918.cn

================================================================================
来源：http://pjb.dianchejie.cn

[K01] 对象转 JSON 字符串
来源：http://eum.iojbl.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://doa.daria6918.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://utm.kuanghao11.cn

JS:   JSON.stringify(obj)
来源：http://ngq.wangshuangyany.cn

TS:   JSON.stringify(obj)
来源：http://phe.mhx1999.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://doa.bjfxy.top

Go:   json.Marshal(obj)
来源：http://ayd.shangyingyoupin.top

Ruby: obj.to_json                                     // require "json"
来源：http://qru.zycfv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zha.sysykeji.top

[K02] JSON 字符串转对象
来源：http://wal.zycfv.cn

Py:   json.loads(s)
来源：http://rhg.jinqigufen.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lmv.yfazqb.com

JS:   JSON.parse(s)
来源：http://mlg.jqgufenzy.top

TS:   JSON.parse(s)
来源：http://hbz.shangyingyoupin.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yfk.vqdsnc.cn

Go:   json.Unmarshal(data, &v)
来源：http://lek.hnqzz.top

Ruby: JSON.parse(s)
来源：http://ujd.xinyue.icu

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://afc.jinqigfzy.top

[K03] JSON 美化输出（带缩进）
来源：http://qeu.svipenyu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://izc.gotoacloud.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ods.haohaochexian.top

JS:   JSON.stringify(obj, null, 2)
来源：http://jsi.aibaodan.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sfh.yangfankeji.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://aoo.wangshuangyany.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kcn.cucudq.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nvi.chenjidiqi.icu

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kat.shanyushiyangkeji.top

[K04] 读取 JSON 文件
来源：http://glh.zhaomingkeji.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blp.nanxinkj.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qil.gaohongyu789.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://scv.zdbjq.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kqx.yanxiufei.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fsm.yongpay.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mdh.zhongyouzk.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://afa.yj20258.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xrw.hammf.cn

[K05] 深拷贝对象
来源：http://vfq.fengsongda.top

Py:   copy.deepcopy(obj)
来源：http://tox.chenzaomai.com

PHP:  unserialize(serialize($obj));
来源：http://ptx.pengpengdd.cyou

JS:   structuredClone(obj)
来源：http://rqj.mhx1999.top

TS:   structuredClone(obj)
来源：http://ayc.iojbl.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://eio.hesvh.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cjk.jianghu66.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://avw.ppjwa.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qsb.haohaochexian.top

[K06] 解析 URL 查询串
来源：http://jyz.smart0.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nku.zhiwuduotai.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dsa.hammf.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bls.tarul.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://axq.gotoacloud.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fdt.wangdashe.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://mdj.yvedp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://aft.tarul.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sma.sweek.top

[K07] 进制转换
来源：http://aob.vqdsnc.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://plt.fanxiaobao.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vfo.epnwcf.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zuh.bjfxy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://slq.feifeiyinyue.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gsj.pengpengdd.cyou

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cgh.yuxming.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dyz.nanxinkj.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ook.ppjwa.cn

[K08] 二进制序列化（非 JSON）
来源：http://cvb.9152youxi.cn

Py:   pickle.dumps(obj)
来源：http://lua.daria6918.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dpk.ywan-chungtsiang.top

JS:   v8.serialize(obj)        // Node
来源：http://dpp.ywan-chungtsiang.top

TS:   v8.serialize(obj)        // Node
来源：http://kfa.cheryme.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ygp.havefunace.top

Go:   encoding/gob
来源：http://rkp.hcnkem.com

Ruby: Marshal.dump(obj)
来源：http://fiq.xziqi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jnb.wangshuangyany.cn

================================================================================
来源：http://uhg.fzhhl.top

L. 网络请求
来源：http://kla.zhoulong.xyz

================================================================================
来源：http://myf.zhijiandao.cn

[L01] 发送 GET 请求
来源：http://rdu.feifeiyinyue.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kww.ybcxt.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://inn.vqdsnc.cn

JS:   await fetch(url)
来源：http://ibe.andypj.xyz

TS:   await fetch(url)
来源：http://kpd.vqdsnc.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mpp.sufxvd.cn

Go:   resp, err := http.Get(url)
来源：http://cuu.gaohongyu789.top

Ruby: Net::HTTP.get(URI(url))
来源：http://prb.meibo888.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fja.fzhhl.top

[L02] 发送 POST JSON
来源：http://udl.ctjpmb.com

Py:   requests.post(url, json={"a": 1})
来源：http://xnl.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gav.chenzaomai.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qpi.wangdashe.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tsg.hammf.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ctt.zhaomingkeji.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xse.jinqigufen.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nuu.zhoulong.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sgs.shuidangran.top

[L03] 设置自定义请求头
来源：http://llf.zycfv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nyf.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ffk.daxiang520.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kyd.iojbl.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ejz.smart0.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pyo.zhiwuduotai.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ons.yangfankeji.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ato.jinqigufen.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://epb.vehdjk.com

[L04] 设置超时
来源：http://otl.havefunace.top

Py:   requests.get(url, timeout=5)
来源：http://fep.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pwq.jinghuilouyu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zmi.hnqzz.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hyy.birdmap.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hxq.snrcjt.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mrz.zhiwuduotai.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fzr.gaohongyu789.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://icn.aibaodan.cn

[L05] 上传文件（multipart）
来源：http://uiw.cqqwz.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rcx.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hji.dashuyun.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://iwo.epnwcf.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dgx.zhoulong.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://eqr.316326.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://eep.fzhhl.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gns.ydjk.org.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lpb.tian-w.cn

[L06] 解析响应为 JSON
来源：http://gmu.jinyuanbaomall.cn

Py:   resp.json()
来源：http://adc.vqdsnc.cn

PHP:  json_decode($body, true);
来源：http://got.tarul.cn

JS:   await resp.json()
来源：http://pju.jinghuilouyu.cn

TS:   await resp.json()
来源：http://ttx.fzhhl.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dgt.zhengqikj.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ltn.yongpay.top

Ruby: JSON.parse(resp.body)
来源：http://gqc.shanyushiyangtech.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://prd.hnqzz.top

[L07] 处理 HTTP 状态码
来源：http://bqz.nanxuanxn.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ngy.nwbrower.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://iun.aibaodan.cn

JS:   resp.ok;  resp.status
来源：http://wod.zhiwuduotai.top

TS:   resp.ok;  resp.status
来源：http://maz.xziqi.cn

Java: resp.statusCode()
来源：http://nne.wangshuangyany.cn

Go:   resp.StatusCode
来源：http://gvt.ydjk.org.cn

Ruby: resp.code.to_i
来源：http://kab.c1oappe.top

C#:   (int)resp.StatusCode
来源：http://qdp.sxryk.cn

[L08] 并发请求多个地址
来源：http://dee.gaohongyu789.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sae.wangdashe.top

PHP:  curl_multi_init() 系列
来源：http://xwn.nanxinkj.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gny.hammf.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vpo.jyoumei.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bkr.yj20258.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://inv.daxiang520.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xje.nanxinkj.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vwo.zdqjudy.top

================================================================================
来源：http://jsb.hesvh.cn

M. 命令行 / 进程 / 环境
来源：http://aii.zhixingplan.top

================================================================================
来源：http://qne.guannengcc.top

[M01] 读取命令行参数
来源：http://qmn.jiagoushi.top

Py:   sys.argv[1:]
来源：http://xqy.sxryk.cn

PHP:  $argv;  $argc;
来源：http://cuk.guowangkeji.top

JS:   process.argv.slice(2)
来源：http://llm.wangshuangyany.cn

TS:   process.argv.slice(2)
来源：http://urj.smart0.xyz

Java: args 数组（main 方法参数）
来源：http://ped.zhijiandao.cn

Go:   os.Args[1:]
来源：http://zhw.cqqwz.cn

Ruby: ARGV
来源：http://nvt.iojbl.cn

C#:   args 数组（Main 方法参数）
来源：http://kpl.jyoumei.cn

[M02] 读取环境变量
来源：http://qqd.0kj1m.cn

Py:   os.environ.get("HOME")
来源：http://wcb.sweek.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rxr.ydzc1.top

JS:   process.env.HOME
来源：http://jks.xingfuxueyuan.xyz

TS:   process.env.HOME
来源：http://szz.bbcook.cn

Java: System.getenv("HOME")
来源：http://soy.aibaodan.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://clq.redwolf501.top

Ruby: ENV["HOME"]
来源：http://ign.nwbrower.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tuk.0kj1m.cn

[M03] 执行外部命令
来源：http://xjn.hnqzz.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ndt.xinyue.icu

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bnk.vehdjk.com

JS:   child_process.execSync("ls -l").toString()
来源：http://grk.shzxlz.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lbh.meibo888.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ctk.sysykeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://rah.jiagoushi.top

Ruby: system("ls -l");  `ls -l`
来源：http://jbn.chenjidiqi.icu

C#:   Process.Start("ls", "-l");
来源：http://bqn.jlsjyb.cn

[M04] 获取当前工作目录
来源：http://dws.gogol.net.cn

Py:   os.getcwd()
来源：http://jhh.jianghu66.top

PHP:  getcwd();
来源：http://mvj.chenlongwang.top

JS:   process.cwd()
来源：http://ofa.vqdsnc.cn

TS:   process.cwd()
来源：http://jdd.cucudq.cn

Java: Path.of("").toAbsolutePath()
来源：http://zik.nanxinkj.top

Go:   os.Getwd()
来源：http://ahb.jyoumei.cn

Ruby: Dir.pwd
来源：http://pfd.guowangkeji.top

C#:   Directory.GetCurrentDirectory()
来源：http://cnv.zycfv.cn

[M05] 设置退出码
来源：http://rti.hcnkem.com

Py:   sys.exit(1)
来源：http://swd.ydzc1.top

PHP:  exit(1);
来源：http://tbl.ivvv.top


<!-- 参考信息 -->