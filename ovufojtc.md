代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bkh.hongshengwenyu.top

TS:   /error/gim
来源：http://ghj.ivvv.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ivl.chenjidiqi.icu

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rqn.vqdsnc.cn

Ruby: s.scan(/error/i)
来源：http://sgd.fehbvm.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hqw.quarkkingdee.top

[I08] 贪婪与非贪婪匹配
来源：http://cgo.316326.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cyb.zdbjq.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kvp.yj20258888.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kiy.mhx1999.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nij.sjlbkw.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vwr.jinghuilouyu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kns.guannengcc.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fnm.zdqjudy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fay.snrcjt.cn

================================================================================
来源：http://jxe.ctjpmb.com

J. 日期与时间
来源：http://fqg.jianghu66.top

================================================================================
来源：http://srl.tanke756.top

[J01] 获取当前时间
来源：http://nkb.jianghu66.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://fkk.fehbvm.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tbp.yuxming.cn

JS:   new Date();  Date.now()
来源：http://lli.guannengcc.top

TS:   new Date();  Date.now()
来源：http://yho.xuetiantiany.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vzj.redwolf501.top

Go:   time.Now()
来源：http://ekw.nanxinkj.top

Ruby: Time.now
来源：http://crp.ybcxt.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ico.yueranfly.top

[J02] 格式化输出
来源：http://pob.yuxming.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rex.zhengqikj.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ebg.yanxiufei.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vgk.dianchejie.cn

TS:   d.toISOString()
来源：http://hlk.mhx1999.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xjq.shangyingyoupin.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://joa.dashuyun.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uqf.nwbrower.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jjl.sufxvd.cn

[J03] 字符串解析为日期
来源：http://eno.chenzaomai.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://oml.hnxiangtu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vck.shanyushiyangkeji.top

JS:   new Date("2024-01-02")
来源：http://thq.cheryme.top

TS:   new Date("2024-01-02")
来源：http://skx.bbcook.cn

Java: LocalDate.parse("2024-01-02")
来源：http://baw.shanyushiyangkeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nxw.sweek.top

Ruby: Date.parse("2024-01-02")
来源：http://oal.svipenyu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ulb.jinqigufen.top

[J04] 时间戳与日期互转
来源：http://bdf.sxryk.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kme.wangshuangyany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://amw.hnqzz.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pbt.0kj1m.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zki.aizwys.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://znf.yuxming.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wky.jqgfzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uxc.fktsv.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gas.yanxiufei.cn

[J05] 时间加减（加 7 天）
来源：http://rnt.jinyuanbaomall.cn

Py:   now + timedelta(days=7)
来源：http://lfv.52xcode.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rmc.ctjpmb.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://phn.guowangkeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qgd.andypj.xyz

Java: LocalDate.now().plusDays(7)
来源：http://gwm.vehdjk.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xwc.zhongyouzk.top

Ruby: Time.now + 7 * 86400
来源：http://iou.daxiang520.top

C#:   DateTime.Now.AddDays(7)
来源：http://whk.zhoulong.xyz

[J06] 计算两时间之差
来源：http://hys.cheryme.top

Py:   (end - start).total_seconds()
来源：http://lnt.iojbl.cn

PHP:  $end->diff($start)->days;
来源：http://nwr.aizwys.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wtm.ywan-chungtsiang.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cwm.chenjidiqi.icu

Java: Duration.between(start, end).toSeconds()
来源：http://yim.zdbjq.cn

Go:   end.Sub(start).Hours()
来源：http://pad.havefunace.top

Ruby: end - start                 # 返回秒数
来源：http://fjh.cashguo.top

C#:   (end - start).TotalSeconds
来源：http://brd.birdmap.top

[J07] 比较两个日期
来源：http://ppe.daria6918.cn

Py:   d1 < d2;  d1 == d2
来源：http://zqm.jqgufenzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://clj.ppjwa.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bvk.epnwcf.com

TS:   d1.getTime() < d2.getTime()
来源：http://kwm.zdqjudy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xsn.yangfankeji.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tto.haohaochexian.top

Ruby: d1 < d2;  d1 == d2
来源：http://ibc.zhijiandao.cn

C#:   d1 < d2;  d1 == d2
来源：http://lut.quarkkingdee.top

[J08] 提取年月日与星期
来源：http://bkj.shangyingyoupin.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rpv.gotoacloud.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dln.birdmap.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://oyf.hammf.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ixe.guowangkeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ljz.zycfv.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ecs.shuidangran.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fsi.yuxming.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gxo.jinqigfzy.top

[J09] 时区处理
来源：http://yvj.daxiang520.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qdn.meibo888.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ped.zdqjudy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eax.shanyushiyangtech.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zma.tian-w.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kvm.gotoacloud.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zsx.sxryk.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vmz.zhengqikj.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bvy.smart0.xyz

[J10] 取今天 / 本月第一天
来源：http://wym.shzxlz.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://aov.zhengqikj.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://twg.daxiang520.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://eaj.jlsjyb.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ffk.fanxiaobao.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tjj.sjlbkw.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fyi.daria6918.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ixm.gogol.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://usa.fengsongda.top

================================================================================
来源：http://xjx.snrcjt.cn

K. JSON 与序列化
来源：http://qtv.vqdsnc.cn

================================================================================
来源：http://dks.guannengcc.top

[K01] 对象转 JSON 字符串
来源：http://vpg.chenzaomai.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://iec.cucudq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yvg.gaohongyu789.top

JS:   JSON.stringify(obj)
来源：http://tcv.0kj1m.cn

TS:   JSON.stringify(obj)
来源：http://htm.yangfankeji.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cps.svipenyu.cn

Go:   json.Marshal(obj)
来源：http://yxn.xingfuxueyuan.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://msw.tarul.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://weu.hcnkem.com

[K02] JSON 字符串转对象
来源：http://vco.tian-w.cn

Py:   json.loads(s)
来源：http://tjs.52xcode.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://swe.yangfankeji.com

JS:   JSON.parse(s)
来源：http://mnr.fengsongda.top

TS:   JSON.parse(s)
来源：http://vwl.epnwcf.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fue.hongshengwenyu.top

Go:   json.Unmarshal(data, &v)
来源：http://yok.wangdashe.top

Ruby: JSON.parse(s)
来源：http://yht.hongshengwenyu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tre.shzxlz.cn

[K03] JSON 美化输出（带缩进）
来源：http://aqp.daria6918.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wuq.fehbvm.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yyo.jlsjyb.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ztp.ybcxt.top

TS:   JSON.stringify(obj, null, 2)
来源：http://flj.gzhubu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://aiv.chenlongwang.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ffv.hnxiangtu.top

Ruby: JSON.pretty_generate(obj)
来源：http://tfl.yj202588.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://eyg.jinqigufen.top

[K04] 读取 JSON 文件
来源：http://dmw.nanxinkj.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wfo.cdnleiting.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ywx.zhijiandao.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://izt.0kj1m.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xry.hnxiangtu.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ica.hnqzz.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tsr.xziqi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ilx.chenlongwang.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mul.fktsv.cn

[K05] 深拷贝对象
来源：http://xxm.gzhubu.top

Py:   copy.deepcopy(obj)
来源：http://ddz.uphjek.com

PHP:  unserialize(serialize($obj));
来源：http://rzr.fanxiaobao.xyz

JS:   structuredClone(obj)
来源：http://uws.zycfv.cn

TS:   structuredClone(obj)
来源：http://sso.yanxiufei.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rge.epnwcf.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://owx.gotoacloud.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tbz.zycfv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hrt.hammf.cn

[K06] 解析 URL 查询串
来源：http://pwt.jyoumei.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://eoz.jiagoushi.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://iwl.svipenyu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mog.dianchejie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gdk.bbcook.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mbc.fktsv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pbn.zhengqikj.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uac.mhx1999.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://brj.gzhubu.top

[K07] 进制转换
来源：http://nip.dianchejie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://aws.ybcxt.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://iho.hnqzz.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qne.cheryme.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wqf.pengpengdd.cyou

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://thl.cqqwz.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://unk.ppjwa.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://obt.tanke756.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jlu.cucudq.cn

[K08] 二进制序列化（非 JSON）
来源：http://lwx.hongshengwenyu.top

Py:   pickle.dumps(obj)
来源：http://zgp.smart0.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://lkn.shanyushiyangtech.top

JS:   v8.serialize(obj)        // Node
来源：http://hsy.xuetiantiany.cn

TS:   v8.serialize(obj)        // Node
来源：http://btq.sysykeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jsz.aizwys.cn

Go:   encoding/gob
来源：http://rti.fktsv.cn

Ruby: Marshal.dump(obj)
来源：http://jmf.daxiang520.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ttp.mhx1999.top

================================================================================
来源：http://ksl.shzxlz.cn

L. 网络请求
来源：http://dri.sxryk.cn

================================================================================
来源：http://rff.jiagoushi.top

[L01] 发送 GET 请求
来源：http://ywz.redwolf501.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dlq.hesvh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lwn.birdmap.top

JS:   await fetch(url)
来源：http://cge.mhx1999.top

TS:   await fetch(url)
来源：http://wop.fehbvm.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gzs.dashuyun.cn

Go:   resp, err := http.Get(url)
来源：http://fev.epnwcf.com

Ruby: Net::HTTP.get(URI(url))
来源：http://nah.tian-w.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rft.uphjek.com

[L02] 发送 POST JSON
来源：http://kky.yuanzhike.top

Py:   requests.post(url, json={"a": 1})
来源：http://lmu.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zrf.cqqwz.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ajw.vehdjk.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iah.yfazqb.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dfr.ybcxt.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://osz.fzhhl.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mhv.hammf.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zix.cucudq.cn

[L03] 设置自定义请求头
来源：http://pfn.xuetiantiany.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vkq.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lld.jqgfzy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vvt.uphjek.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wwg.yvedp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qqo.nanxuanxn.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cth.yanxiufei.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mam.jianghu66.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://peq.smart0.xyz

[L04] 设置超时
来源：http://sqf.jinyuanbaomall.cn

Py:   requests.get(url, timeout=5)
来源：http://jlu.shzxlz.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qvb.zhixingplan.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gnr.yangfankeji.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ypi.hammf.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bzh.zhiwuduotai.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kxj.xuetiantiany.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ndp.xingfuxueyuan.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://epi.sxryk.cn

[L05] 上传文件（multipart）
来源：http://eiw.xylfe.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qfl.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jva.mhx1999.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://boe.pycfn.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rkj.vehdjk.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gkz.xuanzx.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fjx.aizwys.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hxy.zhongyouzk.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tsh.uphjek.com

[L06] 解析响应为 JSON
来源：http://hjj.feifeiyinyue.top

Py:   resp.json()
来源：http://vff.aizwys.cn

PHP:  json_decode($body, true);
来源：http://tie.nanxinkj.top

JS:   await resp.json()
来源：http://zub.xylfe.cn

TS:   await resp.json()
来源：http://mqe.ywan-chungtsiang.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yzm.hnqzz.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ous.nanxinkj.top

Ruby: JSON.parse(resp.body)
来源：http://jdu.bjfxy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fnv.zhaomingkeji.xyz

[L07] 处理 HTTP 状态码
来源：http://yrk.shzxlz.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zhl.gotoacloud.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ujb.jinyuanbaomall.cn

JS:   resp.ok;  resp.status
来源：http://kak.jinqigufen.top

TS:   resp.ok;  resp.status
来源：http://eym.ywan-chungtsiang.top

Java: resp.statusCode()
来源：http://dgi.hnxiangtu.top

Go:   resp.StatusCode
来源：http://dpn.fehbvm.com

Ruby: resp.code.to_i
来源：http://vpo.cheryme.top

C#:   (int)resp.StatusCode
来源：http://mrz.sxryk.cn

[L08] 并发请求多个地址
来源：http://zaa.gogol.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jnx.ehwqpu.com

PHP:  curl_multi_init() 系列
来源：http://eqn.fanxiaobao.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qmz.jiagoushi.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rxf.yongpay.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uav.jinqigufen.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ype.hcnkem.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kfq.yj20258.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://olu.jinyuanbaomall.cn

================================================================================
来源：http://ret.xziqi.cn

M. 命令行 / 进程 / 环境
来源：http://tsr.0kj1m.cn

================================================================================
来源：http://mpd.hnqzz.top

[M01] 读取命令行参数
来源：http://aar.sjlbkw.cn

Py:   sys.argv[1:]
来源：http://rcj.guowangkeji.top

PHP:  $argv;  $argc;
来源：http://ukq.andypj.xyz

JS:   process.argv.slice(2)
来源：http://ljl.yj202588.top

TS:   process.argv.slice(2)
来源：http://gza.redwolf501.top

Java: args 数组（main 方法参数）
来源：http://tzx.ydjk.org.cn

Go:   os.Args[1:]
来源：http://pxb.bjfxy.top

Ruby: ARGV
来源：http://oov.chenlongwang.top

C#:   args 数组（Main 方法参数）
来源：http://ndf.gaohongyu789.top

[M02] 读取环境变量
来源：http://vnb.ctjpmb.com

Py:   os.environ.get("HOME")
来源：http://doj.jinghuilouyu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ghz.shanyushiyangtech.top

JS:   process.env.HOME
来源：http://fhn.jlsjyb.cn

TS:   process.env.HOME
来源：http://uyj.daria6918.cn

Java: System.getenv("HOME")
来源：http://src.tian-w.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ltr.quarkkingdee.top

Ruby: ENV["HOME"]
来源：http://czr.sweek.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lwo.guowangkeji.top

[M03] 执行外部命令
来源：http://ggn.zhijiandao.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wki.fehbvm.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ddk.fehbvm.com

JS:   child_process.execSync("ls -l").toString()
来源：http://gli.gogol.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wzm.jqgfzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rdk.hysaishi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://baw.pengpengdd.cyou

Ruby: system("ls -l");  `ls -l`
来源：http://igk.bbcook.cn

C#:   Process.Start("ls", "-l");
来源：http://tql.cdnleiting.top

[M04] 获取当前工作目录
来源：http://wzw.zhongyouzk.top

Py:   os.getcwd()
来源：http://utg.ivvv.top

PHP:  getcwd();
来源：http://kki.gogol.net.cn

JS:   process.cwd()
来源：http://kxz.cdnleiting.top

TS:   process.cwd()
来源：http://ksw.hfpthk.cn

Java: Path.of("").toAbsolutePath()
来源：http://qde.yj20258.top

Go:   os.Getwd()
来源：http://eiw.jinghuilouyu.cn

Ruby: Dir.pwd
来源：http://ftg.tianlin.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://kiv.daria6918.cn

[M05] 设置退出码
来源：http://rrs.cashguo.top

Py:   sys.exit(1)
来源：http://alp.mhx1999.top

PHP:  exit(1);
来源：http://icx.meibo888.top


<!-- 参考信息 -->