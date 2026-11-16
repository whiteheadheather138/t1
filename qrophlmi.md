代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zos.meibo888.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bip.316326.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kwh.yj20258888.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://tjz.dashuyun.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://col.chenlongwang.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tym.wangdashe.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dms.cucudq.cn

================================================================================
来源：http://djl.yongpay.top

J. 日期与时间
来源：http://qpt.smart0.xyz

================================================================================
来源：http://pxz.shanyushiyangtech.top

[J01] 获取当前时间
来源：http://zpj.yj20258.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://snv.bbcook.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ejh.ybcxt.top

JS:   new Date();  Date.now()
来源：http://sou.tianlin.xyz

TS:   new Date();  Date.now()
来源：http://vxg.jinyuanbaomall.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://sxq.fengsongda.top

Go:   time.Now()
来源：http://lad.dashuyun.cn

Ruby: Time.now
来源：http://jss.nanxuanxn.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lng.hnxiangtu.top

[J02] 格式化输出
来源：http://hma.dashuyun.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oku.feifeiyinyue.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://onh.zhixingplan.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bmy.jlsjyb.cn

TS:   d.toISOString()
来源：http://yql.yangfankeji.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cea.dashuyun.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://aey.jlsjyb.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dxy.hongshengwenyu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://phh.ydjk.org.cn

[J03] 字符串解析为日期
来源：http://xmv.xingfuxueyuan.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jhk.yj20258.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://alu.gaohongyu789.top

JS:   new Date("2024-01-02")
来源：http://xkk.ywan-chungtsiang.top

TS:   new Date("2024-01-02")
来源：http://syz.shanyushiyangkeji.top

Java: LocalDate.parse("2024-01-02")
来源：http://uab.pycfn.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://boa.gzhubu.top

Ruby: Date.parse("2024-01-02")
来源：http://dvj.zdqjudy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://szb.epnwcf.com

[J04] 时间戳与日期互转
来源：http://wsk.sufxvd.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pna.ehwqpu.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cwe.uphjek.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ozf.yuxming.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wuk.pycfn.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://brf.jiagoushi.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jxd.zdbjq.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vhb.svipenyu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ppi.birdmap.top

[J05] 时间加减（加 7 天）
来源：http://xmp.nanxinkj.top

Py:   now + timedelta(days=7)
来源：http://sfp.ctjpmb.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://gvj.yangfankeji.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uvc.gzhubu.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gul.chenlongwang.top

Java: LocalDate.now().plusDays(7)
来源：http://bbr.sweek.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ppg.ydzc1.top

Ruby: Time.now + 7 * 86400
来源：http://rdm.jqgufenzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://joj.gotoacloud.top

[J06] 计算两时间之差
来源：http://okr.sysykeji.top

Py:   (end - start).total_seconds()
来源：http://njv.nwbrower.top

PHP:  $end->diff($start)->days;
来源：http://xmn.xuanzx.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zut.uphjek.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pmz.yj20258888.top

Java: Duration.between(start, end).toSeconds()
来源：http://qzz.aizwys.cn

Go:   end.Sub(start).Hours()
来源：http://yvj.hcnkem.com

Ruby: end - start                 # 返回秒数
来源：http://upk.gotoacloud.top

C#:   (end - start).TotalSeconds
来源：http://vwu.cdnleiting.top

[J07] 比较两个日期
来源：http://rlg.ybcxt.top

Py:   d1 < d2;  d1 == d2
来源：http://ula.shanyushiyangkeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pux.nanxuanxn.top

JS:   d1.getTime() < d2.getTime()
来源：http://gna.havefunace.top

TS:   d1.getTime() < d2.getTime()
来源：http://sxt.fanxiaobao.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://szo.yonumen.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://slo.vqdsnc.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zpc.chenjidiqi.icu

C#:   d1 < d2;  d1 == d2
来源：http://nnu.yuanzhike.top

[J08] 提取年月日与星期
来源：http://cay.gzhubu.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ulb.iojbl.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vyi.yueranfly.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://eop.snrcjt.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uvw.zdbjq.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ral.jqgufenzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xjb.jinqigfzy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ymc.ydjk.org.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nkb.aizwys.cn

[J09] 时区处理
来源：http://hid.shzxlz.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cbk.smart0.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yez.ywan-chungtsiang.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://adt.zhaomingkeji.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bbx.bjfxy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zej.tianlin.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tqj.guowangkeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://pwp.zhaomingkeji.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://skn.sysykeji.top

[J10] 取今天 / 本月第一天
来源：http://jtm.tanke756.top

Py:   date.today();  date.today().replace(day=1)
来源：http://wed.sxryk.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://roo.yuxming.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ruj.fengsongda.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kqw.shuidangran.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qoi.9152youxi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sna.sysykeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zeq.jqgufenzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lrx.xuetiantiany.cn

================================================================================
来源：http://ufu.jlsjyb.cn

K. JSON 与序列化
来源：http://xae.ydzc1.top

================================================================================
来源：http://cif.shangyingyoupin.top

[K01] 对象转 JSON 字符串
来源：http://kri.cdnleiting.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ozd.chenjidiqi.icu

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://syw.jqgfzy.top

JS:   JSON.stringify(obj)
来源：http://hsm.yvedp.cn

TS:   JSON.stringify(obj)
来源：http://qag.iojbl.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rka.gotoacloud.top

Go:   json.Marshal(obj)
来源：http://cvs.havefunace.top

Ruby: obj.to_json                                     // require "json"
来源：http://qmu.yonumen.top

C#:   JsonSerializer.Serialize(obj)
来源：http://gpn.zhijiandao.cn

[K02] JSON 字符串转对象
来源：http://lza.yvedp.cn

Py:   json.loads(s)
来源：http://cpf.fengsongda.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://emt.chenlongwang.top

JS:   JSON.parse(s)
来源：http://pox.yanxiufei.cn

TS:   JSON.parse(s)
来源：http://qdl.sufxvd.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nsx.yangfankeji.com

Go:   json.Unmarshal(data, &v)
来源：http://rgz.tarul.cn

Ruby: JSON.parse(s)
来源：http://hms.xylfe.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://emv.havefunace.top

[K03] JSON 美化输出（带缩进）
来源：http://dcx.yueranfly.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bvp.smart0.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jnv.daria6918.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xwq.zdbjq.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rsk.xuanzx.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dki.316326.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://omn.shuidangran.top

Ruby: JSON.pretty_generate(obj)
来源：http://vbb.ehwqpu.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qnu.yj20258.top

[K04] 读取 JSON 文件
来源：http://pnf.sufxvd.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://msk.ybcxt.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hns.xingfuxueyuan.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lbs.shangyingyoupin.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://opt.guannengcc.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ixw.cucudq.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://use.tian-w.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mah.snrcjt.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fsf.shzxlz.cn

[K05] 深拷贝对象
来源：http://eaq.zycfv.cn

Py:   copy.deepcopy(obj)
来源：http://nbe.zhijiandao.cn

PHP:  unserialize(serialize($obj));
来源：http://vqs.zhoulong.xyz

JS:   structuredClone(obj)
来源：http://cbt.svipenyu.cn

TS:   structuredClone(obj)
来源：http://tjd.hesvh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jcz.jyoumei.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qui.sjlbkw.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nbd.hywenlv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://jki.zdbjq.cn

[K06] 解析 URL 查询串
来源：http://mmu.dianchejie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fyb.chenzaomai.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://taq.haohaochexian.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xbu.zhixingplan.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cax.snrcjt.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yvp.shanyushiyangkeji.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://nwl.tanke756.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qfm.epnwcf.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bht.cucudq.cn

[K07] 进制转换
来源：http://hsg.jinyuanbaomall.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yei.jinqigufen.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wne.tianlin.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://omy.yfazqb.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fgz.uphjek.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rtg.zdbjq.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fzc.ivvv.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uaq.chenlongwang.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mnh.smart0.xyz

[K08] 二进制序列化（非 JSON）
来源：http://cxl.pycfn.com

Py:   pickle.dumps(obj)
来源：http://lfz.bjfxy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://idt.ehwqpu.com

JS:   v8.serialize(obj)        // Node
来源：http://kbc.chenlongwang.top

TS:   v8.serialize(obj)        // Node
来源：http://zei.fanxiaobao.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zzz.uphjek.com

Go:   encoding/gob
来源：http://rlk.quarkkingdee.top

Ruby: Marshal.dump(obj)
来源：http://zso.sjlbkw.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cwe.zdbjq.cn

================================================================================
来源：http://kcn.bbcook.cn

L. 网络请求
来源：http://vlq.yanxiufei.cn

================================================================================
来源：http://xob.zhoulong.xyz

[L01] 发送 GET 请求
来源：http://jje.dashuyun.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gev.zhongyouzk.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://osh.aibaodan.cn

JS:   await fetch(url)
来源：http://agq.sweek.top

TS:   await fetch(url)
来源：http://vor.ivvv.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uwy.jqgfzy.top

Go:   resp, err := http.Get(url)
来源：http://hcz.jinqigfzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://kqb.sweek.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tgm.hcnkem.com

[L02] 发送 POST JSON
来源：http://ieh.xuanzx.com

Py:   requests.post(url, json={"a": 1})
来源：http://cnt.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uem.ydjk.org.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wwn.yj20258888.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nnd.havefunace.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vdd.shangyingyoupin.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tvg.jiagoushi.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cvw.sjlbkw.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cjm.ehwqpu.com

[L03] 设置自定义请求头
来源：http://tpr.52xcode.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fmo.9152youxi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sle.daxiang520.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://arg.c1oappe.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nuz.yueranfly.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://csi.wangdashe.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lcg.0kj1m.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hqg.yanxiufei.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://srz.fengsongda.top

[L04] 设置超时
来源：http://pnn.cashguo.top

Py:   requests.get(url, timeout=5)
来源：http://ftd.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jtr.ydzc1.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oce.jinqigufen.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jao.cqqwz.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zgh.yuanzhike.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xdq.vqdsnc.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lgw.meibo888.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://abw.epnwcf.com

[L05] 上传文件（multipart）
来源：http://mjc.shanyushiyangtech.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vnb.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://eci.wangdashe.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uee.gotoacloud.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://asj.ybcxt.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wxg.sysykeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kml.bjfxy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://iis.svipenyu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ece.zhiwuduotai.top

[L06] 解析响应为 JSON
来源：http://qpk.fzhhl.top

Py:   resp.json()
来源：http://cak.zdbjq.cn

PHP:  json_decode($body, true);
来源：http://nak.jinyuanbaomall.cn

JS:   await resp.json()
来源：http://lcr.zhixingplan.top

TS:   await resp.json()
来源：http://iyo.andypj.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rva.nanxuanxn.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yii.chenlongwang.top

Ruby: JSON.parse(resp.body)
来源：http://gkk.jinghuilouyu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lqb.xuetiantiany.cn

[L07] 处理 HTTP 状态码
来源：http://lys.ywan-chungtsiang.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fwl.svipenyu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ylr.tanke756.top

JS:   resp.ok;  resp.status
来源：http://mva.andypj.xyz

TS:   resp.ok;  resp.status
来源：http://lfw.shangyingyoupin.top

Java: resp.statusCode()
来源：http://bbd.epnwcf.com

Go:   resp.StatusCode
来源：http://tlz.316326.xyz

Ruby: resp.code.to_i
来源：http://mtf.ehwqpu.com

C#:   (int)resp.StatusCode
来源：http://ril.yfazqb.com

[L08] 并发请求多个地址
来源：http://dfe.zhaomingkeji.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cwa.hongshengwenyu.top

PHP:  curl_multi_init() 系列
来源：http://eew.iojbl.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://por.316326.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lst.shanyushiyangtech.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hjg.birdmap.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vba.jinqigfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kgs.chenzaomai.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ayb.vqdsnc.cn

================================================================================
来源：http://day.xylfe.cn

M. 命令行 / 进程 / 环境
来源：http://aim.ydzc1.top

================================================================================
来源：http://jre.zdqjudy.top

[M01] 读取命令行参数
来源：http://zaz.aizwys.cn

Py:   sys.argv[1:]
来源：http://jcr.sufxvd.cn

PHP:  $argv;  $argc;
来源：http://tqr.shanyushiyangtech.top

JS:   process.argv.slice(2)
来源：http://ecu.cheryme.top

TS:   process.argv.slice(2)
来源：http://kab.jqgufenzy.top

Java: args 数组（main 方法参数）
来源：http://imi.nanxinkj.top

Go:   os.Args[1:]
来源：http://lip.zhaomingkeji.xyz

Ruby: ARGV
来源：http://ojz.xuetiantiany.cn

C#:   args 数组（Main 方法参数）
来源：http://rmx.birdmap.top

[M02] 读取环境变量
来源：http://oja.ppjwa.cn

Py:   os.environ.get("HOME")
来源：http://fji.316326.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xxt.hesvh.cn

JS:   process.env.HOME
来源：http://epr.yuanzhike.top

TS:   process.env.HOME
来源：http://bxd.c1oappe.top

Java: System.getenv("HOME")
来源：http://ltn.jinghuilouyu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ifv.tanke756.top

Ruby: ENV["HOME"]
来源：http://euv.mhx1999.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vng.hnxiangtu.top

[M03] 执行外部命令
来源：http://xcj.ctjpmb.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bdr.yj202588.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://sga.ehwqpu.com

JS:   child_process.execSync("ls -l").toString()
来源：http://tln.ydzc1.top

TS:   child_process.execSync("ls -l").toString()
来源：http://iwg.ctjpmb.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://oll.0kj1m.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fvc.316326.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://fyh.zdqjudy.top

C#:   Process.Start("ls", "-l");
来源：http://mpp.redwolf501.top

[M04] 获取当前工作目录
来源：http://wgp.zhaomingkeji.xyz

Py:   os.getcwd()
来源：http://hqd.fanxiaobao.xyz

PHP:  getcwd();
来源：http://xrp.fengsongda.top

JS:   process.cwd()
来源：http://soe.jqgfzy.top

TS:   process.cwd()
来源：http://khz.yonumen.top

Java: Path.of("").toAbsolutePath()
来源：http://aso.sweek.top

Go:   os.Getwd()
来源：http://olv.yangfankeji.com

Ruby: Dir.pwd
来源：http://wun.pengpengdd.cyou

C#:   Directory.GetCurrentDirectory()
来源：http://vqe.ppjwa.cn

[M05] 设置退出码
来源：http://max.ppjwa.cn

Py:   sys.exit(1)
来源：http://kbe.ppjwa.cn

PHP:  exit(1);
来源：http://blk.c1oappe.top

JS:   process.exit(1)
来源：http://fkt.zhengqikj.top

TS:   process.exit(1)
来源：http://ppi.havefunace.top

Java: System.exit(1)
来源：http://qri.aizwys.cn

Go:   os.Exit(1)
来源：http://lrh.birdmap.top

Ruby: exit 1
来源：http://nwa.yueranfly.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fea.hfpthk.cn

[M06] 向标准错误输出
来源：http://gjq.daria6918.cn

Py:   print("err", file=sys.stderr)
来源：http://rmr.fktsv.cn


<!-- 参考信息 -->