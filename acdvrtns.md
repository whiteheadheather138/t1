代发 wailian999

Ruby: s.scan(/error/i)
来源：http://iim.shanyushiyangkeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dfz.nanxuanxn.top

[I08] 贪婪与非贪婪匹配
来源：http://uta.aibaodan.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ovi.chenlongwang.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tez.dashuyun.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://knx.ydjk.org.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ilv.yuxming.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bld.gaohongyu789.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qwd.pycfn.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zyd.snrcjt.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://syg.fanxiaobao.xyz

================================================================================
来源：http://cdn.shuidangran.top

J. 日期与时间
来源：http://ckz.tianlin.xyz

================================================================================
来源：http://dfb.cheryme.top

[J01] 获取当前时间
来源：http://osj.cucudq.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ytk.52xcode.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bkp.epnwcf.com

JS:   new Date();  Date.now()
来源：http://cgc.316326.xyz

TS:   new Date();  Date.now()
来源：http://bwc.ehwqpu.com

Java: LocalDateTime.now();  Instant.now()
来源：http://shr.nwbrower.top

Go:   time.Now()
来源：http://zkj.jinyuanbaomall.cn

Ruby: Time.now
来源：http://yca.tarul.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ysg.ydzc1.top

[J02] 格式化输出
来源：http://mzh.cashguo.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dmg.hnqzz.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lit.mhx1999.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mim.haohaochexian.top

TS:   d.toISOString()
来源：http://pbm.ppjwa.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mja.zhiwuduotai.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sjr.tanke756.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lfx.wangshuangyany.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jsk.tianlin.xyz

[J03] 字符串解析为日期
来源：http://ohq.zhengqikj.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tok.ybcxt.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://alf.ywan-chungtsiang.top

JS:   new Date("2024-01-02")
来源：http://kuq.guannengcc.top

TS:   new Date("2024-01-02")
来源：http://xmh.cheryme.top

Java: LocalDate.parse("2024-01-02")
来源：http://psb.zhiwuduotai.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nzx.ppjwa.cn

Ruby: Date.parse("2024-01-02")
来源：http://nil.chenzaomai.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://una.yvedp.cn

[J04] 时间戳与日期互转
来源：http://zbn.zhijiandao.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kgi.ydzc1.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xzf.sxryk.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://paj.ppjwa.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://uay.fehbvm.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ozm.yangfankeji.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://san.yj20258888.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rvw.yuxming.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gnx.yanxiufei.cn

[J05] 时间加减（加 7 天）
来源：http://fmr.cashguo.top

Py:   now + timedelta(days=7)
来源：http://wlz.zhongyouzk.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://kco.zhaomingkeji.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tgn.bjfxy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ede.gotoacloud.top

Java: LocalDate.now().plusDays(7)
来源：http://ipf.hysaishi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yoh.aizwys.cn

Ruby: Time.now + 7 * 86400
来源：http://tlu.zhixingplan.top

C#:   DateTime.Now.AddDays(7)
来源：http://dvo.yongpay.top

[J06] 计算两时间之差
来源：http://gnd.chenzaomai.com

Py:   (end - start).total_seconds()
来源：http://efv.chenzaomai.com

PHP:  $end->diff($start)->days;
来源：http://itj.daria6918.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wbx.sweek.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jct.yueranfly.top

Java: Duration.between(start, end).toSeconds()
来源：http://ucw.xingfuxueyuan.xyz

Go:   end.Sub(start).Hours()
来源：http://idp.ppjwa.cn

Ruby: end - start                 # 返回秒数
来源：http://agi.sweek.top

C#:   (end - start).TotalSeconds
来源：http://xvw.yonumen.top

[J07] 比较两个日期
来源：http://lyf.xuetiantiany.cn

Py:   d1 < d2;  d1 == d2
来源：http://nul.cucudq.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cck.havefunace.top

JS:   d1.getTime() < d2.getTime()
来源：http://tch.52xcode.cn

TS:   d1.getTime() < d2.getTime()
来源：http://grf.ywan-chungtsiang.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xzs.birdmap.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://req.zycfv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wbr.shanyushiyangkeji.top

C#:   d1 < d2;  d1 == d2
来源：http://bts.dianchejie.cn

[J08] 提取年月日与星期
来源：http://ldf.zhiwuduotai.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hfd.zhaomingkeji.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cpa.nanxuanxn.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ybz.iojbl.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://eyz.shanyushiyangkeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://trs.ydzc1.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lwu.wangdashe.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zkh.hysaishi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lvj.yueranfly.top

[J09] 时区处理
来源：http://puz.jlsjyb.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://grp.jqgfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://aoq.tanke756.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bkb.zdbjq.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ylb.meibo888.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ncd.hfpthk.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kzv.fanxiaobao.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://biu.smart0.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gmz.fengsongda.top

[J10] 取今天 / 本月第一天
来源：http://zla.fengsongda.top

Py:   date.today();  date.today().replace(day=1)
来源：http://gmx.tarul.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wve.shuidangran.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ahf.sweek.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gwl.ppjwa.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sdc.aizwys.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hca.xingfuxueyuan.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yfk.jianghu66.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jus.ybcxt.top

================================================================================
来源：http://lol.hammf.cn

K. JSON 与序列化
来源：http://oxr.cdnleiting.top

================================================================================
来源：http://hrb.gotoacloud.top

[K01] 对象转 JSON 字符串
来源：http://wlw.9152youxi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nuj.sysykeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://atv.cheryme.top

JS:   JSON.stringify(obj)
来源：http://jgs.ppjwa.cn

TS:   JSON.stringify(obj)
来源：http://gds.redwolf501.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://iin.xziqi.cn

Go:   json.Marshal(obj)
来源：http://osk.yangfankeji.com

Ruby: obj.to_json                                     // require "json"
来源：http://owc.vqdsnc.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://uub.jinqigufen.top

[K02] JSON 字符串转对象
来源：http://atb.zhiwuduotai.top

Py:   json.loads(s)
来源：http://ika.yj202588.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://aid.bbcook.cn

JS:   JSON.parse(s)
来源：http://dxv.tarul.cn

TS:   JSON.parse(s)
来源：http://apt.cucudq.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oof.yongpay.top

Go:   json.Unmarshal(data, &v)
来源：http://frg.quarkkingdee.top

Ruby: JSON.parse(s)
来源：http://kih.dianchejie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://khb.yj202588.top

[K03] JSON 美化输出（带缩进）
来源：http://xqm.jinyuanbaomall.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rbr.hesvh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dsa.chenlongwang.top

JS:   JSON.stringify(obj, null, 2)
来源：http://gfo.wangshuangyany.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xll.sxryk.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://htc.cheryme.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mny.aibaodan.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ahm.sysykeji.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://til.jqgufenzy.top

[K04] 读取 JSON 文件
来源：http://uzi.birdmap.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bnx.shzxlz.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dkn.mhx1999.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://psh.316326.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hxa.sysykeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sbh.cheryme.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mjp.fktsv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://sfz.cdnleiting.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wzl.c1oappe.top

[K05] 深拷贝对象
来源：http://aut.9152youxi.cn

Py:   copy.deepcopy(obj)
来源：http://gnx.c1oappe.top

PHP:  unserialize(serialize($obj));
来源：http://cwn.havefunace.top

JS:   structuredClone(obj)
来源：http://qcn.zdbjq.cn

TS:   structuredClone(obj)
来源：http://hdr.birdmap.top

Java: // 手写拷贝构造，或序列化往返
来源：http://jth.chenzaomai.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gwz.ywan-chungtsiang.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://txr.hnxiangtu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://dns.xingfuxueyuan.xyz

[K06] 解析 URL 查询串
来源：http://nid.epnwcf.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ssu.hywenlv.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fqf.shuidangran.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rkf.uphjek.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://anp.jinyuanbaomall.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dmg.yuanzhike.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://xav.hesvh.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jey.dianchejie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uvi.hongshengwenyu.top

[K07] 进制转换
来源：http://zjd.havefunace.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://meu.ydjk.org.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jux.sjlbkw.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ihi.shuidangran.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jgd.9152youxi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vvz.zhoulong.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://foo.yongpay.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ipi.chenjidiqi.icu

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://upn.ehwqpu.com

[K08] 二进制序列化（非 JSON）
来源：http://ona.xinyue.icu

Py:   pickle.dumps(obj)
来源：http://ybf.nwbrower.top

PHP:  serialize($obj);  unserialize($s);
来源：http://phu.redwolf501.top

JS:   v8.serialize(obj)        // Node
来源：http://amu.jinqigufen.top

TS:   v8.serialize(obj)        // Node
来源：http://fkc.zhijiandao.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xmc.cheryme.top

Go:   encoding/gob
来源：http://gii.bbcook.cn

Ruby: Marshal.dump(obj)
来源：http://spu.tanke756.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uwd.zhijiandao.cn

================================================================================
来源：http://eac.daxiang520.top

L. 网络请求
来源：http://kgp.havefunace.top

================================================================================
来源：http://dii.fanxiaobao.xyz

[L01] 发送 GET 请求
来源：http://kld.hysaishi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wpg.xuetiantiany.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rqk.nanxinkj.top

JS:   await fetch(url)
来源：http://yfq.epnwcf.com

TS:   await fetch(url)
来源：http://gzx.hysaishi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ukv.hcnkem.com

Go:   resp, err := http.Get(url)
来源：http://llr.feifeiyinyue.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ffj.jlsjyb.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uzx.nanxinkj.top

[L02] 发送 POST JSON
来源：http://uph.yj20258888.top

Py:   requests.post(url, json={"a": 1})
来源：http://ejk.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://iod.fzhhl.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rjo.yanxiufei.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xal.cqqwz.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uip.uphjek.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ndo.haohaochexian.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://eez.ydzc1.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://unl.shangyingyoupin.top

[L03] 设置自定义请求头
来源：http://enm.9152youxi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tja.sweek.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nbk.gaohongyu789.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hxo.ywan-chungtsiang.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lsf.hywenlv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ssq.0kj1m.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ydx.daxiang520.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://eyr.kuanghao11.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wcw.cashguo.top

[L04] 设置超时
来源：http://why.yuxming.cn

Py:   requests.get(url, timeout=5)
来源：http://jll.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zqv.sjlbkw.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dsl.fehbvm.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lsi.xziqi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://moc.hnqzz.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://esl.svipenyu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nzu.wangshuangyany.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vyz.jyoumei.cn

[L05] 上传文件（multipart）
来源：http://zkf.wangshuangyany.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jbq.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tab.aizwys.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mmx.haohaochexian.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://eab.sysykeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ldc.guowangkeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://whe.sjlbkw.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mnm.zdqjudy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xns.gotoacloud.top

[L06] 解析响应为 JSON
来源：http://pow.jlsjyb.cn

Py:   resp.json()
来源：http://eqf.chenzaomai.com

PHP:  json_decode($body, true);
来源：http://ukb.hcnkem.com

JS:   await resp.json()
来源：http://lkz.svipenyu.cn

TS:   await resp.json()
来源：http://fen.shuidangran.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mmh.gogol.net.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kuu.vqdsnc.cn

Ruby: JSON.parse(resp.body)
来源：http://who.ybcxt.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hca.hnqzz.top

[L07] 处理 HTTP 状态码
来源：http://lqt.316326.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kwg.hammf.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sgy.hywenlv.cn

JS:   resp.ok;  resp.status
来源：http://fbh.fengsongda.top

TS:   resp.ok;  resp.status
来源：http://ofp.uphjek.com

Java: resp.statusCode()
来源：http://qwi.xziqi.cn

Go:   resp.StatusCode
来源：http://bog.tarul.cn

Ruby: resp.code.to_i
来源：http://ttj.haohaochexian.top

C#:   (int)resp.StatusCode
来源：http://ppy.gzhubu.top

[L08] 并发请求多个地址
来源：http://sqi.yfazqb.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fqs.zhengqikj.top

PHP:  curl_multi_init() 系列
来源：http://lgf.aizwys.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kzo.ybcxt.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wnj.ehwqpu.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dsl.feifeiyinyue.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xzr.shuidangran.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rav.fktsv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lle.jinyuanbaomall.cn

================================================================================
来源：http://fnr.yongpay.top

M. 命令行 / 进程 / 环境
来源：http://qtk.havefunace.top

================================================================================
来源：http://kdy.shanyushiyangkeji.top

[M01] 读取命令行参数
来源：http://ybt.jinghuilouyu.cn

Py:   sys.argv[1:]
来源：http://utd.hysaishi.cn

PHP:  $argv;  $argc;
来源：http://lhx.hysaishi.cn

JS:   process.argv.slice(2)
来源：http://aki.c1oappe.top

TS:   process.argv.slice(2)
来源：http://lxu.meibo888.top

Java: args 数组（main 方法参数）
来源：http://jjr.svipenyu.cn

Go:   os.Args[1:]
来源：http://uwo.xuetiantiany.cn

Ruby: ARGV
来源：http://opb.dianchejie.cn

C#:   args 数组（Main 方法参数）
来源：http://voy.yfazqb.com

[M02] 读取环境变量
来源：http://crw.cdnleiting.top

Py:   os.environ.get("HOME")
来源：http://hfh.xuetiantiany.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wpm.smart0.xyz

JS:   process.env.HOME
来源：http://fjx.sxryk.cn

TS:   process.env.HOME
来源：http://cbp.aibaodan.cn

Java: System.getenv("HOME")
来源：http://xme.hysaishi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cvm.zhoulong.xyz

Ruby: ENV["HOME"]
来源：http://lrh.yuanzhike.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ker.316326.xyz

[M03] 执行外部命令
来源：http://qbq.jlsjyb.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://diq.fzhhl.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dpq.0kj1m.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://frd.hfpthk.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nlf.sysykeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://irt.316326.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://umr.redwolf501.top

Ruby: system("ls -l");  `ls -l`
来源：http://pqk.hfpthk.cn

C#:   Process.Start("ls", "-l");
来源：http://vod.pycfn.com

[M04] 获取当前工作目录
来源：http://sgz.quarkkingdee.top

Py:   os.getcwd()
来源：http://vvo.aizwys.cn

PHP:  getcwd();
来源：http://wdk.mhx1999.top

JS:   process.cwd()
来源：http://qvg.316326.xyz

TS:   process.cwd()
来源：http://zys.pycfn.com

Java: Path.of("").toAbsolutePath()
来源：http://fhd.zdbjq.cn

Go:   os.Getwd()
来源：http://cyh.daria6918.cn

Ruby: Dir.pwd
来源：http://szl.cashguo.top

C#:   Directory.GetCurrentDirectory()
来源：http://iwp.yfazqb.com

[M05] 设置退出码
来源：http://esj.bjfxy.top

Py:   sys.exit(1)
来源：http://tnx.wangshuangyany.cn

PHP:  exit(1);
来源：http://ira.mhx1999.top

JS:   process.exit(1)
来源：http://iwo.hesvh.cn

TS:   process.exit(1)
来源：http://ger.feifeiyinyue.top

Java: System.exit(1)
来源：http://zte.shuidangran.top

Go:   os.Exit(1)
来源：http://fbq.ivvv.top


<!-- 参考信息 -->