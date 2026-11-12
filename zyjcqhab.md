代发 wailian999

J. 日期与时间
来源：http://ekn.zhoulong.xyz

================================================================================
来源：http://kxv.ywan-chungtsiang.top

[J01] 获取当前时间
来源：http://yyw.snrcjt.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kvu.hongshengwenyu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://won.pengpengdd.cyou

JS:   new Date();  Date.now()
来源：http://fyy.sweek.top

TS:   new Date();  Date.now()
来源：http://pus.zdbjq.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wjj.yongpay.top

Go:   time.Now()
来源：http://ipd.hammf.cn

Ruby: Time.now
来源：http://vwo.cucudq.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fvf.zhiwuduotai.top

[J02] 格式化输出
来源：http://yjs.zhongyouzk.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yhl.cashguo.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nby.zhijiandao.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mlz.hnqzz.top

TS:   d.toISOString()
来源：http://bvc.bbcook.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fab.shzxlz.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wkp.fzhhl.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://anf.sjlbkw.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dqg.iojbl.cn

[J03] 字符串解析为日期
来源：http://swc.cucudq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://oob.gzhubu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://exq.hongshengwenyu.top

JS:   new Date("2024-01-02")
来源：http://ccs.shzxlz.cn

TS:   new Date("2024-01-02")
来源：http://cvq.chenlongwang.top

Java: LocalDate.parse("2024-01-02")
来源：http://mjp.gogol.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rdd.bjfxy.top

Ruby: Date.parse("2024-01-02")
来源：http://eel.mhx1999.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lyk.zhongyouzk.top

[J04] 时间戳与日期互转
来源：http://pjd.yj20258888.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fzj.andypj.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cvy.hfpthk.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tnx.yuanzhike.top

TS:   Math.floor(Date.now() / 1000)
来源：http://qor.smart0.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mhf.0kj1m.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sge.vehdjk.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rcd.cdnleiting.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://eev.jianghu66.top

[J05] 时间加减（加 7 天）
来源：http://xal.fanxiaobao.xyz

Py:   now + timedelta(days=7)
来源：http://dry.redwolf501.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://jxr.ehwqpu.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pgc.jiagoushi.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uzt.wangshuangyany.cn

Java: LocalDate.now().plusDays(7)
来源：http://dkk.xziqi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://smv.guannengcc.top

Ruby: Time.now + 7 * 86400
来源：http://ggj.andypj.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://zry.nwbrower.top

[J06] 计算两时间之差
来源：http://ert.xuanzx.com

Py:   (end - start).total_seconds()
来源：http://vcz.pycfn.com

PHP:  $end->diff($start)->days;
来源：http://deq.yonumen.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dgz.shuidangran.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wjy.shanyushiyangtech.top

Java: Duration.between(start, end).toSeconds()
来源：http://bsl.jlsjyb.cn

Go:   end.Sub(start).Hours()
来源：http://aes.cheryme.top

Ruby: end - start                 # 返回秒数
来源：http://ysc.jiagoushi.top

C#:   (end - start).TotalSeconds
来源：http://gyc.shanyushiyangkeji.top

[J07] 比较两个日期
来源：http://cuk.aizwys.cn

Py:   d1 < d2;  d1 == d2
来源：http://bqn.yfazqb.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zec.zhengqikj.top

JS:   d1.getTime() < d2.getTime()
来源：http://qkn.jinqigufen.top

TS:   d1.getTime() < d2.getTime()
来源：http://hvc.jiagoushi.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pco.52xcode.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://oda.iojbl.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ads.cqqwz.cn

C#:   d1 < d2;  d1 == d2
来源：http://rpw.yj20258.top

[J08] 提取年月日与星期
来源：http://eow.xuetiantiany.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://del.gaohongyu789.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vik.yangfankeji.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xtc.quarkkingdee.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kuv.sysykeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://luc.vqdsnc.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://psp.yj20258.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bfr.xylfe.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://eoa.fanxiaobao.xyz

[J09] 时区处理
来源：http://twa.ivvv.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://efp.xylfe.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nai.9152youxi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jdy.dashuyun.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aox.yj20258888.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zwj.svipenyu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fnj.guannengcc.top

Ruby: Time.now.getlocal("+08:00")
来源：http://sak.cucudq.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wli.feifeiyinyue.top

[J10] 取今天 / 本月第一天
来源：http://waz.gzhubu.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ccr.fehbvm.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vqh.tanke756.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rup.yongpay.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nwg.pycfn.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://myp.haohaochexian.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xpt.epnwcf.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cci.uphjek.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lcm.tarul.cn

================================================================================
来源：http://lwp.tarul.cn

K. JSON 与序列化
来源：http://kau.quarkkingdee.top

================================================================================
来源：http://ahf.mhx1999.top

[K01] 对象转 JSON 字符串
来源：http://amk.nanxuanxn.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uxa.zhixingplan.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kwh.c1oappe.top

JS:   JSON.stringify(obj)
来源：http://fgd.jqgufenzy.top

TS:   JSON.stringify(obj)
来源：http://myc.ywan-chungtsiang.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ocn.yongpay.top

Go:   json.Marshal(obj)
来源：http://ndz.ywan-chungtsiang.top

Ruby: obj.to_json                                     // require "json"
来源：http://pki.nwbrower.top

C#:   JsonSerializer.Serialize(obj)
来源：http://swc.kuanghao11.cn

[K02] JSON 字符串转对象
来源：http://mzg.ybcxt.top

Py:   json.loads(s)
来源：http://ydq.sjlbkw.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bei.hfpthk.cn

JS:   JSON.parse(s)
来源：http://dps.ydjk.org.cn

TS:   JSON.parse(s)
来源：http://dym.aizwys.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xyn.yvedp.cn

Go:   json.Unmarshal(data, &v)
来源：http://ums.zhongyouzk.top

Ruby: JSON.parse(s)
来源：http://udm.nanxinkj.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ywp.jinyuanbaomall.cn

[K03] JSON 美化输出（带缩进）
来源：http://dys.fzhhl.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sfy.zhengqikj.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://puy.sjlbkw.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ctg.iojbl.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vqo.nwbrower.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pxe.vehdjk.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://eff.fktsv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wqp.hcnkem.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zut.ivvv.top

[K04] 读取 JSON 文件
来源：http://xth.yongpay.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://iiz.ydzc1.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://piz.hysaishi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://esx.ydjk.org.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fei.shanyushiyangtech.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uzv.shzxlz.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cfr.tian-w.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tsb.9152youxi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kns.0kj1m.cn

[K05] 深拷贝对象
来源：http://cln.pycfn.com

Py:   copy.deepcopy(obj)
来源：http://qkr.guannengcc.top

PHP:  unserialize(serialize($obj));
来源：http://wko.fanxiaobao.xyz

JS:   structuredClone(obj)
来源：http://gkl.cheryme.top

TS:   structuredClone(obj)
来源：http://cka.zhoulong.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://yln.shanyushiyangkeji.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hsb.yj20258888.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nhe.yvedp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ykv.xinyue.icu

[K06] 解析 URL 查询串
来源：http://udk.316326.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://epg.quarkkingdee.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://otb.yangfankeji.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nwl.jinqigfzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hhu.shanyushiyangkeji.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zuq.fanxiaobao.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://six.zhoulong.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vqk.smart0.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pmu.ydjk.org.cn

[K07] 进制转换
来源：http://bqi.yangfankeji.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vjy.fengsongda.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lyr.dianchejie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dwy.nanxuanxn.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tjq.shzxlz.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gpw.jinyuanbaomall.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rlo.hongshengwenyu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qog.fzhhl.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fiu.nanxuanxn.top

[K08] 二进制序列化（非 JSON）
来源：http://fzj.jinyuanbaomall.cn

Py:   pickle.dumps(obj)
来源：http://qfr.quarkkingdee.top

PHP:  serialize($obj);  unserialize($s);
来源：http://you.guannengcc.top

JS:   v8.serialize(obj)        // Node
来源：http://mac.hesvh.cn

TS:   v8.serialize(obj)        // Node
来源：http://xey.0kj1m.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lpc.dashuyun.cn

Go:   encoding/gob
来源：http://zqm.daria6918.cn

Ruby: Marshal.dump(obj)
来源：http://iom.0kj1m.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yrn.daria6918.cn

================================================================================
来源：http://juv.epnwcf.com

L. 网络请求
来源：http://kkb.cheryme.top

================================================================================
来源：http://xzg.vehdjk.com

[L01] 发送 GET 请求
来源：http://oqz.gaohongyu789.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://oqs.cqqwz.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jky.jianghu66.top

JS:   await fetch(url)
来源：http://nzz.iojbl.cn

TS:   await fetch(url)
来源：http://jrp.jiagoushi.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gqb.birdmap.top

Go:   resp, err := http.Get(url)
来源：http://wle.dianchejie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rlf.wangdashe.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://efc.tianlin.xyz

[L02] 发送 POST JSON
来源：http://lme.fehbvm.com

Py:   requests.post(url, json={"a": 1})
来源：http://viy.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dga.hesvh.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rlc.yonumen.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hih.zhixingplan.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://szn.yonumen.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uho.fktsv.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kao.ydjk.org.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rog.jianghu66.top

[L03] 设置自定义请求头
来源：http://iix.hongshengwenyu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wav.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nui.yuxming.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://guc.cucudq.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qhu.xinyue.icu

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yxp.jiagoushi.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rgi.c1oappe.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hlb.xingfuxueyuan.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jvn.hongshengwenyu.top

[L04] 设置超时
来源：http://fcl.xylfe.cn

Py:   requests.get(url, timeout=5)
来源：http://zae.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xey.xylfe.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jjt.yuanzhike.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iyd.zhoulong.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://utg.hesvh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://car.guowangkeji.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qap.yangfankeji.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nqp.mhx1999.top

[L05] 上传文件（multipart）
来源：http://lks.sxryk.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blx.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zka.gzhubu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dzb.gotoacloud.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zun.cashguo.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xyk.vqdsnc.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dcz.ywan-chungtsiang.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://otx.jianghu66.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gfm.bbcook.cn

[L06] 解析响应为 JSON
来源：http://umm.jqgufenzy.top

Py:   resp.json()
来源：http://bhh.smart0.xyz

PHP:  json_decode($body, true);
来源：http://nqk.yueranfly.top

JS:   await resp.json()
来源：http://zsq.sweek.top

TS:   await resp.json()
来源：http://obh.nwbrower.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jss.fengsongda.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yzl.ivvv.top

Ruby: JSON.parse(resp.body)
来源：http://nah.yueranfly.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hws.xziqi.cn

[L07] 处理 HTTP 状态码
来源：http://duq.guowangkeji.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hme.meibo888.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://usb.316326.xyz

JS:   resp.ok;  resp.status
来源：http://xsj.xuetiantiany.cn

TS:   resp.ok;  resp.status
来源：http://rhx.yj20258888.top

Java: resp.statusCode()
来源：http://zfy.ybcxt.top

Go:   resp.StatusCode
来源：http://inz.zhongyouzk.top

Ruby: resp.code.to_i
来源：http://euj.sufxvd.cn

C#:   (int)resp.StatusCode
来源：http://luj.fanxiaobao.xyz

[L08] 并发请求多个地址
来源：http://qtb.shzxlz.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qnp.hysaishi.cn

PHP:  curl_multi_init() 系列
来源：http://lrv.tanke756.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fbw.cheryme.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wak.daxiang520.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tom.tarul.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wgp.sjlbkw.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://suy.chenlongwang.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qof.zhiwuduotai.top

================================================================================
来源：http://egr.pycfn.com

M. 命令行 / 进程 / 环境
来源：http://kff.jyoumei.cn

================================================================================
来源：http://uja.tanke756.top

[M01] 读取命令行参数
来源：http://kdr.ydzc1.top

Py:   sys.argv[1:]
来源：http://xxc.0kj1m.cn

PHP:  $argv;  $argc;
来源：http://cng.wangshuangyany.cn

JS:   process.argv.slice(2)
来源：http://aex.zhaomingkeji.xyz

TS:   process.argv.slice(2)
来源：http://xed.yonumen.top

Java: args 数组（main 方法参数）
来源：http://ivi.xuanzx.com

Go:   os.Args[1:]
来源：http://ypq.yanxiufei.cn

Ruby: ARGV
来源：http://ulk.jinyuanbaomall.cn

C#:   args 数组（Main 方法参数）
来源：http://wsd.tarul.cn

[M02] 读取环境变量
来源：http://brq.cheryme.top

Py:   os.environ.get("HOME")
来源：http://rdp.zhaomingkeji.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vrm.jinyuanbaomall.cn

JS:   process.env.HOME
来源：http://mzq.zhiwuduotai.top

TS:   process.env.HOME
来源：http://pki.cheryme.top

Java: System.getenv("HOME")
来源：http://bnw.zhijiandao.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sto.hongshengwenyu.top

Ruby: ENV["HOME"]
来源：http://rzy.uphjek.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fie.nanxinkj.top

[M03] 执行外部命令
来源：http://dgk.ydjk.org.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ncu.yj20258888.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ehf.ctjpmb.com

JS:   child_process.execSync("ls -l").toString()
来源：http://bii.dianchejie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yht.daxiang520.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rmm.jqgfzy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://rul.redwolf501.top

Ruby: system("ls -l");  `ls -l`
来源：http://dvy.jinyuanbaomall.cn

C#:   Process.Start("ls", "-l");
来源：http://hqp.zdqjudy.top

[M04] 获取当前工作目录
来源：http://tjj.chenzaomai.com

Py:   os.getcwd()
来源：http://gno.ywan-chungtsiang.top

PHP:  getcwd();
来源：http://trw.dianchejie.cn

JS:   process.cwd()
来源：http://nwn.hnxiangtu.top

TS:   process.cwd()
来源：http://auz.jlsjyb.cn

Java: Path.of("").toAbsolutePath()
来源：http://mpm.yueranfly.top

Go:   os.Getwd()
来源：http://vvu.fehbvm.com

Ruby: Dir.pwd
来源：http://egq.ehwqpu.com

C#:   Directory.GetCurrentDirectory()
来源：http://bec.xuanzx.com

[M05] 设置退出码
来源：http://pac.shzxlz.cn

Py:   sys.exit(1)
来源：http://yqt.yj202588.top

PHP:  exit(1);
来源：http://zni.yvedp.cn

JS:   process.exit(1)
来源：http://bmn.bjfxy.top

TS:   process.exit(1)
来源：http://euy.gotoacloud.top

Java: System.exit(1)
来源：http://cli.52xcode.cn

Go:   os.Exit(1)
来源：http://atr.aibaodan.cn

Ruby: exit 1
来源：http://uew.smart0.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jjb.jqgfzy.top

[M06] 向标准错误输出
来源：http://nkn.smart0.xyz

Py:   print("err", file=sys.stderr)
来源：http://hmh.gaohongyu789.top

PHP:  fwrite(STDERR, "err\n");
来源：http://yfa.52xcode.cn

JS:   console.error("err")
来源：http://zwm.hysaishi.cn

TS:   console.error("err")
来源：http://yqn.nanxuanxn.top

Java: System.err.println("err")
来源：http://ran.pycfn.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kne.aibaodan.cn

Ruby: warn "err"
来源：http://fyb.jinqigfzy.top

C#:   Console.Error.WriteLine("err")
来源：http://gbq.hnqzz.top

[M07] 判断是否为主入口
来源：http://jxk.zhaomingkeji.xyz


<!-- 参考信息 -->