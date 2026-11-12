代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://usd.jlsjyb.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://znn.gogol.net.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lxe.jqgufenzy.top

================================================================================
来源：http://zxt.tanke756.top

J. 日期与时间
来源：http://ndk.svipenyu.cn

================================================================================
来源：http://xdo.snrcjt.cn

[J01] 获取当前时间
来源：http://idx.jiagoushi.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://xor.daria6918.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yor.fengsongda.top

JS:   new Date();  Date.now()
来源：http://etf.hcnkem.com

TS:   new Date();  Date.now()
来源：http://cxt.ivvv.top

Java: LocalDateTime.now();  Instant.now()
来源：http://osa.jinghuilouyu.cn

Go:   time.Now()
来源：http://btk.svipenyu.cn

Ruby: Time.now
来源：http://qat.cdnleiting.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yqq.jlsjyb.cn

[J02] 格式化输出
来源：http://qew.yonumen.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://shh.yj20258.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kiu.316326.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ngd.yj20258888.top

TS:   d.toISOString()
来源：http://rkt.yangfankeji.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qls.52xcode.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://moh.hywenlv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jfu.zhongyouzk.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dwd.yj20258.top

[J03] 字符串解析为日期
来源：http://yod.yj20258888.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xsu.sysykeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://whx.aibaodan.cn

JS:   new Date("2024-01-02")
来源：http://hvx.epnwcf.com

TS:   new Date("2024-01-02")
来源：http://eta.sysykeji.top

Java: LocalDate.parse("2024-01-02")
来源：http://far.jinqigufen.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xof.vqdsnc.cn

Ruby: Date.parse("2024-01-02")
来源：http://mjq.yj20258.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gvi.yfazqb.com

[J04] 时间戳与日期互转
来源：http://nja.chenjidiqi.icu

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jrj.zhengqikj.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rfq.sysykeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yoa.zhoulong.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://kzz.hongshengwenyu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nmo.ybcxt.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lnv.zhoulong.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zzh.pengpengdd.cyou

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gbd.ppjwa.cn

[J05] 时间加减（加 7 天）
来源：http://dcc.gogol.net.cn

Py:   now + timedelta(days=7)
来源：http://jpy.zycfv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jrv.hammf.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fhp.yonumen.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mma.hongshengwenyu.top

Java: LocalDate.now().plusDays(7)
来源：http://voi.jinyuanbaomall.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://eof.jinghuilouyu.cn

Ruby: Time.now + 7 * 86400
来源：http://jpr.jinghuilouyu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jyt.redwolf501.top

[J06] 计算两时间之差
来源：http://awa.jinqigufen.top

Py:   (end - start).total_seconds()
来源：http://jmh.zhengqikj.top

PHP:  $end->diff($start)->days;
来源：http://jet.gaohongyu789.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tnt.daxiang520.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ptl.316326.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://cqb.fktsv.cn

Go:   end.Sub(start).Hours()
来源：http://zki.52xcode.cn

Ruby: end - start                 # 返回秒数
来源：http://ute.svipenyu.cn

C#:   (end - start).TotalSeconds
来源：http://bro.zhaomingkeji.xyz

[J07] 比较两个日期
来源：http://pun.sweek.top

Py:   d1 < d2;  d1 == d2
来源：http://hdf.cqqwz.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zgj.gogol.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://iit.epnwcf.com

TS:   d1.getTime() < d2.getTime()
来源：http://mdn.yonumen.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zxt.fehbvm.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cqy.ybcxt.top

Ruby: d1 < d2;  d1 == d2
来源：http://ktd.cqqwz.cn

C#:   d1 < d2;  d1 == d2
来源：http://jcv.sweek.top

[J08] 提取年月日与星期
来源：http://akp.xingfuxueyuan.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mne.shzxlz.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gxx.svipenyu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jho.daxiang520.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oox.chenjidiqi.icu

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://slu.yj20258.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cwp.ehwqpu.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qdm.gzhubu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sbt.jqgufenzy.top

[J09] 时区处理
来源：http://dyp.yongpay.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://van.jqgufenzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sni.hongshengwenyu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rfg.hnxiangtu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ygh.yueranfly.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ket.ppjwa.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://txq.shanyushiyangkeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://vjv.epnwcf.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jwa.haohaochexian.top

[J10] 取今天 / 本月第一天
来源：http://ida.ywan-chungtsiang.top

Py:   date.today();  date.today().replace(day=1)
来源：http://crh.gaohongyu789.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uef.sufxvd.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rnz.jinqigufen.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://srz.bjfxy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kux.vqdsnc.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gjo.yj202588.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://plq.hcnkem.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lxp.gaohongyu789.top

================================================================================
来源：http://weg.chenzaomai.com

K. JSON 与序列化
来源：http://ctj.yj20258.top

================================================================================
来源：http://hbd.nwbrower.top

[K01] 对象转 JSON 字符串
来源：http://ydt.hongshengwenyu.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ndw.sjlbkw.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oje.yj20258.top

JS:   JSON.stringify(obj)
来源：http://drk.redwolf501.top

TS:   JSON.stringify(obj)
来源：http://lut.iojbl.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ekq.zhaomingkeji.xyz

Go:   json.Marshal(obj)
来源：http://odf.shuidangran.top

Ruby: obj.to_json                                     // require "json"
来源：http://acg.svipenyu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://eti.chenjidiqi.icu

[K02] JSON 字符串转对象
来源：http://hll.hesvh.cn

Py:   json.loads(s)
来源：http://bnu.wangshuangyany.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pmf.yueranfly.top

JS:   JSON.parse(s)
来源：http://qrh.hongshengwenyu.top

TS:   JSON.parse(s)
来源：http://hfv.iojbl.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xxg.hesvh.cn

Go:   json.Unmarshal(data, &v)
来源：http://ehq.yuanzhike.top

Ruby: JSON.parse(s)
来源：http://gyz.fanxiaobao.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tjv.zdbjq.cn

[K03] JSON 美化输出（带缩进）
来源：http://hjc.shanyushiyangtech.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uit.xingfuxueyuan.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://idz.yj20258888.top

JS:   JSON.stringify(obj, null, 2)
来源：http://rqw.haohaochexian.top

TS:   JSON.stringify(obj, null, 2)
来源：http://tvo.sjlbkw.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://giz.ydzc1.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mom.nanxuanxn.top

Ruby: JSON.pretty_generate(obj)
来源：http://osa.ywan-chungtsiang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cji.yuanzhike.top

[K04] 读取 JSON 文件
来源：http://fwv.hnqzz.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://inl.wangshuangyany.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vyy.hammf.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jik.fanxiaobao.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fdm.shzxlz.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nhr.fengsongda.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://isi.hfpthk.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fib.jiagoushi.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uak.yanxiufei.cn

[K05] 深拷贝对象
来源：http://dpl.ctjpmb.com

Py:   copy.deepcopy(obj)
来源：http://ajb.yuanzhike.top

PHP:  unserialize(serialize($obj));
来源：http://aoh.sjlbkw.cn

JS:   structuredClone(obj)
来源：http://ivx.yuxming.cn

TS:   structuredClone(obj)
来源：http://baf.wangdashe.top

Java: // 手写拷贝构造，或序列化往返
来源：http://krx.hfpthk.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zcq.ehwqpu.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ywq.jqgfzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://kqh.ctjpmb.com

[K06] 解析 URL 查询串
来源：http://vdr.ydzc1.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hbj.meibo888.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mzh.gaohongyu789.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://reb.yfazqb.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kfh.guannengcc.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://owi.yonumen.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://lfh.52xcode.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bmw.chenlongwang.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nmo.sysykeji.top

[K07] 进制转换
来源：http://fjh.zdbjq.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zsq.dianchejie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hqq.nanxinkj.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jen.jyoumei.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fgn.guowangkeji.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wei.shanyushiyangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fhl.xuetiantiany.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qyw.yj202588.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gwk.jinqigufen.top

[K08] 二进制序列化（非 JSON）
来源：http://enr.xuetiantiany.cn

Py:   pickle.dumps(obj)
来源：http://klr.hnqzz.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ukf.zhijiandao.cn

JS:   v8.serialize(obj)        // Node
来源：http://ume.shuidangran.top

TS:   v8.serialize(obj)        // Node
来源：http://jlv.shanyushiyangkeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wzx.redwolf501.top

Go:   encoding/gob
来源：http://bgt.jqgfzy.top

Ruby: Marshal.dump(obj)
来源：http://vxu.nanxuanxn.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ngq.xziqi.cn

================================================================================
来源：http://nun.yuxming.cn

L. 网络请求
来源：http://oxd.ivvv.top

================================================================================
来源：http://sro.dashuyun.cn

[L01] 发送 GET 请求
来源：http://qls.chenjidiqi.icu

Py:   requests.get(url)                        # 第三方库 requests
来源：http://koq.nanxinkj.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vuv.9152youxi.cn

JS:   await fetch(url)
来源：http://sey.yvedp.cn

TS:   await fetch(url)
来源：http://bsy.wangshuangyany.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mpy.hysaishi.cn

Go:   resp, err := http.Get(url)
来源：http://qwf.tian-w.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://isv.iojbl.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dfn.yvedp.cn

[L02] 发送 POST JSON
来源：http://jis.fanxiaobao.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://ezn.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uui.cashguo.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pvm.havefunace.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jut.ybcxt.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://oja.gaohongyu789.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vpj.gogol.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bvy.ybcxt.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bvo.guowangkeji.top

[L03] 设置自定义请求头
来源：http://mwl.yj20258.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vkh.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jad.tanke756.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sid.hnqzz.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://aeq.yanxiufei.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gyk.feifeiyinyue.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://omi.yuanzhike.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lyp.chenlongwang.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hvw.andypj.xyz

[L04] 设置超时
来源：http://ynq.zhaomingkeji.xyz

Py:   requests.get(url, timeout=5)
来源：http://wbf.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hhj.uphjek.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://krs.hnxiangtu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zyr.fzhhl.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lqq.tianlin.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://whe.ehwqpu.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://khi.ywan-chungtsiang.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rvl.meibo888.top

[L05] 上传文件（multipart）
来源：http://buq.cucudq.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qvt.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mur.zhixingplan.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ehc.ydzc1.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kvx.hywenlv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vde.vqdsnc.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ynr.hnxiangtu.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hhw.vqdsnc.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qxm.smart0.xyz

[L06] 解析响应为 JSON
来源：http://cri.bjfxy.top

Py:   resp.json()
来源：http://ntn.0kj1m.cn

PHP:  json_decode($body, true);
来源：http://lmf.zdqjudy.top

JS:   await resp.json()
来源：http://mfi.xuanzx.com

TS:   await resp.json()
来源：http://qnz.sweek.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://iav.hcnkem.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kts.0kj1m.cn

Ruby: JSON.parse(resp.body)
来源：http://oho.andypj.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://frz.dianchejie.cn

[L07] 处理 HTTP 状态码
来源：http://gqw.yfazqb.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vfh.gotoacloud.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ztx.tian-w.cn

JS:   resp.ok;  resp.status
来源：http://lwj.hnqzz.top

TS:   resp.ok;  resp.status
来源：http://wrv.hongshengwenyu.top

Java: resp.statusCode()
来源：http://eej.daxiang520.top

Go:   resp.StatusCode
来源：http://xsy.yuanzhike.top

Ruby: resp.code.to_i
来源：http://xic.kuanghao11.cn

C#:   (int)resp.StatusCode
来源：http://lki.cqqwz.cn

[L08] 并发请求多个地址
来源：http://iue.zhengqikj.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yhg.shzxlz.cn

PHP:  curl_multi_init() 系列
来源：http://iiv.yj20258888.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kmx.tianlin.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dey.xziqi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://isn.gogol.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yrr.tarul.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lll.jiagoushi.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tfp.shzxlz.cn

================================================================================
来源：http://ulz.hnqzz.top

M. 命令行 / 进程 / 环境
来源：http://krr.pycfn.com

================================================================================
来源：http://pfw.xingfuxueyuan.xyz

[M01] 读取命令行参数
来源：http://adn.yj202588.top

Py:   sys.argv[1:]
来源：http://qgu.hcnkem.com

PHP:  $argv;  $argc;
来源：http://cxi.tian-w.cn

JS:   process.argv.slice(2)
来源：http://zco.cheryme.top

TS:   process.argv.slice(2)
来源：http://dwt.birdmap.top

Java: args 数组（main 方法参数）
来源：http://ofo.uphjek.com

Go:   os.Args[1:]
来源：http://irs.yangfankeji.com

Ruby: ARGV
来源：http://bgt.tianlin.xyz

C#:   args 数组（Main 方法参数）
来源：http://nyq.jianghu66.top

[M02] 读取环境变量
来源：http://aoz.birdmap.top

Py:   os.environ.get("HOME")
来源：http://wfw.jqgfzy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nhn.yueranfly.top

JS:   process.env.HOME
来源：http://vbz.tarul.cn

TS:   process.env.HOME
来源：http://mbu.smart0.xyz

Java: System.getenv("HOME")
来源：http://wcm.daria6918.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jig.yj20258.top

Ruby: ENV["HOME"]
来源：http://upj.sufxvd.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dfi.fengsongda.top

[M03] 执行外部命令
来源：http://khp.ctjpmb.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kwr.chenlongwang.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pgw.epnwcf.com

JS:   child_process.execSync("ls -l").toString()
来源：http://jmf.sxryk.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://cpe.yj202588.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xzx.kuanghao11.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jcr.ehwqpu.com

Ruby: system("ls -l");  `ls -l`
来源：http://ktx.9152youxi.cn

C#:   Process.Start("ls", "-l");
来源：http://bst.yangfankeji.com

[M04] 获取当前工作目录
来源：http://uyx.jinghuilouyu.cn

Py:   os.getcwd()
来源：http://vhr.sysykeji.top

PHP:  getcwd();
来源：http://ycy.daria6918.cn

JS:   process.cwd()
来源：http://nnd.xylfe.cn

TS:   process.cwd()
来源：http://upe.meibo888.top

Java: Path.of("").toAbsolutePath()
来源：http://ctw.cheryme.top

Go:   os.Getwd()
来源：http://zxr.andypj.xyz

Ruby: Dir.pwd
来源：http://ynz.pycfn.com

C#:   Directory.GetCurrentDirectory()
来源：http://krb.yonumen.top

[M05] 设置退出码
来源：http://ctu.shzxlz.cn

Py:   sys.exit(1)
来源：http://loj.jyoumei.cn

PHP:  exit(1);
来源：http://pwh.havefunace.top

JS:   process.exit(1)
来源：http://zhx.gogol.net.cn

TS:   process.exit(1)
来源：http://hsw.jinghuilouyu.cn

Java: System.exit(1)
来源：http://ajc.cqqwz.cn

Go:   os.Exit(1)
来源：http://pxs.jyoumei.cn

Ruby: exit 1
来源：http://mxz.zhongyouzk.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://otj.gaohongyu789.top

[M06] 向标准错误输出
来源：http://kgh.daxiang520.top

Py:   print("err", file=sys.stderr)
来源：http://bub.mhx1999.top

PHP:  fwrite(STDERR, "err\n");
来源：http://lwd.zhiwuduotai.top

JS:   console.error("err")
来源：http://vww.jiagoushi.top

TS:   console.error("err")
来源：http://bzf.0kj1m.cn

Java: System.err.println("err")
来源：http://xrm.yuxming.cn


<!-- 参考信息 -->