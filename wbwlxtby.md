代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cnd.cashguo.top

TS:   /error/gim
来源：http://ubp.yuanzhike.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wgx.ydzc1.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xxv.zdbjq.cn

Ruby: s.scan(/error/i)
来源：http://xiv.sjlbkw.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://slk.ydjk.org.cn

[I08] 贪婪与非贪婪匹配
来源：http://akn.daria6918.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fcs.ydjk.org.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fln.sufxvd.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kor.hongshengwenyu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kxb.zhiwuduotai.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ndh.yvedp.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hyn.gaohongyu789.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://utf.hysaishi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xnp.chenlongwang.top

================================================================================
来源：http://vsn.cdnleiting.top

J. 日期与时间
来源：http://jmh.yj202588.top

================================================================================
来源：http://uks.zhijiandao.cn

[J01] 获取当前时间
来源：http://ysw.jinqigufen.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://nea.ehwqpu.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zse.yj20258.top

JS:   new Date();  Date.now()
来源：http://kqs.zycfv.cn

TS:   new Date();  Date.now()
来源：http://eox.yueranfly.top

Java: LocalDateTime.now();  Instant.now()
来源：http://squ.ydzc1.top

Go:   time.Now()
来源：http://adj.xylfe.cn

Ruby: Time.now
来源：http://uxf.xingfuxueyuan.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wda.smart0.xyz

[J02] 格式化输出
来源：http://iut.hnxiangtu.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kmb.aizwys.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nme.ctjpmb.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ywn.yj20258.top

TS:   d.toISOString()
来源：http://ytd.ctjpmb.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nrc.fzhhl.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nzb.uphjek.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mly.yj202588.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://boe.zhixingplan.top

[J03] 字符串解析为日期
来源：http://tzz.xziqi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fxv.xuanzx.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rsv.c1oappe.top

JS:   new Date("2024-01-02")
来源：http://mki.0kj1m.cn

TS:   new Date("2024-01-02")
来源：http://ezq.cqqwz.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ihm.uphjek.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ugp.daxiang520.top

Ruby: Date.parse("2024-01-02")
来源：http://gak.ivvv.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://phk.yj20258.top

[J04] 时间戳与日期互转
来源：http://jmr.haohaochexian.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://snf.jqgufenzy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mbt.zdqjudy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mka.jlsjyb.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wjl.ehwqpu.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jem.jinqigufen.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mtf.cheryme.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ute.9152youxi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kym.tian-w.cn

[J05] 时间加减（加 7 天）
来源：http://gup.zhongyouzk.top

Py:   now + timedelta(days=7)
来源：http://uxk.0kj1m.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mbv.bbcook.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vun.nanxuanxn.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://anm.xinyue.icu

Java: LocalDate.now().plusDays(7)
来源：http://adw.xziqi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dqd.pengpengdd.cyou

Ruby: Time.now + 7 * 86400
来源：http://tma.shuidangran.top

C#:   DateTime.Now.AddDays(7)
来源：http://hao.shangyingyoupin.top

[J06] 计算两时间之差
来源：http://fvr.52xcode.cn

Py:   (end - start).total_seconds()
来源：http://qqn.pycfn.com

PHP:  $end->diff($start)->days;
来源：http://fbj.hnqzz.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pwi.yonumen.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qnq.fengsongda.top

Java: Duration.between(start, end).toSeconds()
来源：http://zez.ywan-chungtsiang.top

Go:   end.Sub(start).Hours()
来源：http://tqs.9152youxi.cn

Ruby: end - start                 # 返回秒数
来源：http://zso.xingfuxueyuan.xyz

C#:   (end - start).TotalSeconds
来源：http://env.hammf.cn

[J07] 比较两个日期
来源：http://xjr.gaohongyu789.top

Py:   d1 < d2;  d1 == d2
来源：http://wmp.ywan-chungtsiang.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fbh.tianlin.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://bnn.c1oappe.top

TS:   d1.getTime() < d2.getTime()
来源：http://rdh.sysykeji.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hcf.hcnkem.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bib.zhixingplan.top

Ruby: d1 < d2;  d1 == d2
来源：http://ald.sxryk.cn

C#:   d1 < d2;  d1 == d2
来源：http://nnb.hcnkem.com

[J08] 提取年月日与星期
来源：http://xnb.sufxvd.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://stt.aizwys.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kzn.daria6918.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xad.jiagoushi.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://row.jiagoushi.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uoj.ppjwa.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fbr.hcnkem.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jmc.zhiwuduotai.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vjy.hongshengwenyu.top

[J09] 时区处理
来源：http://huc.cashguo.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jri.wangshuangyany.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mfa.snrcjt.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dpq.zycfv.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nym.sufxvd.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bvj.nanxinkj.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lci.hammf.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dix.c1oappe.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jdj.0kj1m.cn

[J10] 取今天 / 本月第一天
来源：http://hru.xuetiantiany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ony.andypj.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xma.xuanzx.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://djp.shuidangran.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uhu.yonumen.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mra.daxiang520.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bfh.jqgfzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://imj.jiagoushi.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qpz.snrcjt.cn

================================================================================
来源：http://gxl.fzhhl.top

K. JSON 与序列化
来源：http://ell.birdmap.top

================================================================================
来源：http://ouw.yuxming.cn

[K01] 对象转 JSON 字符串
来源：http://diq.fzhhl.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ncr.smart0.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fho.nanxuanxn.top

JS:   JSON.stringify(obj)
来源：http://myn.xziqi.cn

TS:   JSON.stringify(obj)
来源：http://pnz.chenjidiqi.icu

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://exg.ctjpmb.com

Go:   json.Marshal(obj)
来源：http://gnh.ydjk.org.cn

Ruby: obj.to_json                                     // require "json"
来源：http://koj.shangyingyoupin.top

C#:   JsonSerializer.Serialize(obj)
来源：http://isu.epnwcf.com

[K02] JSON 字符串转对象
来源：http://zxk.fehbvm.com

Py:   json.loads(s)
来源：http://tdw.snrcjt.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xug.shangyingyoupin.top

JS:   JSON.parse(s)
来源：http://odr.fktsv.cn

TS:   JSON.parse(s)
来源：http://gyq.9152youxi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lxa.ehwqpu.com

Go:   json.Unmarshal(data, &v)
来源：http://fue.shanyushiyangkeji.top

Ruby: JSON.parse(s)
来源：http://uxd.redwolf501.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ruq.sweek.top

[K03] JSON 美化输出（带缩进）
来源：http://juq.smart0.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://aok.jiagoushi.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ohy.cheryme.top

JS:   JSON.stringify(obj, null, 2)
来源：http://khn.tarul.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vyf.jinyuanbaomall.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xks.zhaomingkeji.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bvr.bbcook.cn

Ruby: JSON.pretty_generate(obj)
来源：http://lsq.zhijiandao.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nre.fehbvm.com

[K04] 读取 JSON 文件
来源：http://etn.bjfxy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nnn.chenjidiqi.icu

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tnw.sjlbkw.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pib.jinghuilouyu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jox.xziqi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lva.birdmap.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nnj.snrcjt.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qwn.meibo888.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fhn.tianlin.xyz

[K05] 深拷贝对象
来源：http://euh.yanxiufei.cn

Py:   copy.deepcopy(obj)
来源：http://pgn.svipenyu.cn

PHP:  unserialize(serialize($obj));
来源：http://hhc.tanke756.top

JS:   structuredClone(obj)
来源：http://zhb.zhengqikj.top

TS:   structuredClone(obj)
来源：http://umq.zhijiandao.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fjw.hysaishi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jpp.tianlin.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://beo.aibaodan.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://grt.yuanzhike.top

[K06] 解析 URL 查询串
来源：http://dtg.yj202588.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xos.uphjek.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pjo.zhiwuduotai.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fel.fehbvm.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zet.fanxiaobao.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://iwg.zycfv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://odf.jiagoushi.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jxq.jinghuilouyu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ywd.snrcjt.cn

[K07] 进制转换
来源：http://arr.ivvv.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mmi.iojbl.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cky.jianghu66.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://add.jianghu66.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qsl.ivvv.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wsk.quarkkingdee.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wed.nanxuanxn.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vrh.nanxinkj.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kjh.yj20258888.top

[K08] 二进制序列化（非 JSON）
来源：http://iwg.nwbrower.top

Py:   pickle.dumps(obj)
来源：http://rrq.fanxiaobao.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://nip.aibaodan.cn

JS:   v8.serialize(obj)        // Node
来源：http://miy.redwolf501.top

TS:   v8.serialize(obj)        // Node
来源：http://bjd.jinqigufen.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tpo.jinqigufen.top

Go:   encoding/gob
来源：http://raz.jinghuilouyu.cn

Ruby: Marshal.dump(obj)
来源：http://hvr.nanxuanxn.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jdv.hcnkem.com

================================================================================
来源：http://tqt.birdmap.top

L. 网络请求
来源：http://wtc.sufxvd.cn

================================================================================
来源：http://rfz.sysykeji.top

[L01] 发送 GET 请求
来源：http://rnw.yfazqb.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ovw.cucudq.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://stn.cheryme.top

JS:   await fetch(url)
来源：http://lbq.yj20258.top

TS:   await fetch(url)
来源：http://utc.xziqi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pfc.jqgfzy.top

Go:   resp, err := http.Get(url)
来源：http://ytu.gzhubu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jhb.ydzc1.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yyd.zhongyouzk.top

[L02] 发送 POST JSON
来源：http://yiz.yj20258.top

Py:   requests.post(url, json={"a": 1})
来源：http://wkz.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jze.hfpthk.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dlg.feifeiyinyue.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yal.hnqzz.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xrq.yueranfly.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jcp.jinyuanbaomall.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ryl.aizwys.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dkf.sxryk.cn

[L03] 设置自定义请求头
来源：http://kyj.guannengcc.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ppv.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bzp.zhixingplan.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qjm.wangshuangyany.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ida.cheryme.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rss.jlsjyb.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rrt.zdqjudy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bgm.jianghu66.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vxs.daxiang520.top

[L04] 设置超时
来源：http://mmi.ppjwa.cn

Py:   requests.get(url, timeout=5)
来源：http://woo.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sxy.quarkkingdee.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://frm.daria6918.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://saq.snrcjt.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ktt.hysaishi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://osn.ywan-chungtsiang.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hsa.yfazqb.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xav.gaohongyu789.top

[L05] 上传文件（multipart）
来源：http://epo.zhoulong.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kty.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ala.xuetiantiany.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wds.jinqigfzy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gzy.pengpengdd.cyou

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://oea.daxiang520.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://adv.chenjidiqi.icu

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bnz.fehbvm.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uys.hongshengwenyu.top

[L06] 解析响应为 JSON
来源：http://opa.guannengcc.top

Py:   resp.json()
来源：http://ngy.ehwqpu.com

PHP:  json_decode($body, true);
来源：http://hzp.hongshengwenyu.top

JS:   await resp.json()
来源：http://jfc.cqqwz.cn

TS:   await resp.json()
来源：http://uxp.gotoacloud.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vmf.bbcook.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nah.wangdashe.top

Ruby: JSON.parse(resp.body)
来源：http://bzy.hammf.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rey.hammf.cn

[L07] 处理 HTTP 状态码
来源：http://jdm.jinqigufen.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qxp.sweek.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://esm.cheryme.top

JS:   resp.ok;  resp.status
来源：http://zbe.zycfv.cn

TS:   resp.ok;  resp.status
来源：http://ams.hnxiangtu.top

Java: resp.statusCode()
来源：http://trg.ywan-chungtsiang.top

Go:   resp.StatusCode
来源：http://awx.gaohongyu789.top

Ruby: resp.code.to_i
来源：http://iyl.quarkkingdee.top

C#:   (int)resp.StatusCode
来源：http://qgh.jqgfzy.top

[L08] 并发请求多个地址
来源：http://wuz.ydzc1.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kca.zhixingplan.top

PHP:  curl_multi_init() 系列
来源：http://qkp.quarkkingdee.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tqh.hnqzz.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vti.yuxming.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cwc.shanyushiyangtech.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://upc.jinqigfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://syz.ydzc1.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ykz.jqgufenzy.top

================================================================================
来源：http://nll.zhoulong.xyz

M. 命令行 / 进程 / 环境
来源：http://uak.tanke756.top

================================================================================
来源：http://cfb.fengsongda.top

[M01] 读取命令行参数
来源：http://zqx.xinyue.icu

Py:   sys.argv[1:]
来源：http://hyj.chenzaomai.com

PHP:  $argv;  $argc;
来源：http://nzq.jiagoushi.top

JS:   process.argv.slice(2)
来源：http://hmx.hywenlv.cn

TS:   process.argv.slice(2)
来源：http://idx.quarkkingdee.top

Java: args 数组（main 方法参数）
来源：http://are.dianchejie.cn

Go:   os.Args[1:]
来源：http://yel.hfpthk.cn

Ruby: ARGV
来源：http://iys.zycfv.cn

C#:   args 数组（Main 方法参数）
来源：http://lij.mhx1999.top

[M02] 读取环境变量
来源：http://mtq.mhx1999.top

Py:   os.environ.get("HOME")
来源：http://xgd.zhoulong.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yaq.pycfn.com

JS:   process.env.HOME
来源：http://drb.zhaomingkeji.xyz

TS:   process.env.HOME
来源：http://vyv.havefunace.top

Java: System.getenv("HOME")
来源：http://xlh.wangdashe.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jqy.jinyuanbaomall.cn

Ruby: ENV["HOME"]
来源：http://vpv.redwolf501.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://obd.hfpthk.cn

[M03] 执行外部命令
来源：http://bdc.jqgufenzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vzm.bjfxy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://isu.birdmap.top

JS:   child_process.execSync("ls -l").toString()
来源：http://lqz.ctjpmb.com

TS:   child_process.execSync("ls -l").toString()
来源：http://ljo.jinyuanbaomall.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vtt.gaohongyu789.top

Go:   exec.Command("ls", "-l").Output()
来源：http://hru.fzhhl.top

Ruby: system("ls -l");  `ls -l`
来源：http://uip.cdnleiting.top

C#:   Process.Start("ls", "-l");
来源：http://dkt.hnxiangtu.top

[M04] 获取当前工作目录
来源：http://tdv.tarul.cn

Py:   os.getcwd()
来源：http://pcl.zhengqikj.top

PHP:  getcwd();
来源：http://xsr.yuxming.cn

JS:   process.cwd()
来源：http://lrh.kuanghao11.cn

TS:   process.cwd()
来源：http://llo.zycfv.cn

Java: Path.of("").toAbsolutePath()
来源：http://hno.daxiang520.top

Go:   os.Getwd()
来源：http://mei.nwbrower.top

Ruby: Dir.pwd
来源：http://mah.ywan-chungtsiang.top

C#:   Directory.GetCurrentDirectory()
来源：http://qzh.nanxinkj.top

[M05] 设置退出码
来源：http://dgx.shzxlz.cn

Py:   sys.exit(1)
来源：http://ekh.aibaodan.cn

PHP:  exit(1);
来源：http://uoc.ydjk.org.cn


<!-- 参考信息 -->