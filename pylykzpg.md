代发 wailian999

Ruby: s.scan(/error/i)
来源：http://fky.yvedp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dzc.xuetiantiany.cn

[I08] 贪婪与非贪婪匹配
来源：http://iwp.ywan-chungtsiang.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kxt.yueranfly.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jvr.vehdjk.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nuz.haohaochexian.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sor.jinyuanbaomall.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lgc.jinqigfzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kzg.dianchejie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zec.zhoulong.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xiv.ivvv.top

================================================================================
来源：http://dpa.ctjpmb.com

J. 日期与时间
来源：http://gpu.jinghuilouyu.cn

================================================================================
来源：http://rdb.nanxinkj.top

[J01] 获取当前时间
来源：http://zru.nwbrower.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://dxo.316326.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wlv.ehwqpu.com

JS:   new Date();  Date.now()
来源：http://gda.jinqigufen.top

TS:   new Date();  Date.now()
来源：http://yji.gotoacloud.top

Java: LocalDateTime.now();  Instant.now()
来源：http://nos.hywenlv.cn

Go:   time.Now()
来源：http://tcu.quarkkingdee.top

Ruby: Time.now
来源：http://wxl.cdnleiting.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qmo.aizwys.cn

[J02] 格式化输出
来源：http://spf.bjfxy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://frh.zhijiandao.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ply.iojbl.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://siy.fzhhl.top

TS:   d.toISOString()
来源：http://ygb.tanke756.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://urx.jqgufenzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://duc.fanxiaobao.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ouw.ydzc1.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://udz.xziqi.cn

[J03] 字符串解析为日期
来源：http://ddk.zycfv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lzi.gaohongyu789.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bmb.9152youxi.cn

JS:   new Date("2024-01-02")
来源：http://lxv.cashguo.top

TS:   new Date("2024-01-02")
来源：http://wza.svipenyu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://nlz.aizwys.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xmu.hongshengwenyu.top

Ruby: Date.parse("2024-01-02")
来源：http://pbh.havefunace.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dkn.redwolf501.top

[J04] 时间戳与日期互转
来源：http://ixn.gaohongyu789.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xkq.hfpthk.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wdj.fktsv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://urh.hnxiangtu.top

TS:   Math.floor(Date.now() / 1000)
来源：http://nfu.hesvh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nar.ydzc1.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xvx.fktsv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lsu.cucudq.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rxc.snrcjt.cn

[J05] 时间加减（加 7 天）
来源：http://ghc.svipenyu.cn

Py:   now + timedelta(days=7)
来源：http://vts.xziqi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://byh.fanxiaobao.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://scn.xuetiantiany.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rth.shangyingyoupin.top

Java: LocalDate.now().plusDays(7)
来源：http://utr.jinghuilouyu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ycf.yangfankeji.com

Ruby: Time.now + 7 * 86400
来源：http://ugu.wangshuangyany.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rtt.ppjwa.cn

[J06] 计算两时间之差
来源：http://icd.ywan-chungtsiang.top

Py:   (end - start).total_seconds()
来源：http://pre.hywenlv.cn

PHP:  $end->diff($start)->days;
来源：http://dge.jinyuanbaomall.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uev.tianlin.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lrc.aizwys.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jnl.tanke756.top

Go:   end.Sub(start).Hours()
来源：http://xci.shanyushiyangkeji.top

Ruby: end - start                 # 返回秒数
来源：http://foz.tianlin.xyz

C#:   (end - start).TotalSeconds
来源：http://mbf.fehbvm.com

[J07] 比较两个日期
来源：http://oiy.shanyushiyangkeji.top

Py:   d1 < d2;  d1 == d2
来源：http://rne.nanxinkj.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wdq.52xcode.cn

JS:   d1.getTime() < d2.getTime()
来源：http://pcm.yfazqb.com

TS:   d1.getTime() < d2.getTime()
来源：http://lwb.zdqjudy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ifl.snrcjt.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xki.jiagoushi.top

Ruby: d1 < d2;  d1 == d2
来源：http://wwk.yueranfly.top

C#:   d1 < d2;  d1 == d2
来源：http://ofz.ybcxt.top

[J08] 提取年月日与星期
来源：http://lqg.yongpay.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nsw.birdmap.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hxt.pycfn.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rte.zdqjudy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://byb.wangdashe.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ufp.zhaomingkeji.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bvu.ehwqpu.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dvi.zhixingplan.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://upa.hnqzz.top

[J09] 时区处理
来源：http://dno.gaohongyu789.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dwc.yvedp.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tts.ivvv.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sjq.0kj1m.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wcb.sweek.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tuf.hfpthk.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vtx.pengpengdd.cyou

Ruby: Time.now.getlocal("+08:00")
来源：http://saa.zhongyouzk.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://puy.yj20258.top

[J10] 取今天 / 本月第一天
来源：http://qfm.fanxiaobao.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://lui.birdmap.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zgz.yj202588.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yjk.yanxiufei.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iac.sxryk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rvc.nanxuanxn.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ywp.shuidangran.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fgc.meibo888.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rqp.ydzc1.top

================================================================================
来源：http://yxu.epnwcf.com

K. JSON 与序列化
来源：http://gyl.chenjidiqi.icu

================================================================================
来源：http://gqp.chenlongwang.top

[K01] 对象转 JSON 字符串
来源：http://alx.pycfn.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yof.zdbjq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hdm.cashguo.top

JS:   JSON.stringify(obj)
来源：http://qti.ydzc1.top

TS:   JSON.stringify(obj)
来源：http://oew.guowangkeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hef.xziqi.cn

Go:   json.Marshal(obj)
来源：http://uvo.zdbjq.cn

Ruby: obj.to_json                                     // require "json"
来源：http://iea.xylfe.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bhd.ivvv.top

[K02] JSON 字符串转对象
来源：http://crk.xuetiantiany.cn

Py:   json.loads(s)
来源：http://tjo.uphjek.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://frg.tianlin.xyz

JS:   JSON.parse(s)
来源：http://byn.zycfv.cn

TS:   JSON.parse(s)
来源：http://onr.vqdsnc.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gpi.sjlbkw.cn

Go:   json.Unmarshal(data, &v)
来源：http://uek.dianchejie.cn

Ruby: JSON.parse(s)
来源：http://tbu.zycfv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hth.guannengcc.top

[K03] JSON 美化输出（带缩进）
来源：http://ygm.zycfv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qmq.ywan-chungtsiang.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ssg.yonumen.top

JS:   JSON.stringify(obj, null, 2)
来源：http://rbq.fzhhl.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wdt.tianlin.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://anw.uphjek.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gha.andypj.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://joa.svipenyu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gva.dianchejie.cn

[K04] 读取 JSON 文件
来源：http://mtm.daria6918.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bfq.andypj.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kwj.gogol.net.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rlp.hfpthk.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xnb.jinyuanbaomall.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cde.ppjwa.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://usx.mhx1999.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://vth.hongshengwenyu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://siw.xylfe.cn

[K05] 深拷贝对象
来源：http://uzi.zdqjudy.top

Py:   copy.deepcopy(obj)
来源：http://mla.gzhubu.top

PHP:  unserialize(serialize($obj));
来源：http://ybf.jlsjyb.cn

JS:   structuredClone(obj)
来源：http://ayz.ctjpmb.com

TS:   structuredClone(obj)
来源：http://epo.hcnkem.com

Java: // 手写拷贝构造，或序列化往返
来源：http://hlr.yfazqb.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hze.xylfe.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://urg.pycfn.com

C#:   // 序列化往返，或自定义 Clone
来源：http://dhg.9152youxi.cn

[K06] 解析 URL 查询串
来源：http://giw.yonumen.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://myl.zhixingplan.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vbq.svipenyu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fem.yongpay.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jia.shanyushiyangtech.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xoz.ivvv.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://lhp.yanxiufei.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://odn.xuetiantiany.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rpx.uphjek.com

[K07] 进制转换
来源：http://btw.guowangkeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bbp.sjlbkw.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lxd.ydjk.org.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mrn.zhongyouzk.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jck.52xcode.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dtn.bjfxy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nsb.wangshuangyany.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yvf.yfazqb.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hgw.zdqjudy.top

[K08] 二进制序列化（非 JSON）
来源：http://bpy.wangdashe.top

Py:   pickle.dumps(obj)
来源：http://xyn.shangyingyoupin.top

PHP:  serialize($obj);  unserialize($s);
来源：http://cdy.ctjpmb.com

JS:   v8.serialize(obj)        // Node
来源：http://zsq.smart0.xyz

TS:   v8.serialize(obj)        // Node
来源：http://tom.zhixingplan.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ufw.aizwys.cn

Go:   encoding/gob
来源：http://jnz.daria6918.cn

Ruby: Marshal.dump(obj)
来源：http://uoh.zhijiandao.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mzv.vehdjk.com

================================================================================
来源：http://usj.zhengqikj.top

L. 网络请求
来源：http://pax.zhengqikj.top

================================================================================
来源：http://xbd.nwbrower.top

[L01] 发送 GET 请求
来源：http://hne.jlsjyb.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nls.xinyue.icu

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ysq.yj20258888.top

JS:   await fetch(url)
来源：http://afu.gogol.net.cn

TS:   await fetch(url)
来源：http://tsa.0kj1m.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mox.yuanzhike.top

Go:   resp, err := http.Get(url)
来源：http://mjd.xziqi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dba.gogol.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mzm.shangyingyoupin.top

[L02] 发送 POST JSON
来源：http://mcb.havefunace.top

Py:   requests.post(url, json={"a": 1})
来源：http://dgr.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://opa.0kj1m.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://maq.chenjidiqi.icu

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mdu.daxiang520.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fzu.gzhubu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://koh.cashguo.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jpt.jinqigufen.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yqc.yueranfly.top

[L03] 设置自定义请求头
来源：http://aua.ydjk.org.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vrv.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sbx.xuanzx.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lgd.yj202588.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cjt.zdbjq.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kko.shanyushiyangtech.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ueo.jianghu66.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vse.ctjpmb.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yyr.haohaochexian.top

[L04] 设置超时
来源：http://laz.wangdashe.top

Py:   requests.get(url, timeout=5)
来源：http://aph.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tob.chenzaomai.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yqb.jinqigufen.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wey.nanxuanxn.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fgs.yvedp.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://axh.yj20258.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uyu.fanxiaobao.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wka.zhongyouzk.top

[L05] 上传文件（multipart）
来源：http://tlh.feifeiyinyue.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bcj.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ipi.shanyushiyangtech.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ysl.hammf.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ipg.xingfuxueyuan.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vrv.hfpthk.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dqm.iojbl.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nbp.ctjpmb.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xrf.chenlongwang.top

[L06] 解析响应为 JSON
来源：http://rck.fehbvm.com

Py:   resp.json()
来源：http://fgg.guannengcc.top

PHP:  json_decode($body, true);
来源：http://dxl.zhengqikj.top

JS:   await resp.json()
来源：http://vsp.ydjk.org.cn

TS:   await resp.json()
来源：http://yic.yangfankeji.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wdg.xuanzx.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://goo.yj20258888.top

Ruby: JSON.parse(resp.body)
来源：http://svo.yanxiufei.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://roz.xylfe.cn

[L07] 处理 HTTP 状态码
来源：http://xql.iojbl.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mnu.zhaomingkeji.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ons.ivvv.top

JS:   resp.ok;  resp.status
来源：http://bho.vehdjk.com

TS:   resp.ok;  resp.status
来源：http://vsh.jinghuilouyu.cn

Java: resp.statusCode()
来源：http://wbe.tarul.cn

Go:   resp.StatusCode
来源：http://las.cheryme.top

Ruby: resp.code.to_i
来源：http://hsh.zhongyouzk.top

C#:   (int)resp.StatusCode
来源：http://sbh.sweek.top

[L08] 并发请求多个地址
来源：http://mbu.ctjpmb.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vtx.jinyuanbaomall.cn

PHP:  curl_multi_init() 系列
来源：http://ftg.hysaishi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tls.daria6918.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bjm.gzhubu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nne.fengsongda.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vif.yuanzhike.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xzi.wangshuangyany.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zdu.guowangkeji.top

================================================================================
来源：http://ipx.tian-w.cn

M. 命令行 / 进程 / 环境
来源：http://kqq.9152youxi.cn

================================================================================
来源：http://fhp.jqgfzy.top

[M01] 读取命令行参数
来源：http://bfj.yfazqb.com

Py:   sys.argv[1:]
来源：http://tns.smart0.xyz

PHP:  $argv;  $argc;
来源：http://mht.nanxuanxn.top

JS:   process.argv.slice(2)
来源：http://jyu.cheryme.top

TS:   process.argv.slice(2)
来源：http://ydw.fengsongda.top

Java: args 数组（main 方法参数）
来源：http://int.jqgfzy.top

Go:   os.Args[1:]
来源：http://jaz.meibo888.top

Ruby: ARGV
来源：http://ivg.xuanzx.com

C#:   args 数组（Main 方法参数）
来源：http://mfk.hfpthk.cn

[M02] 读取环境变量
来源：http://nrj.sufxvd.cn

Py:   os.environ.get("HOME")
来源：http://yos.guowangkeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rnu.tarul.cn

JS:   process.env.HOME
来源：http://bil.ybcxt.top

TS:   process.env.HOME
来源：http://enn.yangfankeji.com

Java: System.getenv("HOME")
来源：http://jiq.pycfn.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qbe.yonumen.top

Ruby: ENV["HOME"]
来源：http://bov.redwolf501.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ulz.hnxiangtu.top

[M03] 执行外部命令
来源：http://obf.zhijiandao.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tkc.yj202588.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bfb.cdnleiting.top

JS:   child_process.execSync("ls -l").toString()
来源：http://azd.yj20258888.top

TS:   child_process.execSync("ls -l").toString()
来源：http://itf.316326.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yfa.ppjwa.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://klj.fengsongda.top

Ruby: system("ls -l");  `ls -l`
来源：http://abi.ivvv.top

C#:   Process.Start("ls", "-l");
来源：http://ogt.xinyue.icu

[M04] 获取当前工作目录
来源：http://eah.jyoumei.cn

Py:   os.getcwd()
来源：http://rhi.havefunace.top

PHP:  getcwd();
来源：http://bbc.birdmap.top

JS:   process.cwd()
来源：http://wkp.andypj.xyz

TS:   process.cwd()
来源：http://yzr.yfazqb.com

Java: Path.of("").toAbsolutePath()
来源：http://dnj.shangyingyoupin.top

Go:   os.Getwd()
来源：http://xsn.kuanghao11.cn

Ruby: Dir.pwd
来源：http://bgc.hnxiangtu.top

C#:   Directory.GetCurrentDirectory()
来源：http://ovt.c1oappe.top

[M05] 设置退出码
来源：http://edj.xziqi.cn

Py:   sys.exit(1)
来源：http://wkf.gaohongyu789.top

PHP:  exit(1);
来源：http://ywt.zdbjq.cn

JS:   process.exit(1)
来源：http://cyc.tian-w.cn

TS:   process.exit(1)
来源：http://baq.fehbvm.com

Java: System.exit(1)
来源：http://rfn.andypj.xyz

Go:   os.Exit(1)
来源：http://qcw.svipenyu.cn


<!-- 参考信息 -->