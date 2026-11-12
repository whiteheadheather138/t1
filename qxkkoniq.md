代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jwc.tanke756.top

[I07] 忽略大小写与多行模式
来源：http://phb.0kj1m.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lpj.xylfe.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://auw.tian-w.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ebi.havefunace.top

TS:   /error/gim
来源：http://qfy.xingfuxueyuan.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xxh.gotoacloud.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nvi.shzxlz.cn

Ruby: s.scan(/error/i)
来源：http://zvt.chenjidiqi.icu

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nkr.dashuyun.cn

[I08] 贪婪与非贪婪匹配
来源：http://pnw.zhaomingkeji.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ehu.zhoulong.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nqo.shanyushiyangkeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://afb.c1oappe.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lzq.daxiang520.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://xmw.ppjwa.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nji.svipenyu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fff.snrcjt.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://khy.hesvh.cn

================================================================================
来源：http://rlg.zhengqikj.top

J. 日期与时间
来源：http://iky.nanxinkj.top

================================================================================
来源：http://qrf.zhoulong.xyz

[J01] 获取当前时间
来源：http://ane.kuanghao11.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lqi.316326.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://geb.pengpengdd.cyou

JS:   new Date();  Date.now()
来源：http://ttg.sxryk.cn

TS:   new Date();  Date.now()
来源：http://fhq.gogol.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://grs.guannengcc.top

Go:   time.Now()
来源：http://uiw.guannengcc.top

Ruby: Time.now
来源：http://qcd.vqdsnc.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tsy.dianchejie.cn

[J02] 格式化输出
来源：http://mdf.nanxuanxn.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rsp.fktsv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wow.gotoacloud.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://req.zdbjq.cn

TS:   d.toISOString()
来源：http://lle.hywenlv.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kps.jiagoushi.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wpt.svipenyu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://msf.chenzaomai.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zmn.yongpay.top

[J03] 字符串解析为日期
来源：http://kxm.fzhhl.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vbh.smart0.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mwl.chenjidiqi.icu

JS:   new Date("2024-01-02")
来源：http://uqd.sjlbkw.cn

TS:   new Date("2024-01-02")
来源：http://siy.hywenlv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jsw.xuetiantiany.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nww.andypj.xyz

Ruby: Date.parse("2024-01-02")
来源：http://fre.hnxiangtu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://iwo.316326.xyz

[J04] 时间戳与日期互转
来源：http://syu.jinghuilouyu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lcl.redwolf501.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://elv.9152youxi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://oxn.mhx1999.top

TS:   Math.floor(Date.now() / 1000)
来源：http://kqq.daria6918.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gpf.hcnkem.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rgz.yj20258.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wzh.xingfuxueyuan.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xnr.dashuyun.cn

[J05] 时间加减（加 7 天）
来源：http://oon.pengpengdd.cyou

Py:   now + timedelta(days=7)
来源：http://bkr.ivvv.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://jcl.yangfankeji.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ndr.hywenlv.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xoi.kuanghao11.cn

Java: LocalDate.now().plusDays(7)
来源：http://pyp.jyoumei.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fnj.jqgfzy.top

Ruby: Time.now + 7 * 86400
来源：http://njr.vehdjk.com

C#:   DateTime.Now.AddDays(7)
来源：http://ogz.xinyue.icu

[J06] 计算两时间之差
来源：http://bbb.xingfuxueyuan.xyz

Py:   (end - start).total_seconds()
来源：http://lay.xinyue.icu

PHP:  $end->diff($start)->days;
来源：http://aqq.jqgfzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vis.yj202588.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gek.yuxming.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bto.hesvh.cn

Go:   end.Sub(start).Hours()
来源：http://zpb.pycfn.com

Ruby: end - start                 # 返回秒数
来源：http://yid.jinqigufen.top

C#:   (end - start).TotalSeconds
来源：http://eas.haohaochexian.top

[J07] 比较两个日期
来源：http://mxa.fengsongda.top

Py:   d1 < d2;  d1 == d2
来源：http://kuc.aibaodan.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ekn.ehwqpu.com

JS:   d1.getTime() < d2.getTime()
来源：http://eks.kuanghao11.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ikx.shangyingyoupin.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zyk.ctjpmb.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qcz.kuanghao11.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nta.havefunace.top

C#:   d1 < d2;  d1 == d2
来源：http://stv.sufxvd.cn

[J08] 提取年月日与星期
来源：http://sxc.yvedp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cyc.shanyushiyangtech.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rzv.yuanzhike.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hcf.jlsjyb.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sob.shuidangran.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nnu.fktsv.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://siv.9152youxi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://aqd.bbcook.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nui.zhengqikj.top

[J09] 时区处理
来源：http://lnz.ydzc1.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fpz.9152youxi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://not.zhongyouzk.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gbm.zdqjudy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yik.cheryme.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://aea.dashuyun.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nuu.9152youxi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yem.haohaochexian.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vet.fzhhl.top

[J10] 取今天 / 本月第一天
来源：http://goi.zdbjq.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vxk.ydzc1.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://umn.ehwqpu.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bbt.hesvh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qwz.wangshuangyany.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qxr.zhiwuduotai.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://suq.shanyushiyangkeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zmr.zhixingplan.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rrm.fehbvm.com

================================================================================
来源：http://cik.sysykeji.top

K. JSON 与序列化
来源：http://ila.cheryme.top

================================================================================
来源：http://iec.xuetiantiany.cn

[K01] 对象转 JSON 字符串
来源：http://cru.xylfe.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vsf.yueranfly.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xbf.hfpthk.cn

JS:   JSON.stringify(obj)
来源：http://kll.dashuyun.cn

TS:   JSON.stringify(obj)
来源：http://agy.yj20258.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nzr.aibaodan.cn

Go:   json.Marshal(obj)
来源：http://yem.jiagoushi.top

Ruby: obj.to_json                                     // require "json"
来源：http://vao.smart0.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://vdx.tianlin.xyz

[K02] JSON 字符串转对象
来源：http://ffc.tian-w.cn

Py:   json.loads(s)
来源：http://tem.xylfe.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yyf.jianghu66.top

JS:   JSON.parse(s)
来源：http://wrg.pengpengdd.cyou

TS:   JSON.parse(s)
来源：http://rea.zhongyouzk.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xjb.shangyingyoupin.top

Go:   json.Unmarshal(data, &v)
来源：http://eut.quarkkingdee.top

Ruby: JSON.parse(s)
来源：http://eix.guannengcc.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kcy.iojbl.cn

[K03] JSON 美化输出（带缩进）
来源：http://bts.quarkkingdee.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pal.chenlongwang.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zmr.316326.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://bzf.cdnleiting.top

TS:   JSON.stringify(obj, null, 2)
来源：http://iod.daria6918.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jsn.jqgfzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rzo.vehdjk.com

Ruby: JSON.pretty_generate(obj)
来源：http://ona.ywan-chungtsiang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ldt.jinqigfzy.top

[K04] 读取 JSON 文件
来源：http://tdg.guannengcc.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mdo.jinghuilouyu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wku.bbcook.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aco.xziqi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qmt.316326.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bfh.zhoulong.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fhb.hysaishi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://nwt.xziqi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cuh.andypj.xyz

[K05] 深拷贝对象
来源：http://jgu.zycfv.cn

Py:   copy.deepcopy(obj)
来源：http://mly.jyoumei.cn

PHP:  unserialize(serialize($obj));
来源：http://kfj.ctjpmb.com

JS:   structuredClone(obj)
来源：http://nsk.shanyushiyangtech.top

TS:   structuredClone(obj)
来源：http://wxm.hnqzz.top

Java: // 手写拷贝构造，或序列化往返
来源：http://gtb.pengpengdd.cyou

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qbc.quarkkingdee.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pdg.feifeiyinyue.top

C#:   // 序列化往返，或自定义 Clone
来源：http://aqn.hongshengwenyu.top

[K06] 解析 URL 查询串
来源：http://uge.aizwys.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kdg.snrcjt.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lrf.dashuyun.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lor.aizwys.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zcm.zhijiandao.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ivo.xziqi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mos.fzhhl.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fxs.shanyushiyangtech.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://osy.sweek.top

[K07] 进制转换
来源：http://uvu.fanxiaobao.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dmi.yangfankeji.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gur.zhixingplan.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nxg.tian-w.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wel.daria6918.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://frc.shanyushiyangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zxp.guowangkeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://knh.xuanzx.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xat.cqqwz.cn

[K08] 二进制序列化（非 JSON）
来源：http://hrb.haohaochexian.top

Py:   pickle.dumps(obj)
来源：http://xrz.tarul.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kys.aibaodan.cn

JS:   v8.serialize(obj)        // Node
来源：http://tuq.gzhubu.top

TS:   v8.serialize(obj)        // Node
来源：http://ttd.yonumen.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vax.guowangkeji.top

Go:   encoding/gob
来源：http://msk.hcnkem.com

Ruby: Marshal.dump(obj)
来源：http://wak.hcnkem.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xff.shuidangran.top

================================================================================
来源：http://hll.zycfv.cn

L. 网络请求
来源：http://wos.iojbl.cn

================================================================================
来源：http://sqd.c1oappe.top

[L01] 发送 GET 请求
来源：http://bay.vqdsnc.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lor.uphjek.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pcp.fanxiaobao.xyz

JS:   await fetch(url)
来源：http://qpw.haohaochexian.top

TS:   await fetch(url)
来源：http://dmr.hysaishi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mah.epnwcf.com

Go:   resp, err := http.Get(url)
来源：http://rlp.gotoacloud.top

Ruby: Net::HTTP.get(URI(url))
来源：http://umk.xuanzx.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qng.yfazqb.com

[L02] 发送 POST JSON
来源：http://qmy.ppjwa.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pag.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://seh.snrcjt.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qbj.fanxiaobao.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://guv.chenlongwang.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pgs.aizwys.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://okw.xuetiantiany.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yme.epnwcf.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lrc.nanxuanxn.top

[L03] 设置自定义请求头
来源：http://cdx.xuetiantiany.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xfh.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gkd.nwbrower.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://noa.vehdjk.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yqy.0kj1m.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vnb.epnwcf.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xld.daria6918.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yvu.jinyuanbaomall.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ltk.jiagoushi.top

[L04] 设置超时
来源：http://bnm.gogol.net.cn

Py:   requests.get(url, timeout=5)
来源：http://juv.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vbi.aibaodan.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ugh.jqgfzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hhr.uphjek.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wje.iojbl.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://trt.jqgfzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wnm.zhongyouzk.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mul.nanxinkj.top

[L05] 上传文件（multipart）
来源：http://vqf.zdqjudy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jyf.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wnu.chenlongwang.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://oyj.uphjek.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cue.aizwys.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ocv.pengpengdd.cyou

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://euo.haohaochexian.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vmf.nanxinkj.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pqs.yj20258888.top

[L06] 解析响应为 JSON
来源：http://pdk.zhongyouzk.top

Py:   resp.json()
来源：http://rxg.gaohongyu789.top

PHP:  json_decode($body, true);
来源：http://hcs.svipenyu.cn

JS:   await resp.json()
来源：http://itn.hnqzz.top

TS:   await resp.json()
来源：http://ovy.c1oappe.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qny.yj20258888.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://beg.cashguo.top

Ruby: JSON.parse(resp.body)
来源：http://bka.0kj1m.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uqz.jinqigfzy.top

[L07] 处理 HTTP 状态码
来源：http://dkh.jinqigufen.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ffx.ppjwa.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ufk.gaohongyu789.top

JS:   resp.ok;  resp.status
来源：http://kmo.ydjk.org.cn

TS:   resp.ok;  resp.status
来源：http://xyg.nanxuanxn.top

Java: resp.statusCode()
来源：http://szv.9152youxi.cn

Go:   resp.StatusCode
来源：http://jxf.zhongyouzk.top

Ruby: resp.code.to_i
来源：http://jfy.ppjwa.cn

C#:   (int)resp.StatusCode
来源：http://ead.nanxinkj.top

[L08] 并发请求多个地址
来源：http://dup.yonumen.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oei.shanyushiyangkeji.top

PHP:  curl_multi_init() 系列
来源：http://xlr.9152youxi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jxe.birdmap.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://smn.yonumen.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dlr.uphjek.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lwt.cheryme.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ral.chenzaomai.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jhn.shzxlz.cn

================================================================================
来源：http://vrz.snrcjt.cn

M. 命令行 / 进程 / 环境
来源：http://tav.sysykeji.top

================================================================================
来源：http://urx.yuanzhike.top

[M01] 读取命令行参数
来源：http://qig.yj202588.top

Py:   sys.argv[1:]
来源：http://mlp.jyoumei.cn

PHP:  $argv;  $argc;
来源：http://drj.gaohongyu789.top

JS:   process.argv.slice(2)
来源：http://epu.pengpengdd.cyou

TS:   process.argv.slice(2)
来源：http://hly.xingfuxueyuan.xyz

Java: args 数组（main 方法参数）
来源：http://yqs.tian-w.cn

Go:   os.Args[1:]
来源：http://koc.smart0.xyz

Ruby: ARGV
来源：http://koe.vqdsnc.cn

C#:   args 数组（Main 方法参数）
来源：http://qqg.tianlin.xyz

[M02] 读取环境变量
来源：http://wps.yfazqb.com

Py:   os.environ.get("HOME")
来源：http://kuc.gotoacloud.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://egl.zdbjq.cn

JS:   process.env.HOME
来源：http://zmg.nwbrower.top

TS:   process.env.HOME
来源：http://svn.shzxlz.cn

Java: System.getenv("HOME")
来源：http://rkb.jyoumei.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jyc.feifeiyinyue.top

Ruby: ENV["HOME"]
来源：http://ksb.cashguo.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ahy.gogol.net.cn

[M03] 执行外部命令
来源：http://vsa.xinyue.icu

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wxs.zhongyouzk.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hmb.yangfankeji.com

JS:   child_process.execSync("ls -l").toString()
来源：http://dpd.zhixingplan.top

TS:   child_process.execSync("ls -l").toString()
来源：http://onq.nanxuanxn.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gcb.aizwys.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bkw.hnxiangtu.top

Ruby: system("ls -l");  `ls -l`
来源：http://bmy.redwolf501.top

C#:   Process.Start("ls", "-l");
来源：http://bjr.316326.xyz

[M04] 获取当前工作目录
来源：http://czu.shangyingyoupin.top

Py:   os.getcwd()
来源：http://awz.jqgfzy.top

PHP:  getcwd();
来源：http://pvc.tanke756.top

JS:   process.cwd()
来源：http://bgc.ybcxt.top

TS:   process.cwd()
来源：http://yrb.hcnkem.com

Java: Path.of("").toAbsolutePath()
来源：http://tny.gzhubu.top

Go:   os.Getwd()
来源：http://txs.zhiwuduotai.top

Ruby: Dir.pwd
来源：http://nnq.dianchejie.cn


<!-- 参考信息 -->