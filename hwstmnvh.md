代发 wailian999

J. 日期与时间
来源：http://tba.xingfuxueyuan.xyz

================================================================================
来源：http://rfp.hnxiangtu.top

[J01] 获取当前时间
来源：http://jbt.yongpay.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://uut.hesvh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zxb.fzhhl.top

JS:   new Date();  Date.now()
来源：http://jmq.0kj1m.cn

TS:   new Date();  Date.now()
来源：http://dto.dashuyun.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mwe.zhoulong.xyz

Go:   time.Now()
来源：http://ehr.nanxuanxn.top

Ruby: Time.now
来源：http://uuf.yuxming.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://omn.ydjk.org.cn

[J02] 格式化输出
来源：http://dys.jiagoushi.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fjl.jinyuanbaomall.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wlg.zhijiandao.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uhj.shzxlz.cn

TS:   d.toISOString()
来源：http://hxz.bbcook.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wkg.cashguo.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://szw.aibaodan.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lxk.quarkkingdee.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qhs.cdnleiting.top

[J03] 字符串解析为日期
来源：http://zfp.zycfv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kpf.zhengqikj.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gtm.uphjek.com

JS:   new Date("2024-01-02")
来源：http://luw.vqdsnc.cn

TS:   new Date("2024-01-02")
来源：http://nif.zhaomingkeji.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://jif.xinyue.icu

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dhy.9152youxi.cn

Ruby: Date.parse("2024-01-02")
来源：http://soi.quarkkingdee.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fva.xuanzx.com

[J04] 时间戳与日期互转
来源：http://dqt.sysykeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nom.zhixingplan.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mrg.jqgufenzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uac.redwolf501.top

TS:   Math.floor(Date.now() / 1000)
来源：http://hxn.svipenyu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://aph.cashguo.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://eqk.mhx1999.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xsn.yj202588.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hbb.xuetiantiany.cn

[J05] 时间加减（加 7 天）
来源：http://kun.zdbjq.cn

Py:   now + timedelta(days=7)
来源：http://rcv.zdbjq.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mej.xingfuxueyuan.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rhe.feifeiyinyue.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ocr.zycfv.cn

Java: LocalDate.now().plusDays(7)
来源：http://bgt.tian-w.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://izn.yangfankeji.com

Ruby: Time.now + 7 * 86400
来源：http://lft.bjfxy.top

C#:   DateTime.Now.AddDays(7)
来源：http://iut.cheryme.top

[J06] 计算两时间之差
来源：http://gao.tanke756.top

Py:   (end - start).total_seconds()
来源：http://uly.hongshengwenyu.top

PHP:  $end->diff($start)->days;
来源：http://ofr.vehdjk.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ckk.dashuyun.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vrl.mhx1999.top

Java: Duration.between(start, end).toSeconds()
来源：http://ysg.snrcjt.cn

Go:   end.Sub(start).Hours()
来源：http://cqx.zhengqikj.top

Ruby: end - start                 # 返回秒数
来源：http://kbc.shanyushiyangtech.top

C#:   (end - start).TotalSeconds
来源：http://iee.tian-w.cn

[J07] 比较两个日期
来源：http://agr.smart0.xyz

Py:   d1 < d2;  d1 == d2
来源：http://lbm.9152youxi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vck.xuanzx.com

JS:   d1.getTime() < d2.getTime()
来源：http://pgn.jqgfzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://fvo.zhengqikj.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://izr.jqgfzy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qwh.dashuyun.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fsr.vqdsnc.cn

C#:   d1 < d2;  d1 == d2
来源：http://fnt.smart0.xyz

[J08] 提取年月日与星期
来源：http://ezh.guowangkeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nqu.zhoulong.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ewt.hysaishi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bwa.snrcjt.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xmy.jqgufenzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jfx.hnqzz.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fxs.zdbjq.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jln.hfpthk.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hnt.tian-w.cn

[J09] 时区处理
来源：http://vjz.fzhhl.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xst.jinqigfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://evv.chenlongwang.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uhp.guowangkeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wbd.xuetiantiany.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dox.meibo888.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://avi.9152youxi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://oly.xylfe.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://umq.svipenyu.cn

[J10] 取今天 / 本月第一天
来源：http://dwk.zhiwuduotai.top

Py:   date.today();  date.today().replace(day=1)
来源：http://wsm.shanyushiyangkeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qwj.sxryk.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jcc.yvedp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dov.zhoulong.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gkn.uphjek.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ywg.yj20258888.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mcp.sweek.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://txv.ywan-chungtsiang.top

================================================================================
来源：http://ajv.jianghu66.top

K. JSON 与序列化
来源：http://alb.fehbvm.com

================================================================================
来源：http://peb.hammf.cn

[K01] 对象转 JSON 字符串
来源：http://ftv.chenjidiqi.icu

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qbc.guannengcc.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://adk.zdbjq.cn

JS:   JSON.stringify(obj)
来源：http://woz.epnwcf.com

TS:   JSON.stringify(obj)
来源：http://zgk.nanxinkj.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://djs.tian-w.cn

Go:   json.Marshal(obj)
来源：http://mdt.xingfuxueyuan.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://ohr.cheryme.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ram.guannengcc.top

[K02] JSON 字符串转对象
来源：http://kgy.kuanghao11.cn

Py:   json.loads(s)
来源：http://pzd.gogol.net.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fkt.chenzaomai.com

JS:   JSON.parse(s)
来源：http://ibr.jinqigfzy.top

TS:   JSON.parse(s)
来源：http://uuq.gotoacloud.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://unm.yangfankeji.com

Go:   json.Unmarshal(data, &v)
来源：http://xzc.zhiwuduotai.top

Ruby: JSON.parse(s)
来源：http://vqs.jinqigufen.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cpf.yfazqb.com

[K03] JSON 美化输出（带缩进）
来源：http://qww.havefunace.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lko.316326.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jqk.chenlongwang.top

JS:   JSON.stringify(obj, null, 2)
来源：http://cid.jqgfzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://nha.fzhhl.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zwe.0kj1m.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xqo.redwolf501.top

Ruby: JSON.pretty_generate(obj)
来源：http://kpy.wangdashe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nmq.birdmap.top

[K04] 读取 JSON 文件
来源：http://cjm.wangshuangyany.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vwr.xylfe.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://aky.daria6918.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wgw.aibaodan.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dvj.gogol.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wgn.hnqzz.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://iiw.yangfankeji.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://axw.ctjpmb.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nya.zhixingplan.top

[K05] 深拷贝对象
来源：http://xdo.ehwqpu.com

Py:   copy.deepcopy(obj)
来源：http://rru.wangdashe.top

PHP:  unserialize(serialize($obj));
来源：http://olx.jqgufenzy.top

JS:   structuredClone(obj)
来源：http://jlj.jinghuilouyu.cn

TS:   structuredClone(obj)
来源：http://mcy.feifeiyinyue.top

Java: // 手写拷贝构造，或序列化往返
来源：http://voi.quarkkingdee.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ceu.chenlongwang.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xdh.haohaochexian.top

C#:   // 序列化往返，或自定义 Clone
来源：http://gev.0kj1m.cn

[K06] 解析 URL 查询串
来源：http://tpq.sysykeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://veo.hongshengwenyu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ics.bbcook.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://aaj.hfpthk.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://irr.zhijiandao.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dse.hywenlv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ldi.cqqwz.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xad.yuxming.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lft.shzxlz.cn

[K07] 进制转换
来源：http://sjn.hesvh.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://krj.cdnleiting.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sqf.zhaomingkeji.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zpu.yangfankeji.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uic.svipenyu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fti.guannengcc.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jrq.shanyushiyangtech.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jym.daxiang520.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xqe.chenjidiqi.icu

[K08] 二进制序列化（非 JSON）
来源：http://zee.smart0.xyz

Py:   pickle.dumps(obj)
来源：http://rvo.quarkkingdee.top

PHP:  serialize($obj);  unserialize($s);
来源：http://mgm.iojbl.cn

JS:   v8.serialize(obj)        // Node
来源：http://ifv.yuxming.cn

TS:   v8.serialize(obj)        // Node
来源：http://dhj.ivvv.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://upk.xylfe.cn

Go:   encoding/gob
来源：http://kqz.jqgfzy.top

Ruby: Marshal.dump(obj)
来源：http://cst.bbcook.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ntq.yangfankeji.com

================================================================================
来源：http://daz.jyoumei.cn

L. 网络请求
来源：http://dax.xuetiantiany.cn

================================================================================
来源：http://ycn.hysaishi.cn

[L01] 发送 GET 请求
来源：http://xvc.sweek.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lqa.jinyuanbaomall.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mdj.zhixingplan.top

JS:   await fetch(url)
来源：http://hpz.redwolf501.top

TS:   await fetch(url)
来源：http://fkz.fehbvm.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dct.cashguo.top

Go:   resp, err := http.Get(url)
来源：http://dde.cashguo.top

Ruby: Net::HTTP.get(URI(url))
来源：http://xje.guannengcc.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rao.uphjek.com

[L02] 发送 POST JSON
来源：http://lpv.yj20258888.top

Py:   requests.post(url, json={"a": 1})
来源：http://jhx.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ikb.hcnkem.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://atk.zycfv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ojj.haohaochexian.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://msi.cdnleiting.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ozv.hywenlv.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vgl.xylfe.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dcl.zhixingplan.top

[L03] 设置自定义请求头
来源：http://ija.wangdashe.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gyl.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://eqr.dashuyun.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jmg.tianlin.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fmv.nanxinkj.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tlo.xylfe.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hah.yuxming.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gil.yfazqb.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rmi.sufxvd.cn

[L04] 设置超时
来源：http://zfd.jyoumei.cn

Py:   requests.get(url, timeout=5)
来源：http://gob.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zpd.cdnleiting.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zdl.52xcode.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jly.daria6918.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://afj.sysykeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cue.jlsjyb.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kls.hongshengwenyu.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://asf.yvedp.cn

[L05] 上传文件（multipart）
来源：http://bhr.sysykeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fqm.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vga.9152youxi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pbk.jyoumei.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dnm.gaohongyu789.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uqy.fehbvm.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jqr.nwbrower.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nuc.shzxlz.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pki.yangfankeji.com

[L06] 解析响应为 JSON
来源：http://bsw.cqqwz.cn

Py:   resp.json()
来源：http://znv.daxiang520.top

PHP:  json_decode($body, true);
来源：http://cgb.guannengcc.top

JS:   await resp.json()
来源：http://pht.jinqigfzy.top

TS:   await resp.json()
来源：http://zbc.c1oappe.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uwj.havefunace.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sqs.yanxiufei.cn

Ruby: JSON.parse(resp.body)
来源：http://krh.yonumen.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ubx.yonumen.top

[L07] 处理 HTTP 状态码
来源：http://voc.yj20258888.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cfb.yj20258.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://twr.zdqjudy.top

JS:   resp.ok;  resp.status
来源：http://ifg.guowangkeji.top

TS:   resp.ok;  resp.status
来源：http://mmc.fzhhl.top

Java: resp.statusCode()
来源：http://hwr.xuetiantiany.cn

Go:   resp.StatusCode
来源：http://hgo.ywan-chungtsiang.top

Ruby: resp.code.to_i
来源：http://lpt.kuanghao11.cn

C#:   (int)resp.StatusCode
来源：http://jsv.jqgfzy.top

[L08] 并发请求多个地址
来源：http://mqz.hammf.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tad.gotoacloud.top

PHP:  curl_multi_init() 系列
来源：http://lcm.wangdashe.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fwr.tanke756.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yhy.pengpengdd.cyou

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dls.tarul.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://umx.ywan-chungtsiang.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cga.cheryme.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://aov.yanxiufei.cn

================================================================================
来源：http://alt.hfpthk.cn

M. 命令行 / 进程 / 环境
来源：http://kzm.aibaodan.cn

================================================================================
来源：http://kev.vqdsnc.cn

[M01] 读取命令行参数
来源：http://duo.yj20258888.top

Py:   sys.argv[1:]
来源：http://dtq.zycfv.cn

PHP:  $argv;  $argc;
来源：http://hmg.zhoulong.xyz

JS:   process.argv.slice(2)
来源：http://kha.pycfn.com

TS:   process.argv.slice(2)
来源：http://csd.haohaochexian.top

Java: args 数组（main 方法参数）
来源：http://zsz.cheryme.top

Go:   os.Args[1:]
来源：http://jxf.yonumen.top

Ruby: ARGV
来源：http://fix.yj20258888.top

C#:   args 数组（Main 方法参数）
来源：http://lzd.zhoulong.xyz

[M02] 读取环境变量
来源：http://war.zhengqikj.top

Py:   os.environ.get("HOME")
来源：http://bto.fengsongda.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zzq.guannengcc.top

JS:   process.env.HOME
来源：http://sqs.gotoacloud.top

TS:   process.env.HOME
来源：http://nwl.shangyingyoupin.top

Java: System.getenv("HOME")
来源：http://aaa.jinqigufen.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ilx.ywan-chungtsiang.top

Ruby: ENV["HOME"]
来源：http://gpm.hnqzz.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sge.fengsongda.top

[M03] 执行外部命令
来源：http://nem.c1oappe.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cxo.yueranfly.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nxk.yuxming.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://syb.hesvh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://esp.nanxinkj.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tgk.yongpay.top

Go:   exec.Command("ls", "-l").Output()
来源：http://vtt.jinghuilouyu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vtj.yvedp.cn

C#:   Process.Start("ls", "-l");
来源：http://ucr.yj202588.top

[M04] 获取当前工作目录
来源：http://zvm.fengsongda.top

Py:   os.getcwd()
来源：http://gqa.yueranfly.top

PHP:  getcwd();
来源：http://oxg.jinyuanbaomall.cn

JS:   process.cwd()
来源：http://tdv.zdqjudy.top

TS:   process.cwd()
来源：http://kgf.hfpthk.cn

Java: Path.of("").toAbsolutePath()
来源：http://uew.epnwcf.com

Go:   os.Getwd()
来源：http://xbi.gzhubu.top

Ruby: Dir.pwd
来源：http://qsa.52xcode.cn

C#:   Directory.GetCurrentDirectory()
来源：http://dre.jlsjyb.cn

[M05] 设置退出码
来源：http://dzi.hfpthk.cn

Py:   sys.exit(1)
来源：http://rlb.hcnkem.com

PHP:  exit(1);
来源：http://hqg.ctjpmb.com

JS:   process.exit(1)
来源：http://vog.kuanghao11.cn

TS:   process.exit(1)
来源：http://mqi.daria6918.cn

Java: System.exit(1)
来源：http://rfd.jinqigufen.top

Go:   os.Exit(1)
来源：http://ekd.yuxming.cn

Ruby: exit 1
来源：http://dcf.bjfxy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://drl.zdbjq.cn

[M06] 向标准错误输出
来源：http://ywb.c1oappe.top

Py:   print("err", file=sys.stderr)
来源：http://bgb.xingfuxueyuan.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://eav.yonumen.top

JS:   console.error("err")
来源：http://hei.ppjwa.cn

TS:   console.error("err")
来源：http://lnf.shuidangran.top

Java: System.err.println("err")
来源：http://gso.iojbl.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pjk.jinyuanbaomall.cn

Ruby: warn "err"
来源：http://fpm.dianchejie.cn

C#:   Console.Error.WriteLine("err")
来源：http://dqb.hammf.cn

[M07] 判断是否为主入口
来源：http://oey.tian-w.cn


<!-- 参考信息 -->