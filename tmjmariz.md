代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gbv.hysaishi.cn

[I07] 忽略大小写与多行模式
来源：http://fvm.cucudq.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cjr.yvedp.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jmx.smart0.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oho.c1oappe.top

TS:   /error/gim
来源：http://kvh.jianghu66.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yfb.tarul.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dcj.jiagoushi.top

Ruby: s.scan(/error/i)
来源：http://uob.c1oappe.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ill.pengpengdd.cyou

[I08] 贪婪与非贪婪匹配
来源：http://keo.fengsongda.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kgi.yj20258888.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://npa.zhijiandao.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vjc.bjfxy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lpf.sweek.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ztg.zdbjq.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zmw.fanxiaobao.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://eua.jinyuanbaomall.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ptm.cheryme.top

================================================================================
来源：http://eyq.sxryk.cn

J. 日期与时间
来源：http://eis.cdnleiting.top

================================================================================
来源：http://les.sysykeji.top

[J01] 获取当前时间
来源：http://chu.pengpengdd.cyou

Py:   datetime.now();  datetime.now(UTC)
来源：http://mud.tian-w.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fgz.tanke756.top

JS:   new Date();  Date.now()
来源：http://hju.hcnkem.com

TS:   new Date();  Date.now()
来源：http://hjb.andypj.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://cjk.epnwcf.com

Go:   time.Now()
来源：http://nma.gzhubu.top

Ruby: Time.now
来源：http://taq.smart0.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sep.fehbvm.com

[J02] 格式化输出
来源：http://bqi.nwbrower.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vpk.feifeiyinyue.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hvq.yfazqb.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bdm.fengsongda.top

TS:   d.toISOString()
来源：http://gxt.fanxiaobao.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pjm.ywan-chungtsiang.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://low.jinghuilouyu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bkw.snrcjt.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jkx.gogol.net.cn

[J03] 字符串解析为日期
来源：http://hcu.zhixingplan.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rwu.ctjpmb.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gri.cqqwz.cn

JS:   new Date("2024-01-02")
来源：http://xrx.aizwys.cn

TS:   new Date("2024-01-02")
来源：http://kaf.daxiang520.top

Java: LocalDate.parse("2024-01-02")
来源：http://gwo.snrcjt.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://umw.tian-w.cn

Ruby: Date.parse("2024-01-02")
来源：http://opq.52xcode.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ooc.jyoumei.cn

[J04] 时间戳与日期互转
来源：http://zdn.hcnkem.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://src.jinghuilouyu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gkl.dashuyun.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ppu.hywenlv.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://auj.jinqigufen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://txn.fzhhl.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ohq.fzhhl.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cry.shzxlz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lip.zhongyouzk.top

[J05] 时间加减（加 7 天）
来源：http://csv.yuanzhike.top

Py:   now + timedelta(days=7)
来源：http://wfj.ctjpmb.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://znp.xuanzx.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mbg.chenzaomai.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qid.sufxvd.cn

Java: LocalDate.now().plusDays(7)
来源：http://nmc.cdnleiting.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qee.havefunace.top

Ruby: Time.now + 7 * 86400
来源：http://xuy.xylfe.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hfk.zhixingplan.top

[J06] 计算两时间之差
来源：http://qoe.tian-w.cn

Py:   (end - start).total_seconds()
来源：http://lij.ppjwa.cn

PHP:  $end->diff($start)->days;
来源：http://mmy.zycfv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bev.zhixingplan.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jxv.tarul.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dmp.52xcode.cn

Go:   end.Sub(start).Hours()
来源：http://drg.aizwys.cn

Ruby: end - start                 # 返回秒数
来源：http://nke.sufxvd.cn

C#:   (end - start).TotalSeconds
来源：http://ujp.hywenlv.cn

[J07] 比较两个日期
来源：http://atp.sysykeji.top

Py:   d1 < d2;  d1 == d2
来源：http://dhm.smart0.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ofz.316326.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://mlv.jinqigfzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://mcl.cqqwz.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ecm.vqdsnc.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sfh.shzxlz.cn

Ruby: d1 < d2;  d1 == d2
来源：http://esl.shzxlz.cn

C#:   d1 < d2;  d1 == d2
来源：http://enm.cqqwz.cn

[J08] 提取年月日与星期
来源：http://syt.cucudq.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ojn.pengpengdd.cyou

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lxm.ywan-chungtsiang.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://emp.feifeiyinyue.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nov.zdqjudy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rjs.ivvv.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xak.xuetiantiany.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qpe.haohaochexian.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tga.ybcxt.top

[J09] 时区处理
来源：http://zth.jianghu66.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gpm.tianlin.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fww.guowangkeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bzu.yonumen.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vyf.kuanghao11.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ica.ctjpmb.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://coj.shanyushiyangtech.top

Ruby: Time.now.getlocal("+08:00")
来源：http://yfm.xuetiantiany.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ugo.andypj.xyz

[J10] 取今天 / 本月第一天
来源：http://eqq.zycfv.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ysf.yanxiufei.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://twp.havefunace.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dgy.yuanzhike.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pdi.gogol.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wkc.jinyuanbaomall.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pxf.cqqwz.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qib.ppjwa.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qmq.bjfxy.top

================================================================================
来源：http://zaa.zhoulong.xyz

K. JSON 与序列化
来源：http://xab.hnxiangtu.top

================================================================================
来源：http://ero.guowangkeji.top

[K01] 对象转 JSON 字符串
来源：http://zdf.zhongyouzk.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jgv.ppjwa.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yhn.jinyuanbaomall.cn

JS:   JSON.stringify(obj)
来源：http://yeb.aizwys.cn

TS:   JSON.stringify(obj)
来源：http://eam.shanyushiyangkeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rii.meibo888.top

Go:   json.Marshal(obj)
来源：http://drb.nanxuanxn.top

Ruby: obj.to_json                                     // require "json"
来源：http://uuv.daria6918.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lbv.daria6918.cn

[K02] JSON 字符串转对象
来源：http://mpb.jinyuanbaomall.cn

Py:   json.loads(s)
来源：http://qlk.xinyue.icu

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://oaf.tianlin.xyz

JS:   JSON.parse(s)
来源：http://jmq.ywan-chungtsiang.top

TS:   JSON.parse(s)
来源：http://hpc.fengsongda.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xpq.redwolf501.top

Go:   json.Unmarshal(data, &v)
来源：http://guo.bbcook.cn

Ruby: JSON.parse(s)
来源：http://zwv.gaohongyu789.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kff.52xcode.cn

[K03] JSON 美化输出（带缩进）
来源：http://mcg.zhixingplan.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qcn.hysaishi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wjh.9152youxi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rdr.aizwys.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hqb.gotoacloud.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://iou.cdnleiting.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yuj.gzhubu.top

Ruby: JSON.pretty_generate(obj)
来源：http://xge.jinqigufen.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rzx.redwolf501.top

[K04] 读取 JSON 文件
来源：http://pnz.wangshuangyany.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ieg.ydzc1.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://omm.fehbvm.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://whp.yfazqb.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wns.cucudq.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tya.meibo888.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fav.316326.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://ogl.birdmap.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mvx.hnxiangtu.top

[K05] 深拷贝对象
来源：http://olz.yonumen.top

Py:   copy.deepcopy(obj)
来源：http://fqo.ctjpmb.com

PHP:  unserialize(serialize($obj));
来源：http://kgw.gogol.net.cn

JS:   structuredClone(obj)
来源：http://diu.zdqjudy.top

TS:   structuredClone(obj)
来源：http://fbu.jqgfzy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://yys.dianchejie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kuf.vehdjk.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://srb.xziqi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hvs.9152youxi.cn

[K06] 解析 URL 查询串
来源：http://riv.hysaishi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jhi.dianchejie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wvx.iojbl.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://syc.jlsjyb.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ajm.sufxvd.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://snh.dashuyun.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bap.snrcjt.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nyr.jqgfzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hcr.aibaodan.cn

[K07] 进制转换
来源：http://mzb.gaohongyu789.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cvm.gaohongyu789.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ncp.sysykeji.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xew.yuanzhike.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sgw.jianghu66.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fbt.sysykeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://spw.0kj1m.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fix.shangyingyoupin.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uwv.hnxiangtu.top

[K08] 二进制序列化（非 JSON）
来源：http://vqc.jyoumei.cn

Py:   pickle.dumps(obj)
来源：http://xzf.shanyushiyangkeji.top

PHP:  serialize($obj);  unserialize($s);
来源：http://znp.yanxiufei.cn

JS:   v8.serialize(obj)        // Node
来源：http://huc.shzxlz.cn

TS:   v8.serialize(obj)        // Node
来源：http://tre.jyoumei.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cae.cqqwz.cn

Go:   encoding/gob
来源：http://sdz.iojbl.cn

Ruby: Marshal.dump(obj)
来源：http://rdl.ehwqpu.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://isw.chenzaomai.com

================================================================================
来源：http://pgu.c1oappe.top

L. 网络请求
来源：http://zee.gotoacloud.top

================================================================================
来源：http://bxg.fehbvm.com

[L01] 发送 GET 请求
来源：http://bfw.vehdjk.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://egp.wangshuangyany.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://acg.xinyue.icu

JS:   await fetch(url)
来源：http://klp.yueranfly.top

TS:   await fetch(url)
来源：http://zie.yj20258.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://huo.ivvv.top

Go:   resp, err := http.Get(url)
来源：http://esg.sysykeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://nww.hfpthk.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vgs.jinghuilouyu.cn

[L02] 发送 POST JSON
来源：http://elz.zhijiandao.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hlt.sxryk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jjk.yueranfly.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fhn.316326.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kqw.bbcook.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zeo.jyoumei.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ira.birdmap.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kcg.shanyushiyangkeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fxq.xuetiantiany.cn

[L03] 设置自定义请求头
来源：http://nyo.wangdashe.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vac.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zrr.wangshuangyany.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vlr.ybcxt.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kjv.ctjpmb.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yql.svipenyu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://iml.hysaishi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://oxa.aibaodan.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://irg.zhongyouzk.top

[L04] 设置超时
来源：http://oub.hywenlv.cn

Py:   requests.get(url, timeout=5)
来源：http://gto.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qbb.hfpthk.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cup.jqgfzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ekz.smart0.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xxt.tanke756.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fea.fehbvm.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fqw.gotoacloud.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gch.fengsongda.top

[L05] 上传文件（multipart）
来源：http://eqv.xuanzx.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zih.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kiu.epnwcf.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ncp.meibo888.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uno.iojbl.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zry.jlsjyb.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://krm.cqqwz.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ggr.pengpengdd.cyou

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://edo.ydzc1.top

[L06] 解析响应为 JSON
来源：http://jqf.bjfxy.top

Py:   resp.json()
来源：http://srr.uphjek.com

PHP:  json_decode($body, true);
来源：http://map.ivvv.top

JS:   await resp.json()
来源：http://oke.jiagoushi.top

TS:   await resp.json()
来源：http://nug.yj202588.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rxn.tarul.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wfw.52xcode.cn

Ruby: JSON.parse(resp.body)
来源：http://ryh.daxiang520.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nqb.zhixingplan.top

[L07] 处理 HTTP 状态码
来源：http://jmf.tarul.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xum.yj202588.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fjk.mhx1999.top

JS:   resp.ok;  resp.status
来源：http://dxy.daria6918.cn

TS:   resp.ok;  resp.status
来源：http://inc.zhoulong.xyz

Java: resp.statusCode()
来源：http://uwa.yueranfly.top

Go:   resp.StatusCode
来源：http://ggy.svipenyu.cn

Ruby: resp.code.to_i
来源：http://idy.sxryk.cn

C#:   (int)resp.StatusCode
来源：http://txc.ywan-chungtsiang.top

[L08] 并发请求多个地址
来源：http://bzg.yongpay.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rau.fzhhl.top

PHP:  curl_multi_init() 系列
来源：http://lrl.yfazqb.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://etv.wangdashe.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kfn.aizwys.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://snq.jinqigfzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dbe.ctjpmb.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ypc.chenzaomai.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yic.shuidangran.top

================================================================================
来源：http://ezq.yfazqb.com

M. 命令行 / 进程 / 环境
来源：http://hwi.wangshuangyany.cn

================================================================================
来源：http://qiw.jinyuanbaomall.cn

[M01] 读取命令行参数
来源：http://enz.0kj1m.cn

Py:   sys.argv[1:]
来源：http://ota.epnwcf.com

PHP:  $argv;  $argc;
来源：http://xnz.snrcjt.cn

JS:   process.argv.slice(2)
来源：http://imm.hnqzz.top

TS:   process.argv.slice(2)
来源：http://tij.yongpay.top

Java: args 数组（main 方法参数）
来源：http://pfh.yanxiufei.cn

Go:   os.Args[1:]
来源：http://gvg.ehwqpu.com

Ruby: ARGV
来源：http://qyx.xuetiantiany.cn

C#:   args 数组（Main 方法参数）
来源：http://mwb.shzxlz.cn

[M02] 读取环境变量
来源：http://hjx.jinyuanbaomall.cn

Py:   os.environ.get("HOME")
来源：http://tzl.ydzc1.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pzq.ppjwa.cn

JS:   process.env.HOME
来源：http://umo.meibo888.top

TS:   process.env.HOME
来源：http://pcz.tanke756.top

Java: System.getenv("HOME")
来源：http://dgh.gogol.net.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://aqz.zhongyouzk.top

Ruby: ENV["HOME"]
来源：http://zhe.316326.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kck.xingfuxueyuan.xyz

[M03] 执行外部命令
来源：http://sog.tian-w.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vmf.zhijiandao.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mnm.zhiwuduotai.top

JS:   child_process.execSync("ls -l").toString()
来源：http://rez.ctjpmb.com

TS:   child_process.execSync("ls -l").toString()
来源：http://hyx.guannengcc.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tia.yvedp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fhq.pycfn.com

Ruby: system("ls -l");  `ls -l`
来源：http://aok.feifeiyinyue.top

C#:   Process.Start("ls", "-l");
来源：http://ydp.sysykeji.top

[M04] 获取当前工作目录
来源：http://eao.guowangkeji.top

Py:   os.getcwd()
来源：http://mwa.ywan-chungtsiang.top

PHP:  getcwd();
来源：http://qin.zhiwuduotai.top

JS:   process.cwd()
来源：http://fgf.fanxiaobao.xyz

TS:   process.cwd()
来源：http://waa.zhixingplan.top

Java: Path.of("").toAbsolutePath()
来源：http://lix.hnxiangtu.top

Go:   os.Getwd()
来源：http://bns.yfazqb.com

Ruby: Dir.pwd
来源：http://paw.yanxiufei.cn


<!-- 参考信息 -->