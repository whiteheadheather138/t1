代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://omy.chenzaomai.com

TS:   /error/gim
来源：http://hqx.cheryme.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mlx.zhongyouzk.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://akb.tanke756.top

Ruby: s.scan(/error/i)
来源：http://bpe.guowangkeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://adz.yj20258888.top

[I08] 贪婪与非贪婪匹配
来源：http://yoj.jinghuilouyu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vna.sweek.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qux.jinyuanbaomall.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zhv.hnxiangtu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nwr.fehbvm.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://ynv.yanxiufei.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://chr.zhengqikj.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wqg.ybcxt.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://elr.xingfuxueyuan.xyz

================================================================================
来源：http://gsm.shzxlz.cn

J. 日期与时间
来源：http://akx.fktsv.cn

================================================================================
来源：http://ndy.yvedp.cn

[J01] 获取当前时间
来源：http://ttq.cdnleiting.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://nyb.xuetiantiany.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mln.aibaodan.cn

JS:   new Date();  Date.now()
来源：http://rxv.yvedp.cn

TS:   new Date();  Date.now()
来源：http://jlb.xinyue.icu

Java: LocalDateTime.now();  Instant.now()
来源：http://zxq.shangyingyoupin.top

Go:   time.Now()
来源：http://vrs.xuanzx.com

Ruby: Time.now
来源：http://xsi.nanxuanxn.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://goq.cheryme.top

[J02] 格式化输出
来源：http://cjf.jinqigfzy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zpu.yangfankeji.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tli.zhijiandao.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pzy.sxryk.cn

TS:   d.toISOString()
来源：http://qjk.sweek.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://znm.gogol.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kne.xuetiantiany.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uwe.jinqigufen.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ezd.ybcxt.top

[J03] 字符串解析为日期
来源：http://wtj.fzhhl.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kgc.meibo888.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bqq.jlsjyb.cn

JS:   new Date("2024-01-02")
来源：http://sav.bjfxy.top

TS:   new Date("2024-01-02")
来源：http://ytf.hammf.cn

Java: LocalDate.parse("2024-01-02")
来源：http://nps.jinqigfzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yho.pengpengdd.cyou

Ruby: Date.parse("2024-01-02")
来源：http://ywq.jlsjyb.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qit.ydzc1.top

[J04] 时间戳与日期互转
来源：http://mqf.haohaochexian.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rss.ehwqpu.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hsl.zhengqikj.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wes.fengsongda.top

TS:   Math.floor(Date.now() / 1000)
来源：http://uxe.52xcode.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pus.ybcxt.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fbw.zdqjudy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nfz.cashguo.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bdd.316326.xyz

[J05] 时间加减（加 7 天）
来源：http://apm.sufxvd.cn

Py:   now + timedelta(days=7)
来源：http://aur.zhijiandao.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vhx.yvedp.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://psp.yj202588.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hzh.316326.xyz

Java: LocalDate.now().plusDays(7)
来源：http://noy.chenzaomai.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nur.jqgufenzy.top

Ruby: Time.now + 7 * 86400
来源：http://ugy.yonumen.top

C#:   DateTime.Now.AddDays(7)
来源：http://abl.dashuyun.cn

[J06] 计算两时间之差
来源：http://wlk.c1oappe.top

Py:   (end - start).total_seconds()
来源：http://lhw.shzxlz.cn

PHP:  $end->diff($start)->days;
来源：http://hko.guowangkeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vbt.redwolf501.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://llf.cashguo.top

Java: Duration.between(start, end).toSeconds()
来源：http://mnd.vehdjk.com

Go:   end.Sub(start).Hours()
来源：http://jqj.zhoulong.xyz

Ruby: end - start                 # 返回秒数
来源：http://iho.svipenyu.cn

C#:   (end - start).TotalSeconds
来源：http://wtw.c1oappe.top

[J07] 比较两个日期
来源：http://ntv.yonumen.top

Py:   d1 < d2;  d1 == d2
来源：http://evu.zhixingplan.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ptl.chenlongwang.top

JS:   d1.getTime() < d2.getTime()
来源：http://nfp.tarul.cn

TS:   d1.getTime() < d2.getTime()
来源：http://opm.pengpengdd.cyou

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://taa.smart0.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sds.bbcook.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jbb.gogol.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://xau.ywan-chungtsiang.top

[J08] 提取年月日与星期
来源：http://cyi.jiagoushi.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://umh.vqdsnc.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qqk.zhaomingkeji.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jhv.yuxming.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lav.c1oappe.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://agf.chenjidiqi.icu

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jtr.yfazqb.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zoo.chenjidiqi.icu

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zfk.gaohongyu789.top

[J09] 时区处理
来源：http://jne.xuanzx.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kgb.vehdjk.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fdj.dashuyun.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fxe.hywenlv.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sum.yueranfly.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wgw.cqqwz.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ojp.fktsv.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://swk.guannengcc.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dtx.yueranfly.top

[J10] 取今天 / 本月第一天
来源：http://bmj.jianghu66.top

Py:   date.today();  date.today().replace(day=1)
来源：http://bqz.vehdjk.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://oyk.snrcjt.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vzd.ivvv.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mvm.yongpay.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wre.xuanzx.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xcr.chenzaomai.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://txi.316326.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xcd.vqdsnc.cn

================================================================================
来源：http://mda.nwbrower.top

K. JSON 与序列化
来源：http://iri.zhiwuduotai.top

================================================================================
来源：http://kjx.daria6918.cn

[K01] 对象转 JSON 字符串
来源：http://xnc.yuanzhike.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://txk.shuidangran.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://itf.tianlin.xyz

JS:   JSON.stringify(obj)
来源：http://ffz.ctjpmb.com

TS:   JSON.stringify(obj)
来源：http://kog.shzxlz.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qdc.jyoumei.cn

Go:   json.Marshal(obj)
来源：http://oes.yangfankeji.com

Ruby: obj.to_json                                     // require "json"
来源：http://sah.yj20258888.top

C#:   JsonSerializer.Serialize(obj)
来源：http://thg.shanyushiyangkeji.top

[K02] JSON 字符串转对象
来源：http://aie.nwbrower.top

Py:   json.loads(s)
来源：http://kvn.52xcode.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qdj.guannengcc.top

JS:   JSON.parse(s)
来源：http://sds.shzxlz.cn

TS:   JSON.parse(s)
来源：http://nsp.52xcode.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kmo.tian-w.cn

Go:   json.Unmarshal(data, &v)
来源：http://sbz.chenjidiqi.icu

Ruby: JSON.parse(s)
来源：http://dpi.mhx1999.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xcb.meibo888.top

[K03] JSON 美化输出（带缩进）
来源：http://njo.xinyue.icu

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tde.fktsv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pdb.mhx1999.top

JS:   JSON.stringify(obj, null, 2)
来源：http://gox.vqdsnc.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://jhd.hysaishi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yau.haohaochexian.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://aoc.zdbjq.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xri.jinqigufen.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qdk.dashuyun.cn

[K04] 读取 JSON 文件
来源：http://chr.sweek.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uir.sjlbkw.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nxa.zhongyouzk.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://unl.pycfn.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tak.cucudq.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dlo.yfazqb.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zzv.daria6918.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wxh.zdqjudy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ekc.kuanghao11.cn

[K05] 深拷贝对象
来源：http://nun.ctjpmb.com

Py:   copy.deepcopy(obj)
来源：http://jez.jqgufenzy.top

PHP:  unserialize(serialize($obj));
来源：http://skh.hnqzz.top

JS:   structuredClone(obj)
来源：http://pft.sufxvd.cn

TS:   structuredClone(obj)
来源：http://zzp.316326.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://sez.fengsongda.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://oqy.fzhhl.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qyy.zdqjudy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://uzs.yangfankeji.com

[K06] 解析 URL 查询串
来源：http://lmt.jinghuilouyu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jgn.cdnleiting.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rsa.bbcook.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ytc.kuanghao11.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ofx.jinqigfzy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://epk.fanxiaobao.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://pxy.cdnleiting.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dod.cqqwz.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jao.cashguo.top

[K07] 进制转换
来源：http://ovq.ydzc1.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://szw.jianghu66.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sbw.ppjwa.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ldh.ydzc1.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ksc.jiagoushi.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://erb.zhaomingkeji.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dir.hammf.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jsf.c1oappe.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xuc.yj202588.top

[K08] 二进制序列化（非 JSON）
来源：http://iov.feifeiyinyue.top

Py:   pickle.dumps(obj)
来源：http://atj.xingfuxueyuan.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://pyx.cdnleiting.top

JS:   v8.serialize(obj)        // Node
来源：http://pgq.jianghu66.top

TS:   v8.serialize(obj)        // Node
来源：http://bvw.sjlbkw.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hmf.ybcxt.top

Go:   encoding/gob
来源：http://gzf.cashguo.top

Ruby: Marshal.dump(obj)
来源：http://ann.daxiang520.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://iec.snrcjt.cn

================================================================================
来源：http://goh.havefunace.top

L. 网络请求
来源：http://iva.yanxiufei.cn

================================================================================
来源：http://rjx.zhaomingkeji.xyz

[L01] 发送 GET 请求
来源：http://dfi.zdbjq.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nlz.ehwqpu.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yct.guowangkeji.top

JS:   await fetch(url)
来源：http://sni.yangfankeji.com

TS:   await fetch(url)
来源：http://awy.zhiwuduotai.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vye.0kj1m.cn

Go:   resp, err := http.Get(url)
来源：http://wim.hongshengwenyu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ezj.cashguo.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ceu.yanxiufei.cn

[L02] 发送 POST JSON
来源：http://bod.gotoacloud.top

Py:   requests.post(url, json={"a": 1})
来源：http://fwo.hesvh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nrc.yj20258.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://anu.xinyue.icu

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://frt.hongshengwenyu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://txh.ctjpmb.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ukh.sufxvd.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nfn.nanxuanxn.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ssh.ehwqpu.com

[L03] 设置自定义请求头
来源：http://dqm.jinqigfzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pbg.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wlb.ydjk.org.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jty.shzxlz.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qts.fktsv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bod.jyoumei.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ruf.yongpay.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nnt.cashguo.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lrj.jianghu66.top

[L04] 设置超时
来源：http://tde.hywenlv.cn

Py:   requests.get(url, timeout=5)
来源：http://qci.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jvr.yueranfly.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mit.nanxinkj.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pan.jinqigufen.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xwu.bbcook.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ylj.zhongyouzk.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hda.fzhhl.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qdm.chenjidiqi.icu

[L05] 上传文件（multipart）
来源：http://kiu.dashuyun.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wqq.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yqe.sxryk.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zfk.9152youxi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jma.zhixingplan.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sqs.hongshengwenyu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fci.guowangkeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ubu.gzhubu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jvu.zhongyouzk.top

[L06] 解析响应为 JSON
来源：http://uzr.birdmap.top

Py:   resp.json()
来源：http://enq.9152youxi.cn

PHP:  json_decode($body, true);
来源：http://phi.fengsongda.top

JS:   await resp.json()
来源：http://umm.hywenlv.cn

TS:   await resp.json()
来源：http://mgd.sysykeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://iuk.nwbrower.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pyg.yj202588.top

Ruby: JSON.parse(resp.body)
来源：http://xwh.dashuyun.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cho.ydzc1.top

[L07] 处理 HTTP 状态码
来源：http://xli.yvedp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yft.cheryme.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://goq.zhiwuduotai.top

JS:   resp.ok;  resp.status
来源：http://mhl.fehbvm.com

TS:   resp.ok;  resp.status
来源：http://tue.shzxlz.cn

Java: resp.statusCode()
来源：http://eed.9152youxi.cn

Go:   resp.StatusCode
来源：http://ldv.0kj1m.cn

Ruby: resp.code.to_i
来源：http://myy.ydjk.org.cn

C#:   (int)resp.StatusCode
来源：http://ufr.sysykeji.top

[L08] 并发请求多个地址
来源：http://nql.feifeiyinyue.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hbq.hysaishi.cn

PHP:  curl_multi_init() 系列
来源：http://ynz.jqgufenzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jpp.jiagoushi.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vgx.hywenlv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kce.jinqigfzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ltw.nanxuanxn.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mux.daxiang520.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qdx.bbcook.cn

================================================================================
来源：http://htx.cheryme.top

M. 命令行 / 进程 / 环境
来源：http://tlk.ydjk.org.cn

================================================================================
来源：http://wmp.svipenyu.cn

[M01] 读取命令行参数
来源：http://guk.wangdashe.top

Py:   sys.argv[1:]
来源：http://hsu.tarul.cn

PHP:  $argv;  $argc;
来源：http://owf.havefunace.top

JS:   process.argv.slice(2)
来源：http://vjm.nanxuanxn.top

TS:   process.argv.slice(2)
来源：http://ang.sufxvd.cn

Java: args 数组（main 方法参数）
来源：http://lwo.kuanghao11.cn

Go:   os.Args[1:]
来源：http://pdd.jqgfzy.top

Ruby: ARGV
来源：http://qtx.cheryme.top

C#:   args 数组（Main 方法参数）
来源：http://qdu.tian-w.cn

[M02] 读取环境变量
来源：http://ljv.redwolf501.top

Py:   os.environ.get("HOME")
来源：http://dew.xinyue.icu

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uaa.hesvh.cn

JS:   process.env.HOME
来源：http://oyi.nwbrower.top

TS:   process.env.HOME
来源：http://hbe.xingfuxueyuan.xyz

Java: System.getenv("HOME")
来源：http://cof.52xcode.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oqt.ehwqpu.com

Ruby: ENV["HOME"]
来源：http://gmd.havefunace.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://iqw.9152youxi.cn

[M03] 执行外部命令
来源：http://beq.zhoulong.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dzm.pengpengdd.cyou

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jbh.gzhubu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://bft.shzxlz.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://oax.gogol.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xqy.jinghuilouyu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://arh.tianlin.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://tew.xuanzx.com

C#:   Process.Start("ls", "-l");
来源：http://vrd.shanyushiyangtech.top

[M04] 获取当前工作目录
来源：http://jfj.fehbvm.com

Py:   os.getcwd()
来源：http://qiz.guannengcc.top

PHP:  getcwd();
来源：http://bzk.daxiang520.top

JS:   process.cwd()
来源：http://rzk.xuanzx.com

TS:   process.cwd()
来源：http://pei.0kj1m.cn

Java: Path.of("").toAbsolutePath()
来源：http://pdm.ivvv.top

Go:   os.Getwd()
来源：http://yzv.zhaomingkeji.xyz

Ruby: Dir.pwd
来源：http://ugb.ivvv.top

C#:   Directory.GetCurrentDirectory()
来源：http://bzq.pycfn.com

[M05] 设置退出码
来源：http://yke.shangyingyoupin.top

Py:   sys.exit(1)
来源：http://cym.tanke756.top

PHP:  exit(1);
来源：http://vmp.yuanzhike.top


<!-- 参考信息 -->