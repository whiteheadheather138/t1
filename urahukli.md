代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zof.havefunace.top

TS:   /error/gim
来源：http://mbv.gzhubu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ryi.ybcxt.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zft.epnwcf.com

Ruby: s.scan(/error/i)
来源：http://sou.hongshengwenyu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nzz.yj202588.top

[I08] 贪婪与非贪婪匹配
来源：http://ttf.316326.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ntu.yj202588.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zee.jinqigfzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nie.sxryk.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://eyh.ctjpmb.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://mch.havefunace.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zhk.ydzc1.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tvk.hcnkem.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://whs.jinyuanbaomall.cn

================================================================================
来源：http://bky.kuanghao11.cn

J. 日期与时间
来源：http://jhe.redwolf501.top

================================================================================
来源：http://kvl.meibo888.top

[J01] 获取当前时间
来源：http://glm.zdqjudy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://vvi.sysykeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dks.52xcode.cn

JS:   new Date();  Date.now()
来源：http://gpt.gaohongyu789.top

TS:   new Date();  Date.now()
来源：http://ypc.bjfxy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://tgw.mhx1999.top

Go:   time.Now()
来源：http://zcr.ywan-chungtsiang.top

Ruby: Time.now
来源：http://ydd.yvedp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ocd.wangshuangyany.cn

[J02] 格式化输出
来源：http://azd.zhijiandao.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bor.gotoacloud.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cwt.pengpengdd.cyou

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tqf.xuanzx.com

TS:   d.toISOString()
来源：http://uwb.vehdjk.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fvm.gogol.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ksc.nwbrower.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rpd.zycfv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blh.yuanzhike.top

[J03] 字符串解析为日期
来源：http://chz.xylfe.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qnm.tianlin.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://apj.iojbl.cn

JS:   new Date("2024-01-02")
来源：http://ura.zhijiandao.cn

TS:   new Date("2024-01-02")
来源：http://zzr.nanxuanxn.top

Java: LocalDate.parse("2024-01-02")
来源：http://ntl.guowangkeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wuj.tianlin.xyz

Ruby: Date.parse("2024-01-02")
来源：http://lxn.gotoacloud.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://aqs.tanke756.top

[J04] 时间戳与日期互转
来源：http://vpg.shangyingyoupin.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sbq.pengpengdd.cyou

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bjf.quarkkingdee.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://crp.xylfe.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vlf.smart0.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://chx.havefunace.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jka.cdnleiting.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kqo.fengsongda.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vgt.hywenlv.cn

[J05] 时间加减（加 7 天）
来源：http://yfw.shanyushiyangtech.top

Py:   now + timedelta(days=7)
来源：http://zci.birdmap.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://euf.ydzc1.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ddm.feifeiyinyue.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bdd.quarkkingdee.top

Java: LocalDate.now().plusDays(7)
来源：http://sid.birdmap.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rmx.tianlin.xyz

Ruby: Time.now + 7 * 86400
来源：http://nkt.xylfe.cn

C#:   DateTime.Now.AddDays(7)
来源：http://stb.tianlin.xyz

[J06] 计算两时间之差
来源：http://wzw.quarkkingdee.top

Py:   (end - start).total_seconds()
来源：http://dar.chenzaomai.com

PHP:  $end->diff($start)->days;
来源：http://non.zycfv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nrq.iojbl.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ppg.mhx1999.top

Java: Duration.between(start, end).toSeconds()
来源：http://nlf.zhoulong.xyz

Go:   end.Sub(start).Hours()
来源：http://ngi.daria6918.cn

Ruby: end - start                 # 返回秒数
来源：http://zfg.xziqi.cn

C#:   (end - start).TotalSeconds
来源：http://mpn.ctjpmb.com

[J07] 比较两个日期
来源：http://xiv.cheryme.top

Py:   d1 < d2;  d1 == d2
来源：http://dfc.shzxlz.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nfa.cucudq.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rgy.aibaodan.cn

TS:   d1.getTime() < d2.getTime()
来源：http://txv.yj202588.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gsk.bjfxy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bna.jqgfzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://txq.hammf.cn

C#:   d1 < d2;  d1 == d2
来源：http://myi.svipenyu.cn

[J08] 提取年月日与星期
来源：http://hoo.gzhubu.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uvz.wangdashe.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://eov.zhixingplan.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rxh.hysaishi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://emu.cqqwz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hca.nanxinkj.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lfs.yuanzhike.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ssy.pengpengdd.cyou

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dyj.ydzc1.top

[J09] 时区处理
来源：http://zss.hongshengwenyu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sok.sysykeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mzm.quarkkingdee.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wvi.jinqigufen.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fev.nwbrower.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://aqj.sysykeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hpt.snrcjt.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zgf.haohaochexian.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tuv.vehdjk.com

[J10] 取今天 / 本月第一天
来源：http://hcr.smart0.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://msm.iojbl.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zoc.svipenyu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vai.iojbl.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bbv.cucudq.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://woq.xuetiantiany.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fri.jiagoushi.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ddq.shzxlz.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zsh.pengpengdd.cyou

================================================================================
来源：http://vfh.yfazqb.com

K. JSON 与序列化
来源：http://kdq.fzhhl.top

================================================================================
来源：http://twv.dianchejie.cn

[K01] 对象转 JSON 字符串
来源：http://flt.yonumen.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://plv.ydzc1.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://sbj.haohaochexian.top

JS:   JSON.stringify(obj)
来源：http://zdh.hysaishi.cn

TS:   JSON.stringify(obj)
来源：http://hix.redwolf501.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rhs.tianlin.xyz

Go:   json.Marshal(obj)
来源：http://nlq.mhx1999.top

Ruby: obj.to_json                                     // require "json"
来源：http://zmz.tanke756.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ggm.pengpengdd.cyou

[K02] JSON 字符串转对象
来源：http://kzw.birdmap.top

Py:   json.loads(s)
来源：http://pqd.hnqzz.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://chr.mhx1999.top

JS:   JSON.parse(s)
来源：http://biu.meibo888.top

TS:   JSON.parse(s)
来源：http://ing.yanxiufei.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ktd.mhx1999.top

Go:   json.Unmarshal(data, &v)
来源：http://iia.cheryme.top

Ruby: JSON.parse(s)
来源：http://wzs.tanke756.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fqy.ppjwa.cn

[K03] JSON 美化输出（带缩进）
来源：http://pxy.nwbrower.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qhp.dashuyun.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://izw.chenzaomai.com

JS:   JSON.stringify(obj, null, 2)
来源：http://foa.hongshengwenyu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://jrh.tanke756.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://quy.dashuyun.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://juq.yvedp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ulq.yfazqb.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kuq.aizwys.cn

[K04] 读取 JSON 文件
来源：http://rov.yuanzhike.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hbn.ivvv.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hic.epnwcf.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jrh.ybcxt.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wbs.hysaishi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vtp.xuanzx.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pzg.pengpengdd.cyou

Ruby: JSON.parse(File.read("a.json"))
来源：http://tnc.gzhubu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://usi.yj20258888.top

[K05] 深拷贝对象
来源：http://bze.xylfe.cn

Py:   copy.deepcopy(obj)
来源：http://fxe.fengsongda.top

PHP:  unserialize(serialize($obj));
来源：http://qem.quarkkingdee.top

JS:   structuredClone(obj)
来源：http://dkw.chenjidiqi.icu

TS:   structuredClone(obj)
来源：http://mkt.yueranfly.top

Java: // 手写拷贝构造，或序列化往返
来源：http://iin.zhixingplan.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gxy.mhx1999.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wfb.daria6918.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rre.bbcook.cn

[K06] 解析 URL 查询串
来源：http://giz.gzhubu.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zwv.shanyushiyangtech.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mwt.tianlin.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://geq.cdnleiting.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vvx.zhengqikj.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nxd.hnqzz.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://aux.meibo888.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lyz.jianghu66.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://udp.yj202588.top

[K07] 进制转换
来源：http://zxw.zhijiandao.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://huq.cashguo.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://whi.nwbrower.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jts.yuxming.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://plk.jinghuilouyu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lvk.yangfankeji.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cxp.zhaomingkeji.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qkl.sweek.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ajk.zhoulong.xyz

[K08] 二进制序列化（非 JSON）
来源：http://fyc.hnqzz.top

Py:   pickle.dumps(obj)
来源：http://boi.yueranfly.top

PHP:  serialize($obj);  unserialize($s);
来源：http://hcs.gzhubu.top

JS:   v8.serialize(obj)        // Node
来源：http://xwi.yuanzhike.top

TS:   v8.serialize(obj)        // Node
来源：http://uix.cucudq.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hjq.hcnkem.com

Go:   encoding/gob
来源：http://dpp.sweek.top

Ruby: Marshal.dump(obj)
来源：http://swo.fzhhl.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tsr.mhx1999.top

================================================================================
来源：http://fgh.tanke756.top

L. 网络请求
来源：http://kec.tarul.cn

================================================================================
来源：http://zeq.jqgfzy.top

[L01] 发送 GET 请求
来源：http://hjm.quarkkingdee.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fch.ctjpmb.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yop.yj20258.top

JS:   await fetch(url)
来源：http://ukv.zhongyouzk.top

TS:   await fetch(url)
来源：http://woi.hesvh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rsj.cucudq.cn

Go:   resp, err := http.Get(url)
来源：http://vcb.c1oappe.top

Ruby: Net::HTTP.get(URI(url))
来源：http://fzo.bbcook.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fim.hnxiangtu.top

[L02] 发送 POST JSON
来源：http://psv.jlsjyb.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ury.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zjn.yuxming.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wct.zhiwuduotai.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cbn.fanxiaobao.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bph.yuanzhike.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kiv.jqgfzy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xsb.ppjwa.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vwl.fktsv.cn

[L03] 设置自定义请求头
来源：http://ckl.vqdsnc.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://evi.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mce.wangshuangyany.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qup.mhx1999.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://noy.zycfv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gkx.havefunace.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cup.jianghu66.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jtf.meibo888.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ymw.shanyushiyangkeji.top

[L04] 设置超时
来源：http://ncb.shanyushiyangtech.top

Py:   requests.get(url, timeout=5)
来源：http://qvq.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fxk.yongpay.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://krj.jinghuilouyu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tlv.tarul.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fee.chenjidiqi.icu

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://arx.ivvv.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nly.sxryk.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hgc.cqqwz.cn

[L05] 上传文件（multipart）
来源：http://mjv.xuanzx.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://luk.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xxi.ppjwa.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ner.ivvv.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hyz.xinyue.icu

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blg.zdqjudy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gmb.ivvv.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wcl.jinqigufen.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kdk.sufxvd.cn

[L06] 解析响应为 JSON
来源：http://vds.zhoulong.xyz

Py:   resp.json()
来源：http://ssr.zhijiandao.cn

PHP:  json_decode($body, true);
来源：http://cph.hnqzz.top

JS:   await resp.json()
来源：http://pln.chenjidiqi.icu

TS:   await resp.json()
来源：http://vyc.epnwcf.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qkf.gotoacloud.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gyx.yuanzhike.top

Ruby: JSON.parse(resp.body)
来源：http://cmz.daria6918.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ivv.c1oappe.top

[L07] 处理 HTTP 状态码
来源：http://xpi.sweek.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jap.fzhhl.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yuk.316326.xyz

JS:   resp.ok;  resp.status
来源：http://nex.yuanzhike.top

TS:   resp.ok;  resp.status
来源：http://xaq.jqgfzy.top

Java: resp.statusCode()
来源：http://zir.ehwqpu.com

Go:   resp.StatusCode
来源：http://zac.c1oappe.top

Ruby: resp.code.to_i
来源：http://abz.c1oappe.top

C#:   (int)resp.StatusCode
来源：http://woj.xziqi.cn

[L08] 并发请求多个地址
来源：http://zke.tarul.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wvz.jqgufenzy.top

PHP:  curl_multi_init() 系列
来源：http://weg.cucudq.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yta.316326.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kvd.zdqjudy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wri.fengsongda.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wzs.hongshengwenyu.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nrp.pycfn.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qpp.tianlin.xyz

================================================================================
来源：http://kos.guannengcc.top

M. 命令行 / 进程 / 环境
来源：http://ixs.gaohongyu789.top

================================================================================
来源：http://sct.zhongyouzk.top

[M01] 读取命令行参数
来源：http://eyh.shuidangran.top

Py:   sys.argv[1:]
来源：http://lud.shzxlz.cn

PHP:  $argv;  $argc;
来源：http://qgl.hcnkem.com

JS:   process.argv.slice(2)
来源：http://ren.quarkkingdee.top

TS:   process.argv.slice(2)
来源：http://dmo.bbcook.cn

Java: args 数组（main 方法参数）
来源：http://axi.9152youxi.cn

Go:   os.Args[1:]
来源：http://nlc.hfpthk.cn

Ruby: ARGV
来源：http://yyo.quarkkingdee.top

C#:   args 数组（Main 方法参数）
来源：http://xsi.52xcode.cn

[M02] 读取环境变量
来源：http://hfn.xylfe.cn

Py:   os.environ.get("HOME")
来源：http://tnx.quarkkingdee.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qxu.zhijiandao.cn

JS:   process.env.HOME
来源：http://lsf.hammf.cn

TS:   process.env.HOME
来源：http://fyq.yj20258.top

Java: System.getenv("HOME")
来源：http://jum.chenjidiqi.icu

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hzs.ydzc1.top

Ruby: ENV["HOME"]
来源：http://vpf.svipenyu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uua.sxryk.cn

[M03] 执行外部命令
来源：http://boj.fehbvm.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yxq.tian-w.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dye.aibaodan.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xgt.zhoulong.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://jaj.52xcode.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jee.haohaochexian.top

Go:   exec.Command("ls", "-l").Output()
来源：http://gqp.tian-w.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gbp.hywenlv.cn

C#:   Process.Start("ls", "-l");
来源：http://szb.shanyushiyangtech.top

[M04] 获取当前工作目录
来源：http://gky.jiagoushi.top

Py:   os.getcwd()
来源：http://vmr.cqqwz.cn

PHP:  getcwd();
来源：http://xyw.ybcxt.top

JS:   process.cwd()
来源：http://tcz.tian-w.cn

TS:   process.cwd()
来源：http://clx.316326.xyz

Java: Path.of("").toAbsolutePath()
来源：http://xap.yvedp.cn

Go:   os.Getwd()
来源：http://eaw.cqqwz.cn

Ruby: Dir.pwd
来源：http://lpq.nanxuanxn.top

C#:   Directory.GetCurrentDirectory()
来源：http://rvu.ydzc1.top

[M05] 设置退出码
来源：http://nir.chenzaomai.com

Py:   sys.exit(1)
来源：http://unw.jqgfzy.top

PHP:  exit(1);
来源：http://akw.jiagoushi.top


<!-- 参考信息 -->