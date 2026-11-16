代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kvw.tianlin.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://umh.mhx1999.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xld.ydjk.org.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fmz.pengpengdd.cyou

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vzx.aibaodan.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jvh.cqqwz.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dec.feifeiyinyue.top

================================================================================
来源：http://uhp.yanxiufei.cn

J. 日期与时间
来源：http://eiw.smart0.xyz

================================================================================
来源：http://hjp.yj20258.top

[J01] 获取当前时间
来源：http://rjy.tarul.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://eyf.zycfv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lar.haohaochexian.top

JS:   new Date();  Date.now()
来源：http://blm.nanxuanxn.top

TS:   new Date();  Date.now()
来源：http://ies.shuidangran.top

Java: LocalDateTime.now();  Instant.now()
来源：http://icm.guowangkeji.top

Go:   time.Now()
来源：http://bwk.quarkkingdee.top

Ruby: Time.now
来源：http://lrm.xinyue.icu

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fex.gzhubu.top

[J02] 格式化输出
来源：http://zxg.yonumen.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://enw.zhixingplan.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zde.shuidangran.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hif.shanyushiyangkeji.top

TS:   d.toISOString()
来源：http://pkh.chenzaomai.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lxb.iojbl.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://she.jianghu66.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bky.jinqigufen.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xtx.meibo888.top

[J03] 字符串解析为日期
来源：http://lsl.yfazqb.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vzu.redwolf501.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qxy.vqdsnc.cn

JS:   new Date("2024-01-02")
来源：http://mng.ctjpmb.com

TS:   new Date("2024-01-02")
来源：http://yxf.jinghuilouyu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cdq.jianghu66.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://whj.birdmap.top

Ruby: Date.parse("2024-01-02")
来源：http://rje.c1oappe.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vxm.mhx1999.top

[J04] 时间戳与日期互转
来源：http://bci.ydzc1.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dko.hcnkem.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cnm.yueranfly.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xcs.yongpay.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ngk.cdnleiting.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hpl.ctjpmb.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bni.hysaishi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sdt.yuanzhike.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cdv.andypj.xyz

[J05] 时间加减（加 7 天）
来源：http://knj.fengsongda.top

Py:   now + timedelta(days=7)
来源：http://ntn.9152youxi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nek.nanxinkj.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qpj.hysaishi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mre.hcnkem.com

Java: LocalDate.now().plusDays(7)
来源：http://zhn.bjfxy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pmi.bbcook.cn

Ruby: Time.now + 7 * 86400
来源：http://shm.nanxuanxn.top

C#:   DateTime.Now.AddDays(7)
来源：http://cir.9152youxi.cn

[J06] 计算两时间之差
来源：http://tdg.fehbvm.com

Py:   (end - start).total_seconds()
来源：http://njv.0kj1m.cn

PHP:  $end->diff($start)->days;
来源：http://pbh.zdqjudy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hmr.sysykeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xmb.xinyue.icu

Java: Duration.between(start, end).toSeconds()
来源：http://ath.jqgfzy.top

Go:   end.Sub(start).Hours()
来源：http://fgs.xylfe.cn

Ruby: end - start                 # 返回秒数
来源：http://vpp.xuanzx.com

C#:   (end - start).TotalSeconds
来源：http://bel.yonumen.top

[J07] 比较两个日期
来源：http://gla.vehdjk.com

Py:   d1 < d2;  d1 == d2
来源：http://jre.nwbrower.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://iwa.bbcook.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kwu.havefunace.top

TS:   d1.getTime() < d2.getTime()
来源：http://yqd.wangdashe.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gri.snrcjt.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hmr.jlsjyb.cn

Ruby: d1 < d2;  d1 == d2
来源：http://sye.zhongyouzk.top

C#:   d1 < d2;  d1 == d2
来源：http://jdl.pengpengdd.cyou

[J08] 提取年月日与星期
来源：http://goe.cdnleiting.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://miu.vqdsnc.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fcw.zhoulong.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rbp.zdqjudy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://eny.gaohongyu789.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ohq.316326.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vav.cdnleiting.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nzw.jlsjyb.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dbo.jinqigufen.top

[J09] 时区处理
来源：http://eoc.sysykeji.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yoa.aizwys.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://eqz.meibo888.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wyh.cdnleiting.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mnm.jqgufenzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cap.smart0.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kta.zdbjq.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://nzh.chenlongwang.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wsg.birdmap.top

[J10] 取今天 / 本月第一天
来源：http://hsq.jinghuilouyu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wjr.daria6918.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bwf.c1oappe.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hvs.xinyue.icu

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sua.feifeiyinyue.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fnv.chenlongwang.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://iaw.meibo888.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nwt.ctjpmb.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://szd.xuanzx.com

================================================================================
来源：http://qjg.kuanghao11.cn

K. JSON 与序列化
来源：http://dlr.nanxinkj.top

================================================================================
来源：http://xnj.yfazqb.com

[K01] 对象转 JSON 字符串
来源：http://mid.sufxvd.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gtd.jinyuanbaomall.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tom.pengpengdd.cyou

JS:   JSON.stringify(obj)
来源：http://rsf.fengsongda.top

TS:   JSON.stringify(obj)
来源：http://ezs.ivvv.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mmu.yuanzhike.top

Go:   json.Marshal(obj)
来源：http://mgu.aizwys.cn

Ruby: obj.to_json                                     // require "json"
来源：http://opf.xziqi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://uvq.wangshuangyany.cn

[K02] JSON 字符串转对象
来源：http://aye.zhengqikj.top

Py:   json.loads(s)
来源：http://dpx.yuanzhike.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jly.zdqjudy.top

JS:   JSON.parse(s)
来源：http://vjj.yongpay.top

TS:   JSON.parse(s)
来源：http://ndj.xingfuxueyuan.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rbo.bjfxy.top

Go:   json.Unmarshal(data, &v)
来源：http://ksv.chenzaomai.com

Ruby: JSON.parse(s)
来源：http://lul.jqgfzy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rlm.xziqi.cn

[K03] JSON 美化输出（带缩进）
来源：http://mdz.mhx1999.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://crl.shangyingyoupin.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ypb.cheryme.top

JS:   JSON.stringify(obj, null, 2)
来源：http://dui.vehdjk.com

TS:   JSON.stringify(obj, null, 2)
来源：http://enp.tianlin.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ifk.gaohongyu789.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ifj.ywan-chungtsiang.top

Ruby: JSON.pretty_generate(obj)
来源：http://dfh.yvedp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ogm.hnxiangtu.top

[K04] 读取 JSON 文件
来源：http://tmp.sysykeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://oye.zhixingplan.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wce.smart0.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rmw.xinyue.icu

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sns.daria6918.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cuc.hysaishi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zrp.gotoacloud.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://rys.nwbrower.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hgl.ydjk.org.cn

[K05] 深拷贝对象
来源：http://cpj.gaohongyu789.top

Py:   copy.deepcopy(obj)
来源：http://kly.shanyushiyangtech.top

PHP:  unserialize(serialize($obj));
来源：http://qwl.wangshuangyany.cn

JS:   structuredClone(obj)
来源：http://fsh.yanxiufei.cn

TS:   structuredClone(obj)
来源：http://fko.52xcode.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gig.havefunace.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kim.yj20258888.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://occ.zhengqikj.top

C#:   // 序列化往返，或自定义 Clone
来源：http://kzs.jinyuanbaomall.cn

[K06] 解析 URL 查询串
来源：http://qrp.xziqi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nbj.dianchejie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xzf.zhoulong.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ltt.xingfuxueyuan.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nid.yangfankeji.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fnk.xuanzx.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://tnh.dianchejie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kxb.sxryk.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mpz.tianlin.xyz

[K07] 进制转换
来源：http://ljl.gzhubu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fey.yuxming.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ejd.andypj.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://djo.guowangkeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zuz.xuanzx.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://msi.birdmap.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://exd.ydzc1.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://naj.andypj.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vdy.xylfe.cn

[K08] 二进制序列化（非 JSON）
来源：http://ijj.gogol.net.cn

Py:   pickle.dumps(obj)
来源：http://pzv.pengpengdd.cyou

PHP:  serialize($obj);  unserialize($s);
来源：http://ugb.gogol.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://ild.svipenyu.cn

TS:   v8.serialize(obj)        // Node
来源：http://pvr.cucudq.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xrz.andypj.xyz

Go:   encoding/gob
来源：http://cwc.mhx1999.top

Ruby: Marshal.dump(obj)
来源：http://zng.nwbrower.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cvk.yanxiufei.cn

================================================================================
来源：http://ewt.xinyue.icu

L. 网络请求
来源：http://atw.yangfankeji.com

================================================================================
来源：http://ell.fengsongda.top

[L01] 发送 GET 请求
来源：http://qmx.fehbvm.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://occ.kuanghao11.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rqe.uphjek.com

JS:   await fetch(url)
来源：http://hva.zhijiandao.cn

TS:   await fetch(url)
来源：http://fiv.gotoacloud.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tgp.gzhubu.top

Go:   resp, err := http.Get(url)
来源：http://gay.snrcjt.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://cvh.cheryme.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jxk.epnwcf.com

[L02] 发送 POST JSON
来源：http://bsz.chenjidiqi.icu

Py:   requests.post(url, json={"a": 1})
来源：http://gzh.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pat.xinyue.icu

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ufc.yj20258.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://poy.9152youxi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yxm.nanxuanxn.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dqu.birdmap.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://whc.cqqwz.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://snw.epnwcf.com

[L03] 设置自定义请求头
来源：http://ctc.yueranfly.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gts.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sys.gzhubu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://thh.sjlbkw.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mzz.cucudq.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cnl.cashguo.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rca.tanke756.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bno.sjlbkw.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://skx.jianghu66.top

[L04] 设置超时
来源：http://zlw.yvedp.cn

Py:   requests.get(url, timeout=5)
来源：http://ygq.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kuj.ybcxt.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lrp.cheryme.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://her.smart0.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wun.hysaishi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mjx.gaohongyu789.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cly.316326.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ddo.shanyushiyangkeji.top

[L05] 上传文件（multipart）
来源：http://uvy.uphjek.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xzv.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cjs.birdmap.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uyk.cqqwz.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ubu.hywenlv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wkm.xinyue.icu

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zzz.svipenyu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kuv.redwolf501.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fqt.cdnleiting.top

[L06] 解析响应为 JSON
来源：http://jdn.yuanzhike.top

Py:   resp.json()
来源：http://hgs.ybcxt.top

PHP:  json_decode($body, true);
来源：http://uhy.jinqigfzy.top

JS:   await resp.json()
来源：http://dhe.ctjpmb.com

TS:   await resp.json()
来源：http://sqy.dashuyun.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fwj.mhx1999.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://urz.pycfn.com

Ruby: JSON.parse(resp.body)
来源：http://iup.ctjpmb.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jzx.ehwqpu.com

[L07] 处理 HTTP 状态码
来源：http://nkb.daria6918.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jmn.fengsongda.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://oow.andypj.xyz

JS:   resp.ok;  resp.status
来源：http://wen.hysaishi.cn

TS:   resp.ok;  resp.status
来源：http://ubq.ppjwa.cn

Java: resp.statusCode()
来源：http://qmb.fanxiaobao.xyz

Go:   resp.StatusCode
来源：http://fkw.hesvh.cn

Ruby: resp.code.to_i
来源：http://lzf.zycfv.cn

C#:   (int)resp.StatusCode
来源：http://ifk.fehbvm.com

[L08] 并发请求多个地址
来源：http://eht.c1oappe.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qmh.yj20258888.top

PHP:  curl_multi_init() 系列
来源：http://uck.vqdsnc.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ksm.quarkkingdee.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bzr.zhengqikj.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zun.tarul.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ovj.ydjk.org.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nve.hnxiangtu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yyv.nanxuanxn.top

================================================================================
来源：http://pdg.quarkkingdee.top

M. 命令行 / 进程 / 环境
来源：http://frc.zhijiandao.cn

================================================================================
来源：http://sti.ywan-chungtsiang.top

[M01] 读取命令行参数
来源：http://tej.ehwqpu.com

Py:   sys.argv[1:]
来源：http://efo.redwolf501.top

PHP:  $argv;  $argc;
来源：http://kem.nanxinkj.top

JS:   process.argv.slice(2)
来源：http://mbt.hammf.cn

TS:   process.argv.slice(2)
来源：http://kut.hcnkem.com

Java: args 数组（main 方法参数）
来源：http://man.svipenyu.cn

Go:   os.Args[1:]
来源：http://wnz.iojbl.cn

Ruby: ARGV
来源：http://ucr.hesvh.cn

C#:   args 数组（Main 方法参数）
来源：http://mbt.kuanghao11.cn

[M02] 读取环境变量
来源：http://mfu.yueranfly.top

Py:   os.environ.get("HOME")
来源：http://ofj.gzhubu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://prr.fengsongda.top

JS:   process.env.HOME
来源：http://hce.zycfv.cn

TS:   process.env.HOME
来源：http://nfv.daria6918.cn

Java: System.getenv("HOME")
来源：http://uyt.ehwqpu.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oua.cheryme.top

Ruby: ENV["HOME"]
来源：http://yuc.cheryme.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nmq.ydjk.org.cn

[M03] 执行外部命令
来源：http://fxo.jiagoushi.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dpl.aizwys.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hvp.fanxiaobao.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://swx.fanxiaobao.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://qmv.snrcjt.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wci.jyoumei.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ofq.sufxvd.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wfk.gotoacloud.top

C#:   Process.Start("ls", "-l");
来源：http://oqp.vqdsnc.cn

[M04] 获取当前工作目录
来源：http://xhf.jinyuanbaomall.cn

Py:   os.getcwd()
来源：http://yvw.ppjwa.cn

PHP:  getcwd();
来源：http://jju.bjfxy.top

JS:   process.cwd()
来源：http://swr.mhx1999.top

TS:   process.cwd()
来源：http://qgn.shanyushiyangkeji.top

Java: Path.of("").toAbsolutePath()
来源：http://tul.zhoulong.xyz

Go:   os.Getwd()
来源：http://dde.jinghuilouyu.cn

Ruby: Dir.pwd
来源：http://lfo.hnqzz.top

C#:   Directory.GetCurrentDirectory()
来源：http://gls.vqdsnc.cn

[M05] 设置退出码
来源：http://gti.chenlongwang.top

Py:   sys.exit(1)
来源：http://kev.tian-w.cn

PHP:  exit(1);
来源：http://ajr.daxiang520.top

JS:   process.exit(1)
来源：http://wbi.jqgfzy.top

TS:   process.exit(1)
来源：http://xfs.sufxvd.cn

Java: System.exit(1)
来源：http://xnz.bbcook.cn

Go:   os.Exit(1)
来源：http://fsq.tanke756.top

Ruby: exit 1
来源：http://kcd.wangdashe.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://auw.hysaishi.cn

[M06] 向标准错误输出
来源：http://cva.fzhhl.top

Py:   print("err", file=sys.stderr)
来源：http://jau.sxryk.cn


<!-- 参考信息 -->