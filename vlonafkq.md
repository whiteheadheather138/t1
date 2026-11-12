代发 wailian999

J. 日期与时间
来源：http://ztx.xingfuxueyuan.xyz

================================================================================
来源：http://sjx.hnxiangtu.top

[J01] 获取当前时间
来源：http://vxe.hongshengwenyu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://bqc.tanke756.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://omn.fzhhl.top

JS:   new Date();  Date.now()
来源：http://dyz.zycfv.cn

TS:   new Date();  Date.now()
来源：http://ocq.yanxiufei.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pty.epnwcf.com

Go:   time.Now()
来源：http://yzp.guowangkeji.top

Ruby: Time.now
来源：http://ict.shangyingyoupin.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ztt.epnwcf.com

[J02] 格式化输出
来源：http://vpy.gogol.net.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uec.ehwqpu.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://due.hywenlv.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jwu.tianlin.xyz

TS:   d.toISOString()
来源：http://saq.dashuyun.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ghd.zhaomingkeji.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rnq.hesvh.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vae.gogol.net.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bpy.yangfankeji.com

[J03] 字符串解析为日期
来源：http://bdp.yj20258.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://krg.zhongyouzk.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ejj.sufxvd.cn

JS:   new Date("2024-01-02")
来源：http://efi.redwolf501.top

TS:   new Date("2024-01-02")
来源：http://gxi.shangyingyoupin.top

Java: LocalDate.parse("2024-01-02")
来源：http://pmm.hnxiangtu.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cwr.smart0.xyz

Ruby: Date.parse("2024-01-02")
来源：http://wgk.sxryk.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wcs.vqdsnc.cn

[J04] 时间戳与日期互转
来源：http://qjc.svipenyu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cjn.chenjidiqi.icu

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cui.xuetiantiany.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ewp.quarkkingdee.top

TS:   Math.floor(Date.now() / 1000)
来源：http://lnw.guowangkeji.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ifr.andypj.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qqu.zhixingplan.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uno.c1oappe.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wga.gzhubu.top

[J05] 时间加减（加 7 天）
来源：http://amr.cqqwz.cn

Py:   now + timedelta(days=7)
来源：http://ecp.guannengcc.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://vaf.yj20258.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jfl.sxryk.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tmn.kuanghao11.cn

Java: LocalDate.now().plusDays(7)
来源：http://nui.yangfankeji.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ihy.vqdsnc.cn

Ruby: Time.now + 7 * 86400
来源：http://mvw.pengpengdd.cyou

C#:   DateTime.Now.AddDays(7)
来源：http://bgc.gotoacloud.top

[J06] 计算两时间之差
来源：http://yqe.c1oappe.top

Py:   (end - start).total_seconds()
来源：http://qno.fktsv.cn

PHP:  $end->diff($start)->days;
来源：http://vqg.nanxuanxn.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rdc.yj20258888.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mnu.hysaishi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vrf.aizwys.cn

Go:   end.Sub(start).Hours()
来源：http://vso.sjlbkw.cn

Ruby: end - start                 # 返回秒数
来源：http://msv.gogol.net.cn

C#:   (end - start).TotalSeconds
来源：http://gsx.jyoumei.cn

[J07] 比较两个日期
来源：http://ysq.jianghu66.top

Py:   d1 < d2;  d1 == d2
来源：http://gab.zhongyouzk.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tdo.ydzc1.top

JS:   d1.getTime() < d2.getTime()
来源：http://zxj.jinqigfzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://bqq.ydjk.org.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lvk.quarkkingdee.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uqv.zhaomingkeji.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://mns.sxryk.cn

C#:   d1 < d2;  d1 == d2
来源：http://omb.jqgfzy.top

[J08] 提取年月日与星期
来源：http://oai.tianlin.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mgj.gzhubu.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fyg.tarul.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lbo.ydzc1.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qcg.fengsongda.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ppn.zdqjudy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sjq.zhaomingkeji.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dek.wangdashe.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ifb.ehwqpu.com

[J09] 时区处理
来源：http://lyw.316326.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kna.hysaishi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gus.epnwcf.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yhs.tarul.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fmh.ctjpmb.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kqb.ppjwa.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ncr.hnqzz.top

Ruby: Time.now.getlocal("+08:00")
来源：http://uid.yanxiufei.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gcr.tian-w.cn

[J10] 取今天 / 本月第一天
来源：http://btq.vehdjk.com

Py:   date.today();  date.today().replace(day=1)
来源：http://mok.svipenyu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sgk.sweek.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vyg.hcnkem.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ccf.nwbrower.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tkm.yj202588.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jed.316326.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cax.cheryme.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gcu.xuetiantiany.cn

================================================================================
来源：http://yaz.yj20258888.top

K. JSON 与序列化
来源：http://ora.bbcook.cn

================================================================================
来源：http://lni.pycfn.com

[K01] 对象转 JSON 字符串
来源：http://lsq.nanxinkj.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ule.snrcjt.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pou.sysykeji.top

JS:   JSON.stringify(obj)
来源：http://yfh.yonumen.top

TS:   JSON.stringify(obj)
来源：http://bbk.gaohongyu789.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cuo.dianchejie.cn

Go:   json.Marshal(obj)
来源：http://sns.hesvh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hrn.yj202588.top

C#:   JsonSerializer.Serialize(obj)
来源：http://doc.nwbrower.top

[K02] JSON 字符串转对象
来源：http://hwh.aibaodan.cn

Py:   json.loads(s)
来源：http://maj.ivvv.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://faw.yuanzhike.top

JS:   JSON.parse(s)
来源：http://vaw.pycfn.com

TS:   JSON.parse(s)
来源：http://ukb.feifeiyinyue.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ayy.xylfe.cn

Go:   json.Unmarshal(data, &v)
来源：http://lpz.mhx1999.top

Ruby: JSON.parse(s)
来源：http://bso.jqgfzy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rcx.hammf.cn

[K03] JSON 美化输出（带缩进）
来源：http://von.ctjpmb.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mpg.daria6918.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://spw.zhiwuduotai.top

JS:   JSON.stringify(obj, null, 2)
来源：http://vsb.aibaodan.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ado.gzhubu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xkq.fktsv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ypz.xuetiantiany.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jlj.cdnleiting.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://unc.svipenyu.cn

[K04] 读取 JSON 文件
来源：http://gkb.shanyushiyangkeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://znb.nwbrower.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rok.guowangkeji.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lwc.cheryme.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lix.hnxiangtu.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pwu.cqqwz.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jkf.zhixingplan.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://cyu.hcnkem.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ilr.hongshengwenyu.top

[K05] 深拷贝对象
来源：http://slh.vqdsnc.cn

Py:   copy.deepcopy(obj)
来源：http://hsm.fzhhl.top

PHP:  unserialize(serialize($obj));
来源：http://ugf.hongshengwenyu.top

JS:   structuredClone(obj)
来源：http://dxo.cashguo.top

TS:   structuredClone(obj)
来源：http://vwi.yongpay.top

Java: // 手写拷贝构造，或序列化往返
来源：http://yio.xuanzx.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bow.sysykeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://feo.fehbvm.com

C#:   // 序列化往返，或自定义 Clone
来源：http://ldp.zhongyouzk.top

[K06] 解析 URL 查询串
来源：http://zyo.dashuyun.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tmr.gotoacloud.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dce.jinghuilouyu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sos.shanyushiyangtech.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qqo.guowangkeji.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://aer.ywan-chungtsiang.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://arq.haohaochexian.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mas.zhijiandao.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gcw.ywan-chungtsiang.top

[K07] 进制转换
来源：http://xju.ivvv.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hhs.yuanzhike.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sdl.tian-w.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://djr.hammf.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gcw.shuidangran.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://oeb.nanxuanxn.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://muc.hnxiangtu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cxv.shzxlz.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xna.yuxming.cn

[K08] 二进制序列化（非 JSON）
来源：http://amo.shanyushiyangkeji.top

Py:   pickle.dumps(obj)
来源：http://wym.nwbrower.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ccc.ehwqpu.com

JS:   v8.serialize(obj)        // Node
来源：http://epi.zhiwuduotai.top

TS:   v8.serialize(obj)        // Node
来源：http://qgf.cqqwz.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://apy.jqgufenzy.top

Go:   encoding/gob
来源：http://vyf.andypj.xyz

Ruby: Marshal.dump(obj)
来源：http://nia.dashuyun.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qqd.ivvv.top

================================================================================
来源：http://mvw.dashuyun.cn

L. 网络请求
来源：http://ofq.cdnleiting.top

================================================================================
来源：http://sqg.tianlin.xyz

[L01] 发送 GET 请求
来源：http://tvj.wangdashe.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qyi.feifeiyinyue.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://klc.jinghuilouyu.cn

JS:   await fetch(url)
来源：http://bqk.ydjk.org.cn

TS:   await fetch(url)
来源：http://vzy.wangdashe.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gre.gzhubu.top

Go:   resp, err := http.Get(url)
来源：http://iua.jinqigfzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://kjo.jinghuilouyu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rrl.zhixingplan.top

[L02] 发送 POST JSON
来源：http://lws.vehdjk.com

Py:   requests.post(url, json={"a": 1})
来源：http://jgv.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yzm.52xcode.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hfv.xuanzx.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dyq.epnwcf.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ymq.hysaishi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qrf.yangfankeji.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://psb.bjfxy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zuy.52xcode.cn

[L03] 设置自定义请求头
来源：http://hbi.zhengqikj.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wat.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bnl.zhengqikj.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yyb.ehwqpu.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lgq.fehbvm.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hfl.andypj.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ifd.hywenlv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://itv.uphjek.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jou.fengsongda.top

[L04] 设置超时
来源：http://lhv.mhx1999.top

Py:   requests.get(url, timeout=5)
来源：http://qdn.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://drc.cashguo.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sum.ivvv.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gfg.shuidangran.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qad.yj202588.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jwt.pengpengdd.cyou

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lez.ppjwa.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lup.uphjek.com

[L05] 上传文件（multipart）
来源：http://hle.chenjidiqi.icu

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kgn.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xnl.yonumen.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lbf.tanke756.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jai.xinyue.icu

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qge.yuanzhike.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cqm.redwolf501.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ugi.zhixingplan.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pie.gotoacloud.top

[L06] 解析响应为 JSON
来源：http://hvb.shuidangran.top

Py:   resp.json()
来源：http://vaw.quarkkingdee.top

PHP:  json_decode($body, true);
来源：http://aka.xingfuxueyuan.xyz

JS:   await resp.json()
来源：http://obi.ywan-chungtsiang.top

TS:   await resp.json()
来源：http://pkf.havefunace.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nrt.nwbrower.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hhx.fengsongda.top

Ruby: JSON.parse(resp.body)
来源：http://pmq.cdnleiting.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ysi.cqqwz.cn

[L07] 处理 HTTP 状态码
来源：http://frv.meibo888.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bmn.meibo888.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pcz.ivvv.top

JS:   resp.ok;  resp.status
来源：http://trl.fengsongda.top

TS:   resp.ok;  resp.status
来源：http://duw.nanxinkj.top

Java: resp.statusCode()
来源：http://yky.iojbl.cn

Go:   resp.StatusCode
来源：http://shd.jyoumei.cn

Ruby: resp.code.to_i
来源：http://ugy.jlsjyb.cn

C#:   (int)resp.StatusCode
来源：http://kdi.tian-w.cn

[L08] 并发请求多个地址
来源：http://gqr.xinyue.icu

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qdr.pycfn.com

PHP:  curl_multi_init() 系列
来源：http://tgs.yueranfly.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qtr.shanyushiyangtech.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://arb.zhaomingkeji.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://npe.ppjwa.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jkh.zhixingplan.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://eie.cashguo.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://spg.guannengcc.top

================================================================================
来源：http://ove.yonumen.top

M. 命令行 / 进程 / 环境
来源：http://gmy.yongpay.top

================================================================================
来源：http://zea.sxryk.cn

[M01] 读取命令行参数
来源：http://tyu.uphjek.com

Py:   sys.argv[1:]
来源：http://grj.zhiwuduotai.top

PHP:  $argv;  $argc;
来源：http://jyx.shanyushiyangkeji.top

JS:   process.argv.slice(2)
来源：http://lty.nwbrower.top

TS:   process.argv.slice(2)
来源：http://vhp.tarul.cn

Java: args 数组（main 方法参数）
来源：http://rdo.feifeiyinyue.top

Go:   os.Args[1:]
来源：http://qqx.vehdjk.com

Ruby: ARGV
来源：http://fot.svipenyu.cn

C#:   args 数组（Main 方法参数）
来源：http://uud.shzxlz.cn

[M02] 读取环境变量
来源：http://slh.ydjk.org.cn

Py:   os.environ.get("HOME")
来源：http://qgz.uphjek.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rsg.sufxvd.cn

JS:   process.env.HOME
来源：http://fdy.ydzc1.top

TS:   process.env.HOME
来源：http://apl.jinyuanbaomall.cn

Java: System.getenv("HOME")
来源：http://wtp.jqgufenzy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ymo.hysaishi.cn

Ruby: ENV["HOME"]
来源：http://xyv.uphjek.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lhb.zycfv.cn

[M03] 执行外部命令
来源：http://fii.52xcode.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kpf.nwbrower.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://btc.jyoumei.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://htg.chenzaomai.com

TS:   child_process.execSync("ls -l").toString()
来源：http://xgg.yuxming.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jtq.dianchejie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hwn.yueranfly.top

Ruby: system("ls -l");  `ls -l`
来源：http://zui.chenlongwang.top

C#:   Process.Start("ls", "-l");
来源：http://dwh.shanyushiyangtech.top

[M04] 获取当前工作目录
来源：http://uah.gaohongyu789.top

Py:   os.getcwd()
来源：http://amw.daxiang520.top

PHP:  getcwd();
来源：http://qte.tarul.cn

JS:   process.cwd()
来源：http://nuh.cashguo.top

TS:   process.cwd()
来源：http://npe.nwbrower.top

Java: Path.of("").toAbsolutePath()
来源：http://aoo.aibaodan.cn

Go:   os.Getwd()
来源：http://gbk.hcnkem.com

Ruby: Dir.pwd
来源：http://rii.nanxinkj.top

C#:   Directory.GetCurrentDirectory()
来源：http://kfq.zhaomingkeji.xyz

[M05] 设置退出码
来源：http://seb.xuanzx.com

Py:   sys.exit(1)
来源：http://klt.hnqzz.top

PHP:  exit(1);
来源：http://dhv.mhx1999.top

JS:   process.exit(1)
来源：http://qmi.zycfv.cn

TS:   process.exit(1)
来源：http://soc.jlsjyb.cn

Java: System.exit(1)
来源：http://soa.aizwys.cn

Go:   os.Exit(1)
来源：http://dbk.zycfv.cn

Ruby: exit 1
来源：http://fgw.jinghuilouyu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ids.jinqigufen.top

[M06] 向标准错误输出
来源：http://duv.quarkkingdee.top

Py:   print("err", file=sys.stderr)
来源：http://qoj.bbcook.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pnz.aizwys.cn

JS:   console.error("err")
来源：http://avi.zhoulong.xyz

TS:   console.error("err")
来源：http://dyp.zycfv.cn

Java: System.err.println("err")
来源：http://alq.hnqzz.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vvc.sysykeji.top

Ruby: warn "err"
来源：http://xax.hywenlv.cn

C#:   Console.Error.WriteLine("err")
来源：http://cep.cashguo.top

[M07] 判断是否为主入口
来源：http://dxt.yanxiufei.cn


<!-- 参考信息 -->