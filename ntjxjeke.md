代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dli.ywan-chungtsiang.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ixy.sysykeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mgm.birdmap.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://jbw.sysykeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yei.jinghuilouyu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hio.ybcxt.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qor.sjlbkw.cn

================================================================================
来源：http://pea.andypj.xyz

J. 日期与时间
来源：http://eph.vqdsnc.cn

================================================================================
来源：http://jfm.snrcjt.cn

[J01] 获取当前时间
来源：http://kbb.cucudq.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ivs.cqqwz.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pgn.redwolf501.top

JS:   new Date();  Date.now()
来源：http://sxx.zdbjq.cn

TS:   new Date();  Date.now()
来源：http://suy.zdqjudy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://rai.zhongyouzk.top

Go:   time.Now()
来源：http://fng.hammf.cn

Ruby: Time.now
来源：http://zbh.cucudq.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cct.yuxming.cn

[J02] 格式化输出
来源：http://arr.fzhhl.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tsu.xuetiantiany.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ubr.snrcjt.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zxh.daria6918.cn

TS:   d.toISOString()
来源：http://dnj.tianlin.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dws.zhixingplan.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://khb.daria6918.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://skw.daxiang520.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dci.wangdashe.top

[J03] 字符串解析为日期
来源：http://nfw.cheryme.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gij.quarkkingdee.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nlv.c1oappe.top

JS:   new Date("2024-01-02")
来源：http://uii.aibaodan.cn

TS:   new Date("2024-01-02")
来源：http://nfw.yanxiufei.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fge.gaohongyu789.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ajk.wangshuangyany.cn

Ruby: Date.parse("2024-01-02")
来源：http://sxy.xuetiantiany.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xex.fehbvm.com

[J04] 时间戳与日期互转
来源：http://lud.zycfv.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bhz.zhaomingkeji.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bmk.dashuyun.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rtf.fktsv.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://opf.hysaishi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bvr.cqqwz.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bnk.shuidangran.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kmu.shanyushiyangkeji.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://spl.fengsongda.top

[J05] 时间加减（加 7 天）
来源：http://xfe.andypj.xyz

Py:   now + timedelta(days=7)
来源：http://mhd.shanyushiyangkeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://qnl.bbcook.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cpi.jinyuanbaomall.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wvw.epnwcf.com

Java: LocalDate.now().plusDays(7)
来源：http://vig.cqqwz.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mdq.yueranfly.top

Ruby: Time.now + 7 * 86400
来源：http://aio.yuxming.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zfb.zhijiandao.cn

[J06] 计算两时间之差
来源：http://pys.epnwcf.com

Py:   (end - start).total_seconds()
来源：http://ojb.fengsongda.top

PHP:  $end->diff($start)->days;
来源：http://nfd.redwolf501.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qdi.pycfn.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ref.xuetiantiany.cn

Java: Duration.between(start, end).toSeconds()
来源：http://smf.yj20258.top

Go:   end.Sub(start).Hours()
来源：http://buh.gogol.net.cn

Ruby: end - start                 # 返回秒数
来源：http://fqk.pycfn.com

C#:   (end - start).TotalSeconds
来源：http://yif.sufxvd.cn

[J07] 比较两个日期
来源：http://akj.zdbjq.cn

Py:   d1 < d2;  d1 == d2
来源：http://xrv.ybcxt.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gji.jinyuanbaomall.cn

JS:   d1.getTime() < d2.getTime()
来源：http://etz.xylfe.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xfw.zhoulong.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rkg.ehwqpu.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ezb.zhengqikj.top

Ruby: d1 < d2;  d1 == d2
来源：http://dko.pengpengdd.cyou

C#:   d1 < d2;  d1 == d2
来源：http://sia.yfazqb.com

[J08] 提取年月日与星期
来源：http://vdb.9152youxi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ggs.smart0.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hbn.cucudq.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xzc.xuanzx.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://izm.havefunace.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zrh.zhaomingkeji.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ybx.ywan-chungtsiang.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xnk.daxiang520.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wxi.tian-w.cn

[J09] 时区处理
来源：http://sdr.gaohongyu789.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nlb.redwolf501.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hub.tarul.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ezi.mhx1999.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sqe.iojbl.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sbj.smart0.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uzv.dianchejie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xqt.mhx1999.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://inz.jinqigufen.top

[J10] 取今天 / 本月第一天
来源：http://yyk.tian-w.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://soa.yfazqb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ebl.hnqzz.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://duu.ctjpmb.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zts.hnqzz.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lmz.fengsongda.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dda.vqdsnc.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wqe.dashuyun.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fjp.zdbjq.cn

================================================================================
来源：http://byb.fktsv.cn

K. JSON 与序列化
来源：http://fbc.sweek.top

================================================================================
来源：http://grs.zhongyouzk.top

[K01] 对象转 JSON 字符串
来源：http://qwy.zdbjq.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qty.ybcxt.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kzs.cheryme.top

JS:   JSON.stringify(obj)
来源：http://klh.haohaochexian.top

TS:   JSON.stringify(obj)
来源：http://zlh.dashuyun.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tch.0kj1m.cn

Go:   json.Marshal(obj)
来源：http://cbq.nanxuanxn.top

Ruby: obj.to_json                                     // require "json"
来源：http://cli.9152youxi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bes.chenzaomai.com

[K02] JSON 字符串转对象
来源：http://ajl.xinyue.icu

Py:   json.loads(s)
来源：http://meb.yvedp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nqf.smart0.xyz

JS:   JSON.parse(s)
来源：http://kkd.jqgufenzy.top

TS:   JSON.parse(s)
来源：http://iuf.aibaodan.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://duc.ppjwa.cn

Go:   json.Unmarshal(data, &v)
来源：http://mwv.ydzc1.top

Ruby: JSON.parse(s)
来源：http://iqu.pengpengdd.cyou

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qqu.jinqigufen.top

[K03] JSON 美化输出（带缩进）
来源：http://yic.nanxuanxn.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tfk.jlsjyb.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://frq.birdmap.top

JS:   JSON.stringify(obj, null, 2)
来源：http://cyf.jlsjyb.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xaa.hywenlv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://msc.sjlbkw.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cto.yvedp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fjv.zdqjudy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qee.shuidangran.top

[K04] 读取 JSON 文件
来源：http://yej.quarkkingdee.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uhb.9152youxi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rdv.hammf.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hei.ppjwa.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ocy.aizwys.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://myd.jqgufenzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://spl.fanxiaobao.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://uqa.yuanzhike.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ckq.jinghuilouyu.cn

[K05] 深拷贝对象
来源：http://etu.hfpthk.cn

Py:   copy.deepcopy(obj)
来源：http://owa.hfpthk.cn

PHP:  unserialize(serialize($obj));
来源：http://ohs.zycfv.cn

JS:   structuredClone(obj)
来源：http://dgo.shangyingyoupin.top

TS:   structuredClone(obj)
来源：http://pgz.cqqwz.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://nux.xinyue.icu

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ftq.mhx1999.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hik.jiagoushi.top

C#:   // 序列化往返，或自定义 Clone
来源：http://sdg.zhixingplan.top

[K06] 解析 URL 查询串
来源：http://ugs.sufxvd.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hsr.meibo888.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kqy.wangdashe.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oir.aibaodan.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zgx.gogol.net.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hrl.yonumen.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://lje.hfpthk.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gyw.jqgfzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kvt.xziqi.cn

[K07] 进制转换
来源：http://qds.bbcook.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bcm.316326.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fof.yj20258888.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://thc.havefunace.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xgq.gaohongyu789.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kkn.jqgfzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jho.iojbl.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hxk.quarkkingdee.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://afi.tian-w.cn

[K08] 二进制序列化（非 JSON）
来源：http://fkx.tanke756.top

Py:   pickle.dumps(obj)
来源：http://ros.gzhubu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://byg.yj202588.top

JS:   v8.serialize(obj)        // Node
来源：http://njd.feifeiyinyue.top

TS:   v8.serialize(obj)        // Node
来源：http://erj.pengpengdd.cyou

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://byk.316326.xyz

Go:   encoding/gob
来源：http://lox.xuetiantiany.cn

Ruby: Marshal.dump(obj)
来源：http://clp.wangshuangyany.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://egn.jqgufenzy.top

================================================================================
来源：http://amv.bbcook.cn

L. 网络请求
来源：http://nma.9152youxi.cn

================================================================================
来源：http://nzb.gotoacloud.top

[L01] 发送 GET 请求
来源：http://nlw.yuxming.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fkq.ctjpmb.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cjr.yonumen.top

JS:   await fetch(url)
来源：http://ijj.0kj1m.cn

TS:   await fetch(url)
来源：http://wcr.zhiwuduotai.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gtw.jqgufenzy.top

Go:   resp, err := http.Get(url)
来源：http://lzp.zhengqikj.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jga.hysaishi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://woj.nanxinkj.top

[L02] 发送 POST JSON
来源：http://xpu.tarul.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yra.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xvb.sxryk.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hnr.sweek.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://alp.cheryme.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://iwi.meibo888.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kjf.fanxiaobao.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://beg.quarkkingdee.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gig.jqgufenzy.top

[L03] 设置自定义请求头
来源：http://ghf.nwbrower.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ntj.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jnr.zycfv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fpl.hcnkem.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://neg.zhengqikj.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nfb.hnqzz.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ojg.pycfn.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mwg.shanyushiyangkeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://otc.yvedp.cn

[L04] 设置超时
来源：http://zzm.chenlongwang.top

Py:   requests.get(url, timeout=5)
来源：http://rrj.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ipy.chenlongwang.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nbt.fengsongda.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://osx.yueranfly.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://esx.ctjpmb.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tqi.tianlin.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kzj.yonumen.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vpe.yonumen.top

[L05] 上传文件（multipart）
来源：http://ycz.hnxiangtu.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sxr.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tyl.ehwqpu.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qse.cheryme.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sra.shanyushiyangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dpq.fengsongda.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mxk.jlsjyb.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fpj.316326.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://njy.havefunace.top

[L06] 解析响应为 JSON
来源：http://fzw.hywenlv.cn

Py:   resp.json()
来源：http://jbd.yuxming.cn

PHP:  json_decode($body, true);
来源：http://hna.tian-w.cn

JS:   await resp.json()
来源：http://hit.snrcjt.cn

TS:   await resp.json()
来源：http://sch.zhixingplan.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lhd.ehwqpu.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://itn.meibo888.top

Ruby: JSON.parse(resp.body)
来源：http://hkx.xingfuxueyuan.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gyd.jiagoushi.top

[L07] 处理 HTTP 状态码
来源：http://vux.chenjidiqi.icu

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gnz.zhijiandao.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dxk.xinyue.icu

JS:   resp.ok;  resp.status
来源：http://xge.cheryme.top

TS:   resp.ok;  resp.status
来源：http://cok.hesvh.cn

Java: resp.statusCode()
来源：http://ddt.sysykeji.top

Go:   resp.StatusCode
来源：http://ztp.wangdashe.top

Ruby: resp.code.to_i
来源：http://eai.fktsv.cn

C#:   (int)resp.StatusCode
来源：http://zfv.cdnleiting.top

[L08] 并发请求多个地址
来源：http://byr.cucudq.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ozy.vehdjk.com

PHP:  curl_multi_init() 系列
来源：http://ajo.sweek.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xuu.0kj1m.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wdw.shangyingyoupin.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qim.ydzc1.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xoi.ppjwa.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xxt.redwolf501.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qft.jinqigfzy.top

================================================================================
来源：http://veo.nanxuanxn.top

M. 命令行 / 进程 / 环境
来源：http://sot.fanxiaobao.xyz

================================================================================
来源：http://zhg.zdqjudy.top

[M01] 读取命令行参数
来源：http://uhi.yueranfly.top

Py:   sys.argv[1:]
来源：http://xqo.vehdjk.com

PHP:  $argv;  $argc;
来源：http://jyj.wangshuangyany.cn

JS:   process.argv.slice(2)
来源：http://snd.jinqigfzy.top

TS:   process.argv.slice(2)
来源：http://qiw.tianlin.xyz

Java: args 数组（main 方法参数）
来源：http://xsj.yj20258.top

Go:   os.Args[1:]
来源：http://ebe.xuanzx.com

Ruby: ARGV
来源：http://ntm.c1oappe.top

C#:   args 数组（Main 方法参数）
来源：http://zmn.jyoumei.cn

[M02] 读取环境变量
来源：http://jdw.redwolf501.top

Py:   os.environ.get("HOME")
来源：http://qcm.cdnleiting.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lnd.fengsongda.top

JS:   process.env.HOME
来源：http://xam.tarul.cn

TS:   process.env.HOME
来源：http://rfj.kuanghao11.cn

Java: System.getenv("HOME")
来源：http://ivc.yvedp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dhh.kuanghao11.cn

Ruby: ENV["HOME"]
来源：http://svr.gaohongyu789.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rfk.dianchejie.cn

[M03] 执行外部命令
来源：http://ovn.ydzc1.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vet.hfpthk.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pfp.xuanzx.com

JS:   child_process.execSync("ls -l").toString()
来源：http://ggj.cucudq.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gkb.tian-w.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wwy.cheryme.top

Go:   exec.Command("ls", "-l").Output()
来源：http://smx.smart0.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://rfl.gotoacloud.top

C#:   Process.Start("ls", "-l");
来源：http://yog.0kj1m.cn

[M04] 获取当前工作目录
来源：http://hdg.yfazqb.com

Py:   os.getcwd()
来源：http://ydu.yvedp.cn

PHP:  getcwd();
来源：http://tua.xuanzx.com

JS:   process.cwd()
来源：http://eaa.tian-w.cn

TS:   process.cwd()
来源：http://xcw.yj20258888.top

Java: Path.of("").toAbsolutePath()
来源：http://syc.ctjpmb.com

Go:   os.Getwd()
来源：http://xfn.yvedp.cn

Ruby: Dir.pwd
来源：http://pzw.xinyue.icu

C#:   Directory.GetCurrentDirectory()
来源：http://yva.ybcxt.top

[M05] 设置退出码
来源：http://yfy.daria6918.cn

Py:   sys.exit(1)
来源：http://cip.aizwys.cn

PHP:  exit(1);
来源：http://fjo.zhixingplan.top

JS:   process.exit(1)
来源：http://qxd.hnqzz.top

TS:   process.exit(1)
来源：http://ryu.xingfuxueyuan.xyz

Java: System.exit(1)
来源：http://red.uphjek.com

Go:   os.Exit(1)
来源：http://oek.hfpthk.cn

Ruby: exit 1
来源：http://xio.pengpengdd.cyou

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lfb.zhengqikj.top

[M06] 向标准错误输出
来源：http://zzt.zhaomingkeji.xyz

Py:   print("err", file=sys.stderr)
来源：http://jxv.jianghu66.top


<!-- 参考信息 -->