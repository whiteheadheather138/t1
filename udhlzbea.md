代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fcy.haohaochexian.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mso.dianchejie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jcv.vqdsnc.cn

================================================================================
来源：http://dff.havefunace.top

J. 日期与时间
来源：http://abh.cucudq.cn

================================================================================
来源：http://xua.jinyuanbaomall.cn

[J01] 获取当前时间
来源：http://tiq.zycfv.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vph.cashguo.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://iqh.yongpay.top

JS:   new Date();  Date.now()
来源：http://yay.bjfxy.top

TS:   new Date();  Date.now()
来源：http://fob.gotoacloud.top

Java: LocalDateTime.now();  Instant.now()
来源：http://smh.cashguo.top

Go:   time.Now()
来源：http://sak.dashuyun.cn

Ruby: Time.now
来源：http://dmi.c1oappe.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jpe.chenlongwang.top

[J02] 格式化输出
来源：http://iaz.redwolf501.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dfv.pengpengdd.cyou

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ryq.zhiwuduotai.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xto.nanxuanxn.top

TS:   d.toISOString()
来源：http://sxm.ydzc1.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://noe.yuanzhike.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://udu.hcnkem.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xui.pycfn.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rmh.bjfxy.top

[J03] 字符串解析为日期
来源：http://ylx.cucudq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://doj.uphjek.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://eqo.jqgfzy.top

JS:   new Date("2024-01-02")
来源：http://ulo.kuanghao11.cn

TS:   new Date("2024-01-02")
来源：http://whv.gogol.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://llw.c1oappe.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lze.jinqigufen.top

Ruby: Date.parse("2024-01-02")
来源：http://yln.ctjpmb.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tmh.fktsv.cn

[J04] 时间戳与日期互转
来源：http://uvo.dianchejie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zcn.ywan-chungtsiang.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://abi.sysykeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ddn.jinyuanbaomall.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vjj.tianlin.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hux.yj20258888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://egr.jinqigufen.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ygx.jyoumei.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ima.yangfankeji.com

[J05] 时间加减（加 7 天）
来源：http://aaa.zhiwuduotai.top

Py:   now + timedelta(days=7)
来源：http://bjx.jinqigfzy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://iwe.meibo888.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://azi.pycfn.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nqj.c1oappe.top

Java: LocalDate.now().plusDays(7)
来源：http://hfl.316326.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gta.zhoulong.xyz

Ruby: Time.now + 7 * 86400
来源：http://ndw.shuidangran.top

C#:   DateTime.Now.AddDays(7)
来源：http://rgr.yangfankeji.com

[J06] 计算两时间之差
来源：http://gho.yuxming.cn

Py:   (end - start).total_seconds()
来源：http://rdk.9152youxi.cn

PHP:  $end->diff($start)->days;
来源：http://kuo.jianghu66.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ifb.smart0.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jvz.ywan-chungtsiang.top

Java: Duration.between(start, end).toSeconds()
来源：http://pgv.yongpay.top

Go:   end.Sub(start).Hours()
来源：http://olf.shuidangran.top

Ruby: end - start                 # 返回秒数
来源：http://tro.daxiang520.top

C#:   (end - start).TotalSeconds
来源：http://ctl.jyoumei.cn

[J07] 比较两个日期
来源：http://apk.ppjwa.cn

Py:   d1 < d2;  d1 == d2
来源：http://okc.daxiang520.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dya.hfpthk.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dzt.sysykeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://kjv.fanxiaobao.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zmm.xuetiantiany.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://orx.tian-w.cn

Ruby: d1 < d2;  d1 == d2
来源：http://als.yanxiufei.cn

C#:   d1 < d2;  d1 == d2
来源：http://fpu.nwbrower.top

[J08] 提取年月日与星期
来源：http://gre.yueranfly.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fqc.yonumen.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nif.aizwys.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kyf.yueranfly.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fzw.zdqjudy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jwp.shangyingyoupin.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uke.gaohongyu789.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dlt.meibo888.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yzc.xylfe.cn

[J09] 时区处理
来源：http://wnp.yangfankeji.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xxz.andypj.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tcp.c1oappe.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tkg.zhongyouzk.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://krt.sufxvd.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qdg.sufxvd.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tou.shanyushiyangtech.top

Ruby: Time.now.getlocal("+08:00")
来源：http://fos.yvedp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qxb.fanxiaobao.xyz

[J10] 取今天 / 本月第一天
来源：http://gdq.hfpthk.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ooz.nanxinkj.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xqu.shzxlz.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zax.wangdashe.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xid.smart0.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yyo.xuetiantiany.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jqj.tarul.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tzw.quarkkingdee.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qhr.uphjek.com

================================================================================
来源：http://fld.ehwqpu.com

K. JSON 与序列化
来源：http://hzy.sufxvd.cn

================================================================================
来源：http://kxb.smart0.xyz

[K01] 对象转 JSON 字符串
来源：http://xnv.cucudq.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yff.hnqzz.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dyw.shanyushiyangkeji.top

JS:   JSON.stringify(obj)
来源：http://iww.9152youxi.cn

TS:   JSON.stringify(obj)
来源：http://ysq.yj20258.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hex.xuanzx.com

Go:   json.Marshal(obj)
来源：http://www.yvedp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://tzw.bjfxy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://jxn.zhijiandao.cn

[K02] JSON 字符串转对象
来源：http://bwv.gogol.net.cn

Py:   json.loads(s)
来源：http://dbt.yuxming.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rpy.redwolf501.top

JS:   JSON.parse(s)
来源：http://wpp.tian-w.cn

TS:   JSON.parse(s)
来源：http://ajs.fengsongda.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://opn.hongshengwenyu.top

Go:   json.Unmarshal(data, &v)
来源：http://imp.ydjk.org.cn

Ruby: JSON.parse(s)
来源：http://dto.tanke756.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://niy.aizwys.cn

[K03] JSON 美化输出（带缩进）
来源：http://rha.cqqwz.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ktk.yj20258.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vsm.hysaishi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qip.ydjk.org.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mbb.xuetiantiany.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wza.ppjwa.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rtd.pengpengdd.cyou

Ruby: JSON.pretty_generate(obj)
来源：http://ghw.wangdashe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://iik.yangfankeji.com

[K04] 读取 JSON 文件
来源：http://rvk.316326.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zas.cqqwz.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vhw.aibaodan.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dxz.cheryme.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jrp.guowangkeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sjg.hesvh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ogl.jinghuilouyu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dmv.yfazqb.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wum.ywan-chungtsiang.top

[K05] 深拷贝对象
来源：http://yxu.mhx1999.top

Py:   copy.deepcopy(obj)
来源：http://uxw.ydjk.org.cn

PHP:  unserialize(serialize($obj));
来源：http://zzk.quarkkingdee.top

JS:   structuredClone(obj)
来源：http://mdo.ybcxt.top

TS:   structuredClone(obj)
来源：http://ivf.shzxlz.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cee.ctjpmb.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fyj.daxiang520.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sks.jyoumei.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ule.jlsjyb.cn

[K06] 解析 URL 查询串
来源：http://poh.bjfxy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cxb.0kj1m.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mnu.hfpthk.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://crx.nanxuanxn.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tis.fzhhl.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zqc.hongshengwenyu.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ksj.zhiwuduotai.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hgc.fehbvm.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qxt.yuxming.cn

[K07] 进制转换
来源：http://qji.feifeiyinyue.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mml.shanyushiyangtech.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zyx.jiagoushi.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lco.hfpthk.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qxq.feifeiyinyue.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lvp.xziqi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bol.shanyushiyangtech.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dgq.ywan-chungtsiang.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vyp.wangshuangyany.cn

[K08] 二进制序列化（非 JSON）
来源：http://yzt.shangyingyoupin.top

Py:   pickle.dumps(obj)
来源：http://eer.bbcook.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gsh.meibo888.top

JS:   v8.serialize(obj)        // Node
来源：http://ohq.hcnkem.com

TS:   v8.serialize(obj)        // Node
来源：http://iwx.meibo888.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bei.fengsongda.top

Go:   encoding/gob
来源：http://prq.bbcook.cn

Ruby: Marshal.dump(obj)
来源：http://fup.fanxiaobao.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://miw.tarul.cn

================================================================================
来源：http://mfd.hywenlv.cn

L. 网络请求
来源：http://mek.yanxiufei.cn

================================================================================
来源：http://iwf.kuanghao11.cn

[L01] 发送 GET 请求
来源：http://psl.xziqi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cbx.chenlongwang.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fqc.bbcook.cn

JS:   await fetch(url)
来源：http://dbx.yanxiufei.cn

TS:   await fetch(url)
来源：http://vjf.yj202588.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pwm.cucudq.cn

Go:   resp, err := http.Get(url)
来源：http://gbk.xuanzx.com

Ruby: Net::HTTP.get(URI(url))
来源：http://uqi.feifeiyinyue.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tqt.cheryme.top

[L02] 发送 POST JSON
来源：http://lke.jqgufenzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://tca.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qqv.dianchejie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://box.tianlin.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pex.tarul.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://iwz.jinqigfzy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uiz.hnxiangtu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://afk.gaohongyu789.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sqk.ydjk.org.cn

[L03] 设置自定义请求头
来源：http://jtl.jinyuanbaomall.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ioo.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wsq.snrcjt.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pxz.sufxvd.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qpb.yongpay.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rie.hywenlv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fas.zhijiandao.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jtg.daxiang520.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sbj.yongpay.top

[L04] 设置超时
来源：http://mci.xingfuxueyuan.xyz

Py:   requests.get(url, timeout=5)
来源：http://ilv.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nvw.nanxuanxn.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tdm.chenjidiqi.icu

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uhc.smart0.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jnx.yj20258888.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://myp.aibaodan.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qqc.kuanghao11.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cuy.hnqzz.top

[L05] 上传文件（multipart）
来源：http://oqf.xinyue.icu

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://til.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pee.fzhhl.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://guo.birdmap.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://agf.zhengqikj.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lyf.birdmap.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vnt.jyoumei.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xoo.ybcxt.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wyg.vehdjk.com

[L06] 解析响应为 JSON
来源：http://uei.yj202588.top

Py:   resp.json()
来源：http://nnk.hywenlv.cn

PHP:  json_decode($body, true);
来源：http://rdn.cqqwz.cn

JS:   await resp.json()
来源：http://znr.sufxvd.cn

TS:   await resp.json()
来源：http://fny.zdqjudy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dnh.zhengqikj.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ujy.dashuyun.cn

Ruby: JSON.parse(resp.body)
来源：http://ifl.yvedp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hha.cashguo.top

[L07] 处理 HTTP 状态码
来源：http://bzx.andypj.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hjc.yj202588.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qjd.jianghu66.top

JS:   resp.ok;  resp.status
来源：http://nyb.iojbl.cn

TS:   resp.ok;  resp.status
来源：http://lub.ydzc1.top

Java: resp.statusCode()
来源：http://tjg.wangdashe.top

Go:   resp.StatusCode
来源：http://ptc.yj202588.top

Ruby: resp.code.to_i
来源：http://yxp.snrcjt.cn

C#:   (int)resp.StatusCode
来源：http://yle.shanyushiyangtech.top

[L08] 并发请求多个地址
来源：http://qiv.yanxiufei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rac.uphjek.com

PHP:  curl_multi_init() 系列
来源：http://jqz.gotoacloud.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eov.zdqjudy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kjj.shangyingyoupin.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://odd.nwbrower.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rcj.sweek.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://iba.jqgfzy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cum.yj20258.top

================================================================================
来源：http://ebq.smart0.xyz

M. 命令行 / 进程 / 环境
来源：http://qpf.aibaodan.cn

================================================================================
来源：http://hhj.zhoulong.xyz

[M01] 读取命令行参数
来源：http://hqw.shanyushiyangtech.top

Py:   sys.argv[1:]
来源：http://iew.meibo888.top

PHP:  $argv;  $argc;
来源：http://rta.c1oappe.top

JS:   process.argv.slice(2)
来源：http://fpj.shanyushiyangtech.top

TS:   process.argv.slice(2)
来源：http://cyb.gotoacloud.top

Java: args 数组（main 方法参数）
来源：http://rdo.uphjek.com

Go:   os.Args[1:]
来源：http://xoq.redwolf501.top

Ruby: ARGV
来源：http://zzz.quarkkingdee.top

C#:   args 数组（Main 方法参数）
来源：http://nye.meibo888.top

[M02] 读取环境变量
来源：http://yry.ivvv.top

Py:   os.environ.get("HOME")
来源：http://gjc.xziqi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mcd.yanxiufei.cn

JS:   process.env.HOME
来源：http://ium.fktsv.cn

TS:   process.env.HOME
来源：http://vlt.chenlongwang.top

Java: System.getenv("HOME")
来源：http://rmd.tarul.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hjq.zhengqikj.top

Ruby: ENV["HOME"]
来源：http://jvx.uphjek.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zta.sweek.top

[M03] 执行外部命令
来源：http://lyp.gogol.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://prr.shangyingyoupin.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ugv.jqgfzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://nic.ydjk.org.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xnq.bbcook.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kwr.chenjidiqi.icu

Go:   exec.Command("ls", "-l").Output()
来源：http://cqe.tian-w.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fxx.xingfuxueyuan.xyz

C#:   Process.Start("ls", "-l");
来源：http://ixw.pengpengdd.cyou

[M04] 获取当前工作目录
来源：http://sms.jinyuanbaomall.cn

Py:   os.getcwd()
来源：http://pxu.jinghuilouyu.cn

PHP:  getcwd();
来源：http://udb.aibaodan.cn

JS:   process.cwd()
来源：http://dgc.xuanzx.com

TS:   process.cwd()
来源：http://qet.guowangkeji.top

Java: Path.of("").toAbsolutePath()
来源：http://aat.tarul.cn

Go:   os.Getwd()
来源：http://fpj.yonumen.top

Ruby: Dir.pwd
来源：http://ecg.jqgufenzy.top

C#:   Directory.GetCurrentDirectory()
来源：http://xjl.havefunace.top

[M05] 设置退出码
来源：http://ilw.ctjpmb.com

Py:   sys.exit(1)
来源：http://hra.daxiang520.top

PHP:  exit(1);
来源：http://qas.zhijiandao.cn

JS:   process.exit(1)
来源：http://jal.jqgfzy.top

TS:   process.exit(1)
来源：http://kfo.guannengcc.top

Java: System.exit(1)
来源：http://hvp.cashguo.top

Go:   os.Exit(1)
来源：http://aua.ydzc1.top

Ruby: exit 1
来源：http://xdb.gaohongyu789.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://iov.yj20258888.top

[M06] 向标准错误输出
来源：http://soq.shzxlz.cn

Py:   print("err", file=sys.stderr)
来源：http://qib.tarul.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ijv.birdmap.top

JS:   console.error("err")
来源：http://oge.cashguo.top

TS:   console.error("err")
来源：http://ase.gaohongyu789.top

Java: System.err.println("err")
来源：http://fsq.aizwys.cn


<!-- 参考信息 -->