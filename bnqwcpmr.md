代发 wailian999

Ruby: s.scan(/error/i)
来源：http://xpd.shanyushiyangtech.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://afd.quarkkingdee.top

[I08] 贪婪与非贪婪匹配
来源：http://fkr.zhengqikj.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wxw.hnqzz.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zkx.kuanghao11.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gqu.nwbrower.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://aai.xingfuxueyuan.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://sor.zdqjudy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://scr.jianghu66.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qgb.hesvh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blp.jinqigfzy.top

================================================================================
来源：http://pmj.ybcxt.top

J. 日期与时间
来源：http://roc.xuanzx.com

================================================================================
来源：http://mly.shanyushiyangkeji.top

[J01] 获取当前时间
来源：http://sji.ydjk.org.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fss.sjlbkw.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cgk.yuxming.cn

JS:   new Date();  Date.now()
来源：http://cyt.chenjidiqi.icu

TS:   new Date();  Date.now()
来源：http://zyo.fktsv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://uki.tian-w.cn

Go:   time.Now()
来源：http://vsm.pycfn.com

Ruby: Time.now
来源：http://hcs.cqqwz.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gxl.gaohongyu789.top

[J02] 格式化输出
来源：http://xxr.xuanzx.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://thm.bbcook.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nlz.fehbvm.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://int.zycfv.cn

TS:   d.toISOString()
来源：http://npo.cheryme.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jop.hcnkem.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://krh.yuxming.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gge.yueranfly.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nor.fanxiaobao.xyz

[J03] 字符串解析为日期
来源：http://mqb.jiagoushi.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nlc.wangdashe.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pjm.zhiwuduotai.top

JS:   new Date("2024-01-02")
来源：http://zpb.zhiwuduotai.top

TS:   new Date("2024-01-02")
来源：http://fjx.hysaishi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dlm.yfazqb.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ian.jianghu66.top

Ruby: Date.parse("2024-01-02")
来源：http://xnn.andypj.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gel.cdnleiting.top

[J04] 时间戳与日期互转
来源：http://jbw.daxiang520.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jut.yfazqb.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ixq.yfazqb.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wtz.hesvh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://nuc.yangfankeji.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jiz.zhixingplan.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://psi.zhixingplan.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vwo.316326.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vnu.yueranfly.top

[J05] 时间加减（加 7 天）
来源：http://afu.bbcook.cn

Py:   now + timedelta(days=7)
来源：http://mhv.zhijiandao.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bst.xuanzx.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fow.shuidangran.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zjy.ctjpmb.com

Java: LocalDate.now().plusDays(7)
来源：http://lkp.iojbl.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lcf.zdqjudy.top

Ruby: Time.now + 7 * 86400
来源：http://xrg.yuanzhike.top

C#:   DateTime.Now.AddDays(7)
来源：http://prh.zhaomingkeji.xyz

[J06] 计算两时间之差
来源：http://kmz.xingfuxueyuan.xyz

Py:   (end - start).total_seconds()
来源：http://uma.fengsongda.top

PHP:  $end->diff($start)->days;
来源：http://cum.cheryme.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nbn.gogol.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://guc.wangshuangyany.cn

Java: Duration.between(start, end).toSeconds()
来源：http://esl.tarul.cn

Go:   end.Sub(start).Hours()
来源：http://nnr.hfpthk.cn

Ruby: end - start                 # 返回秒数
来源：http://ftt.shanyushiyangkeji.top

C#:   (end - start).TotalSeconds
来源：http://fpc.ppjwa.cn

[J07] 比较两个日期
来源：http://eok.mhx1999.top

Py:   d1 < d2;  d1 == d2
来源：http://dkl.havefunace.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gpm.nanxuanxn.top

JS:   d1.getTime() < d2.getTime()
来源：http://ivz.feifeiyinyue.top

TS:   d1.getTime() < d2.getTime()
来源：http://wmx.zhixingplan.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ekq.yfazqb.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://skl.guowangkeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://yfm.haohaochexian.top

C#:   d1 < d2;  d1 == d2
来源：http://nrm.gogol.net.cn

[J08] 提取年月日与星期
来源：http://ddt.sysykeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fco.chenzaomai.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vhs.xuanzx.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qei.yj20258888.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://roh.tanke756.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wdn.bjfxy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kwn.mhx1999.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://eeh.guowangkeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qyb.fehbvm.com

[J09] 时区处理
来源：http://aey.zhixingplan.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ffw.vehdjk.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nrf.epnwcf.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gkx.aibaodan.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cga.yonumen.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tni.fanxiaobao.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gtd.zhiwuduotai.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ixv.hfpthk.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uni.jqgufenzy.top

[J10] 取今天 / 本月第一天
来源：http://ypk.xinyue.icu

Py:   date.today();  date.today().replace(day=1)
来源：http://yht.zhoulong.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://akq.yj202588.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pwk.chenjidiqi.icu

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://oot.xuanzx.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bol.shzxlz.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tnd.hywenlv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vld.shuidangran.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://meb.quarkkingdee.top

================================================================================
来源：http://hmf.sufxvd.cn

K. JSON 与序列化
来源：http://arl.xylfe.cn

================================================================================
来源：http://szj.jinghuilouyu.cn

[K01] 对象转 JSON 字符串
来源：http://gdc.shangyingyoupin.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mfz.wangshuangyany.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://awg.jianghu66.top

JS:   JSON.stringify(obj)
来源：http://fxb.snrcjt.cn

TS:   JSON.stringify(obj)
来源：http://wup.zhiwuduotai.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://eij.316326.xyz

Go:   json.Marshal(obj)
来源：http://dvq.fehbvm.com

Ruby: obj.to_json                                     // require "json"
来源：http://eye.aibaodan.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vtg.hysaishi.cn

[K02] JSON 字符串转对象
来源：http://clp.sjlbkw.cn

Py:   json.loads(s)
来源：http://hbf.52xcode.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ppl.bjfxy.top

JS:   JSON.parse(s)
来源：http://lhh.xylfe.cn

TS:   JSON.parse(s)
来源：http://xee.52xcode.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ijl.52xcode.cn

Go:   json.Unmarshal(data, &v)
来源：http://dkx.sxryk.cn

Ruby: JSON.parse(s)
来源：http://eky.yonumen.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://chb.jinqigufen.top

[K03] JSON 美化输出（带缩进）
来源：http://whv.hnxiangtu.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wgf.hammf.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://diq.chenjidiqi.icu

JS:   JSON.stringify(obj, null, 2)
来源：http://tvl.xziqi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ybp.yonumen.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://exs.bbcook.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gqf.guannengcc.top

Ruby: JSON.pretty_generate(obj)
来源：http://puv.0kj1m.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cri.svipenyu.cn

[K04] 读取 JSON 文件
来源：http://xen.jqgfzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ztl.haohaochexian.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ydh.sweek.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yif.nanxinkj.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bhz.shangyingyoupin.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zmi.gogol.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jjo.quarkkingdee.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://kau.daxiang520.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wlj.hysaishi.cn

[K05] 深拷贝对象
来源：http://bdv.fehbvm.com

Py:   copy.deepcopy(obj)
来源：http://xeh.quarkkingdee.top

PHP:  unserialize(serialize($obj));
来源：http://oow.ppjwa.cn

JS:   structuredClone(obj)
来源：http://yuw.hesvh.cn

TS:   structuredClone(obj)
来源：http://gvl.c1oappe.top

Java: // 手写拷贝构造，或序列化往返
来源：http://tpg.nwbrower.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gtq.hnqzz.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bty.chenjidiqi.icu

C#:   // 序列化往返，或自定义 Clone
来源：http://jkt.jyoumei.cn

[K06] 解析 URL 查询串
来源：http://vcg.jinqigfzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://iyo.zhijiandao.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fee.ivvv.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hhu.cqqwz.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bxe.xylfe.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bct.gzhubu.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://avs.smart0.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bdb.jyoumei.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cpo.vqdsnc.cn

[K07] 进制转换
来源：http://pzi.sjlbkw.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vhc.sxryk.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ulo.yanxiufei.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lzd.cheryme.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lfd.cqqwz.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jxi.zhijiandao.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sai.ybcxt.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cyl.birdmap.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blk.fanxiaobao.xyz

[K08] 二进制序列化（非 JSON）
来源：http://jlx.sweek.top

Py:   pickle.dumps(obj)
来源：http://npr.sxryk.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://uiw.hywenlv.cn

JS:   v8.serialize(obj)        // Node
来源：http://qhm.aizwys.cn

TS:   v8.serialize(obj)        // Node
来源：http://zxy.xuanzx.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://khj.cdnleiting.top

Go:   encoding/gob
来源：http://msp.sysykeji.top

Ruby: Marshal.dump(obj)
来源：http://iun.yj20258888.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vrk.uphjek.com

================================================================================
来源：http://ogm.gogol.net.cn

L. 网络请求
来源：http://nbx.wangshuangyany.cn

================================================================================
来源：http://gxh.bbcook.cn

[L01] 发送 GET 请求
来源：http://lro.fehbvm.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://opj.fengsongda.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uhv.guannengcc.top

JS:   await fetch(url)
来源：http://eto.fehbvm.com

TS:   await fetch(url)
来源：http://ysk.wangdashe.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://scu.guannengcc.top

Go:   resp, err := http.Get(url)
来源：http://hhz.zdbjq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pwo.feifeiyinyue.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gbw.shanyushiyangkeji.top

[L02] 发送 POST JSON
来源：http://lth.fengsongda.top

Py:   requests.post(url, json={"a": 1})
来源：http://ydn.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://thc.cheryme.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://upj.yonumen.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xsl.ybcxt.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gln.yuanzhike.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://glb.yueranfly.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ugn.nanxinkj.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jqo.jlsjyb.cn

[L03] 设置自定义请求头
来源：http://ctu.jinyuanbaomall.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fxo.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nrc.pycfn.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gig.fzhhl.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cdt.zdqjudy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tgl.jinghuilouyu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://msq.gzhubu.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fug.vqdsnc.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vni.shuidangran.top

[L04] 设置超时
来源：http://rxu.cheryme.top

Py:   requests.get(url, timeout=5)
来源：http://jhd.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ixg.zhoulong.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gdr.vehdjk.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://plo.hnxiangtu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qib.tarul.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://imr.xziqi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wjw.hfpthk.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cic.zhaomingkeji.xyz

[L05] 上传文件（multipart）
来源：http://rqg.vqdsnc.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://prh.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ybd.jiagoushi.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ymw.chenlongwang.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://drt.zhiwuduotai.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pck.yueranfly.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ygz.tian-w.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xzy.xylfe.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qxr.jqgufenzy.top

[L06] 解析响应为 JSON
来源：http://oaa.yfazqb.com

Py:   resp.json()
来源：http://pkp.dianchejie.cn

PHP:  json_decode($body, true);
来源：http://dxx.havefunace.top

JS:   await resp.json()
来源：http://jci.zhengqikj.top

TS:   await resp.json()
来源：http://ngu.birdmap.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bgw.havefunace.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rab.shanyushiyangtech.top

Ruby: JSON.parse(resp.body)
来源：http://ria.cashguo.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://okt.smart0.xyz

[L07] 处理 HTTP 状态码
来源：http://evt.uphjek.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bzt.52xcode.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gtv.guannengcc.top

JS:   resp.ok;  resp.status
来源：http://kls.zhengqikj.top

TS:   resp.ok;  resp.status
来源：http://nwd.sjlbkw.cn

Java: resp.statusCode()
来源：http://pdr.aizwys.cn

Go:   resp.StatusCode
来源：http://ebo.fktsv.cn

Ruby: resp.code.to_i
来源：http://oac.zhixingplan.top

C#:   (int)resp.StatusCode
来源：http://qli.wangshuangyany.cn

[L08] 并发请求多个地址
来源：http://ofw.gzhubu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yiz.cqqwz.cn

PHP:  curl_multi_init() 系列
来源：http://aru.wangdashe.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mxu.yj202588.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lmx.zhixingplan.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ouw.chenlongwang.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xdy.dashuyun.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ifm.hesvh.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wcn.hesvh.cn

================================================================================
来源：http://vqj.vqdsnc.cn

M. 命令行 / 进程 / 环境
来源：http://mag.shzxlz.cn

================================================================================
来源：http://uzd.fzhhl.top

[M01] 读取命令行参数
来源：http://ubg.shuidangran.top

Py:   sys.argv[1:]
来源：http://hvx.ydzc1.top

PHP:  $argv;  $argc;
来源：http://zrw.jinghuilouyu.cn

JS:   process.argv.slice(2)
来源：http://hqa.tianlin.xyz

TS:   process.argv.slice(2)
来源：http://yyp.chenjidiqi.icu

Java: args 数组（main 方法参数）
来源：http://lss.ydjk.org.cn

Go:   os.Args[1:]
来源：http://vvd.shzxlz.cn

Ruby: ARGV
来源：http://glj.hysaishi.cn

C#:   args 数组（Main 方法参数）
来源：http://fbv.wangshuangyany.cn

[M02] 读取环境变量
来源：http://ohk.wangdashe.top

Py:   os.environ.get("HOME")
来源：http://bqz.tianlin.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://utk.daria6918.cn

JS:   process.env.HOME
来源：http://fmj.yj20258888.top

TS:   process.env.HOME
来源：http://ewl.gaohongyu789.top

Java: System.getenv("HOME")
来源：http://bea.tanke756.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vdj.zhijiandao.cn

Ruby: ENV["HOME"]
来源：http://ugr.yonumen.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://acl.jianghu66.top

[M03] 执行外部命令
来源：http://eoo.ehwqpu.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://udz.xylfe.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ngq.shanyushiyangtech.top

JS:   child_process.execSync("ls -l").toString()
来源：http://fhe.ivvv.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ely.aizwys.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rnn.yuanzhike.top

Go:   exec.Command("ls", "-l").Output()
来源：http://drj.jqgfzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://gsp.jinghuilouyu.cn

C#:   Process.Start("ls", "-l");
来源：http://bhe.epnwcf.com

[M04] 获取当前工作目录
来源：http://ixq.zhoulong.xyz

Py:   os.getcwd()
来源：http://msy.zhoulong.xyz

PHP:  getcwd();
来源：http://ila.birdmap.top

JS:   process.cwd()
来源：http://dsl.zhiwuduotai.top

TS:   process.cwd()
来源：http://tor.sufxvd.cn

Java: Path.of("").toAbsolutePath()
来源：http://jir.hnqzz.top

Go:   os.Getwd()
来源：http://pjo.chenzaomai.com

Ruby: Dir.pwd
来源：http://goo.zhongyouzk.top

C#:   Directory.GetCurrentDirectory()
来源：http://vep.xuanzx.com

[M05] 设置退出码
来源：http://bto.tanke756.top

Py:   sys.exit(1)
来源：http://oit.chenlongwang.top

PHP:  exit(1);
来源：http://xgt.cqqwz.cn

JS:   process.exit(1)
来源：http://nyu.ybcxt.top

TS:   process.exit(1)
来源：http://xyl.jinyuanbaomall.cn

Java: System.exit(1)
来源：http://ibj.yj202588.top

Go:   os.Exit(1)
来源：http://bvp.hnxiangtu.top


<!-- 参考信息 -->