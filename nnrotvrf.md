代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rko.zdqjudy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qzu.dianchejie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dli.gogol.net.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://sih.jyoumei.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qfa.xuanzx.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://eye.feifeiyinyue.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dvx.ivvv.top

================================================================================
来源：http://izv.ctjpmb.com

J. 日期与时间
来源：http://gpr.dianchejie.cn

================================================================================
来源：http://vwj.ydzc1.top

[J01] 获取当前时间
来源：http://lwb.cdnleiting.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://rzo.svipenyu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tdy.hnxiangtu.top

JS:   new Date();  Date.now()
来源：http://koz.tarul.cn

TS:   new Date();  Date.now()
来源：http://gxt.kuanghao11.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kdi.hesvh.cn

Go:   time.Now()
来源：http://qow.ivvv.top

Ruby: Time.now
来源：http://ygu.svipenyu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rgi.jinqigfzy.top

[J02] 格式化输出
来源：http://imy.0kj1m.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ccg.andypj.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wue.hcnkem.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lmw.yueranfly.top

TS:   d.toISOString()
来源：http://oil.bjfxy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jws.cheryme.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lce.cashguo.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pri.birdmap.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yld.wangshuangyany.cn

[J03] 字符串解析为日期
来源：http://ecn.52xcode.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ytu.gaohongyu789.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hgy.fanxiaobao.xyz

JS:   new Date("2024-01-02")
来源：http://jcn.nwbrower.top

TS:   new Date("2024-01-02")
来源：http://aor.jinqigfzy.top

Java: LocalDate.parse("2024-01-02")
来源：http://ktj.gogol.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://crq.ybcxt.top

Ruby: Date.parse("2024-01-02")
来源：http://vgy.hongshengwenyu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vgr.yuanzhike.top

[J04] 时间戳与日期互转
来源：http://ery.vehdjk.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fpf.316326.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gzy.zdqjudy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://twh.daria6918.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://esu.vqdsnc.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://udi.fktsv.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pdg.zhaomingkeji.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://npq.nwbrower.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yjf.kuanghao11.cn

[J05] 时间加减（加 7 天）
来源：http://dyv.dianchejie.cn

Py:   now + timedelta(days=7)
来源：http://dry.jinqigfzy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://fdo.fengsongda.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://emq.jqgfzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://iew.ivvv.top

Java: LocalDate.now().plusDays(7)
来源：http://rbr.fehbvm.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://azg.daxiang520.top

Ruby: Time.now + 7 * 86400
来源：http://vpr.chenjidiqi.icu

C#:   DateTime.Now.AddDays(7)
来源：http://ynp.tanke756.top

[J06] 计算两时间之差
来源：http://ubk.redwolf501.top

Py:   (end - start).total_seconds()
来源：http://zmw.shangyingyoupin.top

PHP:  $end->diff($start)->days;
来源：http://gtv.zhoulong.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ibw.xylfe.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wwq.cdnleiting.top

Java: Duration.between(start, end).toSeconds()
来源：http://hba.vehdjk.com

Go:   end.Sub(start).Hours()
来源：http://kkb.aizwys.cn

Ruby: end - start                 # 返回秒数
来源：http://dzm.vqdsnc.cn

C#:   (end - start).TotalSeconds
来源：http://cpq.havefunace.top

[J07] 比较两个日期
来源：http://yme.zhaomingkeji.xyz

Py:   d1 < d2;  d1 == d2
来源：http://pvq.zhiwuduotai.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mtg.sweek.top

JS:   d1.getTime() < d2.getTime()
来源：http://zaa.sufxvd.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hjw.quarkkingdee.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jih.tian-w.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lii.zdbjq.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zyz.ctjpmb.com

C#:   d1 < d2;  d1 == d2
来源：http://gah.zhoulong.xyz

[J08] 提取年月日与星期
来源：http://fin.jiagoushi.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wty.shanyushiyangtech.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qjw.fzhhl.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tjw.xuanzx.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lek.jinqigufen.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xne.aizwys.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cuf.xuetiantiany.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uux.hnxiangtu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ggi.shzxlz.cn

[J09] 时区处理
来源：http://oiq.jinyuanbaomall.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pob.quarkkingdee.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hcl.vehdjk.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nye.gotoacloud.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cxz.epnwcf.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ark.bbcook.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lhq.zhongyouzk.top

Ruby: Time.now.getlocal("+08:00")
来源：http://nst.zdqjudy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rkb.xylfe.cn

[J10] 取今天 / 本月第一天
来源：http://kpb.fehbvm.com

Py:   date.today();  date.today().replace(day=1)
来源：http://zva.guowangkeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kms.ctjpmb.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xbd.chenjidiqi.icu

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://swk.gogol.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jdu.fzhhl.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fyl.chenlongwang.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pkk.cashguo.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://agk.xuetiantiany.cn

================================================================================
来源：http://gsk.nwbrower.top

K. JSON 与序列化
来源：http://tat.zhengqikj.top

================================================================================
来源：http://edf.jlsjyb.cn

[K01] 对象转 JSON 字符串
来源：http://iuh.bbcook.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://evf.jqgfzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lzn.jqgufenzy.top

JS:   JSON.stringify(obj)
来源：http://mur.fengsongda.top

TS:   JSON.stringify(obj)
来源：http://tzh.yongpay.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mgy.fehbvm.com

Go:   json.Marshal(obj)
来源：http://vrn.zhaomingkeji.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://pcn.ywan-chungtsiang.top

C#:   JsonSerializer.Serialize(obj)
来源：http://qgg.wangshuangyany.cn

[K02] JSON 字符串转对象
来源：http://cwa.gotoacloud.top

Py:   json.loads(s)
来源：http://osu.guowangkeji.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mfj.guowangkeji.top

JS:   JSON.parse(s)
来源：http://jme.gaohongyu789.top

TS:   JSON.parse(s)
来源：http://sal.jinghuilouyu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fyh.jqgfzy.top

Go:   json.Unmarshal(data, &v)
来源：http://lae.ybcxt.top

Ruby: JSON.parse(s)
来源：http://egr.yuxming.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gsd.fengsongda.top

[K03] JSON 美化输出（带缩进）
来源：http://oga.sysykeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ctc.uphjek.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gtj.fzhhl.top

JS:   JSON.stringify(obj, null, 2)
来源：http://nka.svipenyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fwh.jqgfzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://deu.guowangkeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rof.jianghu66.top

Ruby: JSON.pretty_generate(obj)
来源：http://qxk.feifeiyinyue.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pyw.pycfn.com

[K04] 读取 JSON 文件
来源：http://nwd.yonumen.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zer.cucudq.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vyy.gzhubu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kip.hysaishi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vfg.hywenlv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yds.fanxiaobao.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://osn.feifeiyinyue.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://svq.sweek.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wxp.tian-w.cn

[K05] 深拷贝对象
来源：http://nzd.bjfxy.top

Py:   copy.deepcopy(obj)
来源：http://ujx.shanyushiyangkeji.top

PHP:  unserialize(serialize($obj));
来源：http://gsb.sxryk.cn

JS:   structuredClone(obj)
来源：http://xcf.316326.xyz

TS:   structuredClone(obj)
来源：http://jxs.xziqi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xea.sufxvd.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pcy.ybcxt.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mwl.zhixingplan.top

C#:   // 序列化往返，或自定义 Clone
来源：http://byw.yuanzhike.top

[K06] 解析 URL 查询串
来源：http://vcb.xylfe.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://boh.xziqi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xnh.chenlongwang.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fdm.dianchejie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nor.xziqi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uby.xuetiantiany.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hyp.shanyushiyangtech.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uaa.smart0.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://prl.meibo888.top

[K07] 进制转换
来源：http://dvl.fengsongda.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qzt.hammf.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kzr.jyoumei.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cdq.hcnkem.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://apr.gotoacloud.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tnv.ctjpmb.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mbz.guowangkeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tbl.yfazqb.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hdu.snrcjt.cn

[K08] 二进制序列化（非 JSON）
来源：http://pmt.guowangkeji.top

Py:   pickle.dumps(obj)
来源：http://aar.jinqigufen.top

PHP:  serialize($obj);  unserialize($s);
来源：http://gnl.yongpay.top

JS:   v8.serialize(obj)        // Node
来源：http://alv.xziqi.cn

TS:   v8.serialize(obj)        // Node
来源：http://qyl.tarul.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://amn.bjfxy.top

Go:   encoding/gob
来源：http://tcf.dianchejie.cn

Ruby: Marshal.dump(obj)
来源：http://eaw.hnqzz.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ltg.tanke756.top

================================================================================
来源：http://een.hcnkem.com

L. 网络请求
来源：http://uzr.aizwys.cn

================================================================================
来源：http://eib.gaohongyu789.top

[L01] 发送 GET 请求
来源：http://qvo.yvedp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qxz.fktsv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bhr.yj20258.top

JS:   await fetch(url)
来源：http://sla.vehdjk.com

TS:   await fetch(url)
来源：http://iid.snrcjt.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cyf.dashuyun.cn

Go:   resp, err := http.Get(url)
来源：http://kaq.cucudq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://lcy.ctjpmb.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rps.yj20258.top

[L02] 发送 POST JSON
来源：http://zmp.tarul.cn

Py:   requests.post(url, json={"a": 1})
来源：http://erj.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uua.iojbl.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://byx.shzxlz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rmf.dianchejie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cup.guannengcc.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://aer.sweek.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dkj.sjlbkw.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xho.sufxvd.cn

[L03] 设置自定义请求头
来源：http://gpf.guowangkeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uom.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pxh.zhengqikj.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ohk.tian-w.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jit.316326.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yte.zhiwuduotai.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rue.tian-w.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hgz.jqgfzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uoi.redwolf501.top

[L04] 设置超时
来源：http://tzq.52xcode.cn

Py:   requests.get(url, timeout=5)
来源：http://txb.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ndv.epnwcf.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zzu.zhaomingkeji.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pnu.0kj1m.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cyx.sweek.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uvm.dianchejie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gmn.tianlin.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fro.svipenyu.cn

[L05] 上传文件（multipart）
来源：http://gwy.jyoumei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://agk.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dbz.chenjidiqi.icu

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ngn.xziqi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ror.hongshengwenyu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://akq.xziqi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yfo.xylfe.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mvi.haohaochexian.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tpy.shangyingyoupin.top

[L06] 解析响应为 JSON
来源：http://jas.yangfankeji.com

Py:   resp.json()
来源：http://abk.hcnkem.com

PHP:  json_decode($body, true);
来源：http://ooy.yangfankeji.com

JS:   await resp.json()
来源：http://pmm.tanke756.top

TS:   await resp.json()
来源：http://dcs.xziqi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ovp.wangdashe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gza.daxiang520.top

Ruby: JSON.parse(resp.body)
来源：http://dea.yj202588.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qhv.xinyue.icu

[L07] 处理 HTTP 状态码
来源：http://qje.xylfe.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://auf.jlsjyb.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dvf.yonumen.top

JS:   resp.ok;  resp.status
来源：http://lxx.ydjk.org.cn

TS:   resp.ok;  resp.status
来源：http://wsq.hywenlv.cn

Java: resp.statusCode()
来源：http://tvq.ybcxt.top

Go:   resp.StatusCode
来源：http://fts.fengsongda.top

Ruby: resp.code.to_i
来源：http://ehf.chenzaomai.com

C#:   (int)resp.StatusCode
来源：http://huy.fktsv.cn

[L08] 并发请求多个地址
来源：http://skl.zycfv.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vdb.xuetiantiany.cn

PHP:  curl_multi_init() 系列
来源：http://ufb.yonumen.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vlw.zhijiandao.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qal.tanke756.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kwa.vehdjk.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://smr.yonumen.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ant.yonumen.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lmv.hfpthk.cn

================================================================================
来源：http://tqp.bjfxy.top

M. 命令行 / 进程 / 环境
来源：http://wwt.gzhubu.top

================================================================================
来源：http://jrb.iojbl.cn

[M01] 读取命令行参数
来源：http://jeq.aizwys.cn

Py:   sys.argv[1:]
来源：http://utm.sufxvd.cn

PHP:  $argv;  $argc;
来源：http://wsc.iojbl.cn

JS:   process.argv.slice(2)
来源：http://jxd.fktsv.cn

TS:   process.argv.slice(2)
来源：http://uqa.shuidangran.top

Java: args 数组（main 方法参数）
来源：http://qhi.cheryme.top

Go:   os.Args[1:]
来源：http://fac.jinqigufen.top

Ruby: ARGV
来源：http://fgd.jlsjyb.cn

C#:   args 数组（Main 方法参数）
来源：http://vmn.meibo888.top

[M02] 读取环境变量
来源：http://ooh.jinqigufen.top

Py:   os.environ.get("HOME")
来源：http://mgh.sufxvd.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ukb.aibaodan.cn

JS:   process.env.HOME
来源：http://gun.fehbvm.com

TS:   process.env.HOME
来源：http://nys.xylfe.cn

Java: System.getenv("HOME")
来源：http://ylp.svipenyu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tnc.nanxinkj.top

Ruby: ENV["HOME"]
来源：http://wtw.tianlin.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tro.pycfn.com

[M03] 执行外部命令
来源：http://ctq.epnwcf.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kaf.ydzc1.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ech.ctjpmb.com

JS:   child_process.execSync("ls -l").toString()
来源：http://kmi.kuanghao11.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zci.tarul.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blu.aizwys.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://rfl.yonumen.top

Ruby: system("ls -l");  `ls -l`
来源：http://mfc.hammf.cn

C#:   Process.Start("ls", "-l");
来源：http://ohj.zhengqikj.top

[M04] 获取当前工作目录
来源：http://eit.ywan-chungtsiang.top

Py:   os.getcwd()
来源：http://jgf.sufxvd.cn

PHP:  getcwd();
来源：http://ccf.tarul.cn

JS:   process.cwd()
来源：http://pzl.mhx1999.top

TS:   process.cwd()
来源：http://has.dianchejie.cn

Java: Path.of("").toAbsolutePath()
来源：http://kna.pycfn.com

Go:   os.Getwd()
来源：http://qqa.yj202588.top

Ruby: Dir.pwd
来源：http://vyu.daria6918.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jrj.fzhhl.top

[M05] 设置退出码
来源：http://use.yongpay.top

Py:   sys.exit(1)
来源：http://cyp.yangfankeji.com

PHP:  exit(1);
来源：http://fqh.hnqzz.top

JS:   process.exit(1)
来源：http://pqq.wangshuangyany.cn

TS:   process.exit(1)
来源：http://nka.bjfxy.top

Java: System.exit(1)
来源：http://jpz.hfpthk.cn

Go:   os.Exit(1)
来源：http://grt.nanxinkj.top

Ruby: exit 1
来源：http://xca.guannengcc.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qls.jinyuanbaomall.cn

[M06] 向标准错误输出
来源：http://hkv.ydzc1.top

Py:   print("err", file=sys.stderr)
来源：http://apx.dashuyun.cn


<!-- 参考信息 -->