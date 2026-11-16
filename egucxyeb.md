代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zpc.zhongyouzk.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ayc.nanxinkj.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fgf.yuanzhike.top

================================================================================
来源：http://wii.yonumen.top

J. 日期与时间
来源：http://lmn.shanyushiyangkeji.top

================================================================================
来源：http://hwc.wangdashe.top

[J01] 获取当前时间
来源：http://hwj.redwolf501.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://eal.pycfn.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wpi.hcnkem.com

JS:   new Date();  Date.now()
来源：http://tee.jinqigufen.top

TS:   new Date();  Date.now()
来源：http://hho.yuxming.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zll.uphjek.com

Go:   time.Now()
来源：http://hzu.ppjwa.cn

Ruby: Time.now
来源：http://xwb.ywan-chungtsiang.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sba.0kj1m.cn

[J02] 格式化输出
来源：http://hse.zhengqikj.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zpm.sjlbkw.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ohr.yongpay.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nhw.daria6918.cn

TS:   d.toISOString()
来源：http://hsr.316326.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://maj.havefunace.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tkm.chenjidiqi.icu

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://koi.nwbrower.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qjy.vehdjk.com

[J03] 字符串解析为日期
来源：http://soq.sxryk.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vdw.hongshengwenyu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xbv.yj20258888.top

JS:   new Date("2024-01-02")
来源：http://hta.zhijiandao.cn

TS:   new Date("2024-01-02")
来源：http://gch.quarkkingdee.top

Java: LocalDate.parse("2024-01-02")
来源：http://gys.sysykeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nhe.jqgfzy.top

Ruby: Date.parse("2024-01-02")
来源：http://ypv.sufxvd.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bjl.fanxiaobao.xyz

[J04] 时间戳与日期互转
来源：http://qnt.cheryme.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uda.pengpengdd.cyou

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wjp.smart0.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vil.andypj.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://cby.guannengcc.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zzz.hesvh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jpw.svipenyu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xry.chenzaomai.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tbu.zhijiandao.cn

[J05] 时间加减（加 7 天）
来源：http://lfe.vehdjk.com

Py:   now + timedelta(days=7)
来源：http://vvo.ywan-chungtsiang.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://vdx.daxiang520.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ayg.shuidangran.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vmg.guannengcc.top

Java: LocalDate.now().plusDays(7)
来源：http://gmg.hongshengwenyu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fif.kuanghao11.cn

Ruby: Time.now + 7 * 86400
来源：http://iwi.kuanghao11.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gjn.jinyuanbaomall.cn

[J06] 计算两时间之差
来源：http://lqi.zhaomingkeji.xyz

Py:   (end - start).total_seconds()
来源：http://raq.hfpthk.cn

PHP:  $end->diff($start)->days;
来源：http://tpp.tarul.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xcn.0kj1m.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://egy.sufxvd.cn

Java: Duration.between(start, end).toSeconds()
来源：http://paj.xinyue.icu

Go:   end.Sub(start).Hours()
来源：http://mdt.cdnleiting.top

Ruby: end - start                 # 返回秒数
来源：http://vgg.fktsv.cn

C#:   (end - start).TotalSeconds
来源：http://iih.quarkkingdee.top

[J07] 比较两个日期
来源：http://rsu.aibaodan.cn

Py:   d1 < d2;  d1 == d2
来源：http://kzv.jqgufenzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gms.shzxlz.cn

JS:   d1.getTime() < d2.getTime()
来源：http://law.yj20258888.top

TS:   d1.getTime() < d2.getTime()
来源：http://qmw.shanyushiyangkeji.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zhz.fehbvm.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nnc.haohaochexian.top

Ruby: d1 < d2;  d1 == d2
来源：http://oys.fzhhl.top

C#:   d1 < d2;  d1 == d2
来源：http://vzo.chenlongwang.top

[J08] 提取年月日与星期
来源：http://vqr.ydzc1.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kzg.jqgfzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hfz.svipenyu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://haw.ydjk.org.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vnl.havefunace.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://foj.mhx1999.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://avc.daxiang520.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ebo.jinqigufen.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dib.zhijiandao.cn

[J09] 时区处理
来源：http://nfg.fehbvm.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pzb.jinyuanbaomall.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://aqs.shanyushiyangkeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uhk.epnwcf.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gua.shuidangran.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lrf.hongshengwenyu.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sje.ctjpmb.com

Ruby: Time.now.getlocal("+08:00")
来源：http://fvz.fehbvm.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hcv.316326.xyz

[J10] 取今天 / 本月第一天
来源：http://dzu.yuxming.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xtf.aizwys.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hab.ctjpmb.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://emv.316326.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://keu.jianghu66.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zwr.zhiwuduotai.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ndg.redwolf501.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qmb.yongpay.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fwu.zhongyouzk.top

================================================================================
来源：http://zlp.dashuyun.cn

K. JSON 与序列化
来源：http://gwc.sysykeji.top

================================================================================
来源：http://xgj.bjfxy.top

[K01] 对象转 JSON 字符串
来源：http://doo.fzhhl.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fvd.vqdsnc.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://scw.meibo888.top

JS:   JSON.stringify(obj)
来源：http://zkx.yangfankeji.com

TS:   JSON.stringify(obj)
来源：http://crc.guannengcc.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mut.chenlongwang.top

Go:   json.Marshal(obj)
来源：http://vwn.c1oappe.top

Ruby: obj.to_json                                     // require "json"
来源：http://liy.zdbjq.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nth.cucudq.cn

[K02] JSON 字符串转对象
来源：http://vbc.0kj1m.cn

Py:   json.loads(s)
来源：http://ycb.vqdsnc.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ahg.ivvv.top

JS:   JSON.parse(s)
来源：http://bqe.mhx1999.top

TS:   JSON.parse(s)
来源：http://ubn.ybcxt.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gbm.feifeiyinyue.top

Go:   json.Unmarshal(data, &v)
来源：http://eel.fzhhl.top

Ruby: JSON.parse(s)
来源：http://gpo.zhoulong.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wti.yuxming.cn

[K03] JSON 美化输出（带缩进）
来源：http://hgj.zhengqikj.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mbz.xziqi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hui.316326.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://kcx.feifeiyinyue.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ysq.zhoulong.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ynu.jiagoushi.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ovv.xingfuxueyuan.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://qfr.fktsv.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xke.pycfn.com

[K04] 读取 JSON 文件
来源：http://rpu.jinqigfzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://igd.sysykeji.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yat.fktsv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lgm.zdbjq.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aac.daria6918.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gfk.wangshuangyany.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://toj.dianchejie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://smj.xuetiantiany.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://efd.ydzc1.top

[K05] 深拷贝对象
来源：http://qhb.yongpay.top

Py:   copy.deepcopy(obj)
来源：http://cdc.jinghuilouyu.cn

PHP:  unserialize(serialize($obj));
来源：http://one.52xcode.cn

JS:   structuredClone(obj)
来源：http://ilm.gotoacloud.top

TS:   structuredClone(obj)
来源：http://tds.ivvv.top

Java: // 手写拷贝构造，或序列化往返
来源：http://xdn.fanxiaobao.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://odc.cqqwz.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nza.shzxlz.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mql.ydzc1.top

[K06] 解析 URL 查询串
来源：http://hgi.guowangkeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://twm.jlsjyb.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://laz.hammf.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://adb.wangdashe.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cvp.hnxiangtu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://muz.zhongyouzk.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://gdw.jqgfzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kpl.nwbrower.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ghw.jinqigfzy.top

[K07] 进制转换
来源：http://vyq.jinqigfzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nwp.nanxinkj.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xvl.tianlin.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nwj.fktsv.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xds.bbcook.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cgm.zycfv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tee.ppjwa.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ofg.zdbjq.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jcx.0kj1m.cn

[K08] 二进制序列化（非 JSON）
来源：http://xwy.vehdjk.com

Py:   pickle.dumps(obj)
来源：http://zwp.fengsongda.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ihj.yongpay.top

JS:   v8.serialize(obj)        // Node
来源：http://zus.bbcook.cn

TS:   v8.serialize(obj)        // Node
来源：http://xef.chenlongwang.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://snv.jianghu66.top

Go:   encoding/gob
来源：http://iku.hysaishi.cn

Ruby: Marshal.dump(obj)
来源：http://ckb.hysaishi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://itp.jinyuanbaomall.cn

================================================================================
来源：http://lfl.smart0.xyz

L. 网络请求
来源：http://ocq.epnwcf.com

================================================================================
来源：http://sti.pengpengdd.cyou

[L01] 发送 GET 请求
来源：http://fhy.yj202588.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zeg.c1oappe.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bqz.zycfv.cn

JS:   await fetch(url)
来源：http://jnl.aibaodan.cn

TS:   await fetch(url)
来源：http://fhy.cucudq.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jnf.fehbvm.com

Go:   resp, err := http.Get(url)
来源：http://zbq.chenjidiqi.icu

Ruby: Net::HTTP.get(URI(url))
来源：http://vpy.uphjek.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://brk.chenzaomai.com

[L02] 发送 POST JSON
来源：http://vfp.cucudq.cn

Py:   requests.post(url, json={"a": 1})
来源：http://axf.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vze.uphjek.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xve.yj202588.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ayz.daria6918.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ajx.redwolf501.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ggt.pycfn.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cby.yuanzhike.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ftt.shzxlz.cn

[L03] 设置自定义请求头
来源：http://hmq.ybcxt.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dhg.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wcp.tian-w.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cvj.feifeiyinyue.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qlu.c1oappe.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zrx.jlsjyb.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://urx.cheryme.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zpc.tian-w.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qnv.mhx1999.top

[L04] 设置超时
来源：http://yeu.andypj.xyz

Py:   requests.get(url, timeout=5)
来源：http://noa.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://oid.hysaishi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zlo.xziqi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mki.xuanzx.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qwx.yuanzhike.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pvx.aibaodan.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tkp.fengsongda.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lvx.shuidangran.top

[L05] 上传文件（multipart）
来源：http://npl.yangfankeji.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oro.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://olz.zhengqikj.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xqh.cucudq.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dgf.jlsjyb.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ubt.yj20258888.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jfu.hfpthk.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lpa.bbcook.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lgl.zhaomingkeji.xyz

[L06] 解析响应为 JSON
来源：http://yrw.fengsongda.top

Py:   resp.json()
来源：http://ila.zhoulong.xyz

PHP:  json_decode($body, true);
来源：http://msk.yj20258.top

JS:   await resp.json()
来源：http://vly.cashguo.top

TS:   await resp.json()
来源：http://ywl.yuanzhike.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mvb.cqqwz.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ghl.jqgufenzy.top

Ruby: JSON.parse(resp.body)
来源：http://nbb.bbcook.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fxa.wangshuangyany.cn

[L07] 处理 HTTP 状态码
来源：http://fho.yanxiufei.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://myd.xuetiantiany.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tdu.epnwcf.com

JS:   resp.ok;  resp.status
来源：http://buq.hammf.cn

TS:   resp.ok;  resp.status
来源：http://qfo.shuidangran.top

Java: resp.statusCode()
来源：http://cnj.zhongyouzk.top

Go:   resp.StatusCode
来源：http://bfq.fktsv.cn

Ruby: resp.code.to_i
来源：http://zdv.sweek.top

C#:   (int)resp.StatusCode
来源：http://icc.vqdsnc.cn

[L08] 并发请求多个地址
来源：http://eyo.dianchejie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yyl.hnqzz.top

PHP:  curl_multi_init() 系列
来源：http://omd.yuanzhike.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yny.vehdjk.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ftm.ctjpmb.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ebt.snrcjt.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rgk.ybcxt.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ztp.cqqwz.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://chy.ppjwa.cn

================================================================================
来源：http://tqo.xingfuxueyuan.xyz

M. 命令行 / 进程 / 环境
来源：http://ube.cashguo.top

================================================================================
来源：http://azg.jyoumei.cn

[M01] 读取命令行参数
来源：http://hlq.fehbvm.com

Py:   sys.argv[1:]
来源：http://arc.xinyue.icu

PHP:  $argv;  $argc;
来源：http://wfn.dianchejie.cn

JS:   process.argv.slice(2)
来源：http://csr.havefunace.top

TS:   process.argv.slice(2)
来源：http://tyi.haohaochexian.top

Java: args 数组（main 方法参数）
来源：http://cix.zhengqikj.top

Go:   os.Args[1:]
来源：http://emm.jianghu66.top

Ruby: ARGV
来源：http://jou.sweek.top

C#:   args 数组（Main 方法参数）
来源：http://pgw.svipenyu.cn

[M02] 读取环境变量
来源：http://mnu.yonumen.top

Py:   os.environ.get("HOME")
来源：http://ygp.ppjwa.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yoa.iojbl.cn

JS:   process.env.HOME
来源：http://wul.tanke756.top

TS:   process.env.HOME
来源：http://adh.epnwcf.com

Java: System.getenv("HOME")
来源：http://xfq.yueranfly.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vhj.sxryk.cn

Ruby: ENV["HOME"]
来源：http://gyy.zhengqikj.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ogi.nanxinkj.top

[M03] 执行外部命令
来源：http://pqu.daxiang520.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lil.jinghuilouyu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dos.aibaodan.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://uje.meibo888.top

TS:   child_process.execSync("ls -l").toString()
来源：http://rzx.jinyuanbaomall.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pdf.shzxlz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pnb.hammf.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dte.xuetiantiany.cn

C#:   Process.Start("ls", "-l");
来源：http://iop.daria6918.cn

[M04] 获取当前工作目录
来源：http://zjd.52xcode.cn

Py:   os.getcwd()
来源：http://piu.0kj1m.cn

PHP:  getcwd();
来源：http://tel.epnwcf.com

JS:   process.cwd()
来源：http://izg.shangyingyoupin.top

TS:   process.cwd()
来源：http://mbb.smart0.xyz

Java: Path.of("").toAbsolutePath()
来源：http://nto.aizwys.cn

Go:   os.Getwd()
来源：http://wzr.chenjidiqi.icu

Ruby: Dir.pwd
来源：http://aei.jianghu66.top

C#:   Directory.GetCurrentDirectory()
来源：http://mwt.xuanzx.com

[M05] 设置退出码
来源：http://dov.jinyuanbaomall.cn

Py:   sys.exit(1)
来源：http://agq.gogol.net.cn

PHP:  exit(1);
来源：http://bwh.chenzaomai.com

JS:   process.exit(1)
来源：http://bwn.ppjwa.cn

TS:   process.exit(1)
来源：http://bjv.hnqzz.top

Java: System.exit(1)
来源：http://gef.bjfxy.top

Go:   os.Exit(1)
来源：http://nxv.xuetiantiany.cn

Ruby: exit 1
来源：http://voo.aizwys.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bus.redwolf501.top

[M06] 向标准错误输出
来源：http://sxe.tarul.cn

Py:   print("err", file=sys.stderr)
来源：http://nrn.yongpay.top

PHP:  fwrite(STDERR, "err\n");
来源：http://orr.cashguo.top

JS:   console.error("err")
来源：http://xdy.kuanghao11.cn

TS:   console.error("err")
来源：http://cub.birdmap.top

Java: System.err.println("err")
来源：http://nye.c1oappe.top


<!-- 参考信息 -->