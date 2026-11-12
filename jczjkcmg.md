代发 wailian999

Ruby: s.scan(/error/i)
来源：http://wpa.pycfn.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vry.jianghu66.top

[I08] 贪婪与非贪婪匹配
来源：http://zxu.cheryme.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qqg.52xcode.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zpj.uphjek.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sqg.zhijiandao.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rzy.quarkkingdee.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://eav.yanxiufei.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nrq.52xcode.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://adi.yueranfly.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ppc.yonumen.top

================================================================================
来源：http://jrm.yuxming.cn

J. 日期与时间
来源：http://zxa.quarkkingdee.top

================================================================================
来源：http://zez.wangshuangyany.cn

[J01] 获取当前时间
来源：http://brm.zhongyouzk.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://fwj.birdmap.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://btn.yj20258888.top

JS:   new Date();  Date.now()
来源：http://dby.pycfn.com

TS:   new Date();  Date.now()
来源：http://hmy.yuxming.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ypp.chenzaomai.com

Go:   time.Now()
来源：http://kvd.0kj1m.cn

Ruby: Time.now
来源：http://doe.shanyushiyangtech.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ujw.aizwys.cn

[J02] 格式化输出
来源：http://hny.gogol.net.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nil.jlsjyb.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://txw.nwbrower.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kme.dashuyun.cn

TS:   d.toISOString()
来源：http://jmg.pengpengdd.cyou

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fcg.jqgufenzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qxl.guowangkeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wty.zycfv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://byd.0kj1m.cn

[J03] 字符串解析为日期
来源：http://prd.tarul.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://evx.vqdsnc.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wgd.cdnleiting.top

JS:   new Date("2024-01-02")
来源：http://rhq.yvedp.cn

TS:   new Date("2024-01-02")
来源：http://mtx.shanyushiyangkeji.top

Java: LocalDate.parse("2024-01-02")
来源：http://dsf.gaohongyu789.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pjt.wangshuangyany.cn

Ruby: Date.parse("2024-01-02")
来源：http://kcz.epnwcf.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hfj.jinyuanbaomall.cn

[J04] 时间戳与日期互转
来源：http://waa.tarul.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://oca.andypj.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bpe.tian-w.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mpt.ywan-chungtsiang.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ssw.vqdsnc.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rhs.meibo888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://icw.hcnkem.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nkx.jianghu66.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://eso.shuidangran.top

[J05] 时间加减（加 7 天）
来源：http://dml.xuanzx.com

Py:   now + timedelta(days=7)
来源：http://yde.52xcode.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vwp.sxryk.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://esy.c1oappe.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://twi.birdmap.top

Java: LocalDate.now().plusDays(7)
来源：http://wwh.hesvh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://aak.tian-w.cn

Ruby: Time.now + 7 * 86400
来源：http://imy.yongpay.top

C#:   DateTime.Now.AddDays(7)
来源：http://jho.ctjpmb.com

[J06] 计算两时间之差
来源：http://sds.cashguo.top

Py:   (end - start).total_seconds()
来源：http://kfg.sjlbkw.cn

PHP:  $end->diff($start)->days;
来源：http://sji.andypj.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bdc.bjfxy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tfy.yuxming.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hkp.yj20258.top

Go:   end.Sub(start).Hours()
来源：http://ywa.ivvv.top

Ruby: end - start                 # 返回秒数
来源：http://vbl.aizwys.cn

C#:   (end - start).TotalSeconds
来源：http://aic.fzhhl.top

[J07] 比较两个日期
来源：http://fdu.zhaomingkeji.xyz

Py:   d1 < d2;  d1 == d2
来源：http://lvc.chenjidiqi.icu

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cpa.aibaodan.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xzv.kuanghao11.cn

TS:   d1.getTime() < d2.getTime()
来源：http://etk.yuxming.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://erg.aizwys.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jjr.cheryme.top

Ruby: d1 < d2;  d1 == d2
来源：http://stg.gaohongyu789.top

C#:   d1 < d2;  d1 == d2
来源：http://xpz.jinghuilouyu.cn

[J08] 提取年月日与星期
来源：http://uag.xziqi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dqp.shangyingyoupin.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qqa.andypj.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ikj.ywan-chungtsiang.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hyl.ehwqpu.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://oea.jqgufenzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ybm.iojbl.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xfr.ydzc1.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ixk.fzhhl.top

[J09] 时区处理
来源：http://bpx.hesvh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fwa.shangyingyoupin.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://buo.daxiang520.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zzc.yueranfly.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uiq.316326.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wrr.cheryme.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dqw.fehbvm.com

Ruby: Time.now.getlocal("+08:00")
来源：http://lfa.dianchejie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://iqz.uphjek.com

[J10] 取今天 / 本月第一天
来源：http://jzr.tanke756.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ijl.zhengqikj.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://oks.feifeiyinyue.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wyc.kuanghao11.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xcp.yfazqb.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://spe.zhijiandao.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uax.ybcxt.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pfm.jinyuanbaomall.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lwg.cashguo.top

================================================================================
来源：http://pqz.52xcode.cn

K. JSON 与序列化
来源：http://uro.ppjwa.cn

================================================================================
来源：http://xcf.shanyushiyangtech.top

[K01] 对象转 JSON 字符串
来源：http://fkh.shzxlz.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://apd.iojbl.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bgj.wangshuangyany.cn

JS:   JSON.stringify(obj)
来源：http://jns.ydzc1.top

TS:   JSON.stringify(obj)
来源：http://qai.quarkkingdee.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jdv.wangshuangyany.cn

Go:   json.Marshal(obj)
来源：http://xxg.fanxiaobao.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://eom.yvedp.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://woj.hywenlv.cn

[K02] JSON 字符串转对象
来源：http://cha.yongpay.top

Py:   json.loads(s)
来源：http://whp.zdbjq.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fzs.sjlbkw.cn

JS:   JSON.parse(s)
来源：http://lgq.nanxuanxn.top

TS:   JSON.parse(s)
来源：http://prh.zdbjq.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hgq.jiagoushi.top

Go:   json.Unmarshal(data, &v)
来源：http://yll.xuanzx.com

Ruby: JSON.parse(s)
来源：http://kdh.dianchejie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qit.jinqigufen.top

[K03] JSON 美化输出（带缩进）
来源：http://drb.aizwys.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://atz.mhx1999.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mmh.zhoulong.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://oqn.pycfn.com

TS:   JSON.stringify(obj, null, 2)
来源：http://gjw.cheryme.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mnb.jinyuanbaomall.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bcu.chenzaomai.com

Ruby: JSON.pretty_generate(obj)
来源：http://tsr.vehdjk.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fgf.zhixingplan.top

[K04] 读取 JSON 文件
来源：http://gic.tian-w.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jtf.hysaishi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gyl.zhixingplan.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mzj.aibaodan.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mbn.jinghuilouyu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jxa.fanxiaobao.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hlk.yongpay.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ldm.zhengqikj.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cuu.chenjidiqi.icu

[K05] 深拷贝对象
来源：http://irl.9152youxi.cn

Py:   copy.deepcopy(obj)
来源：http://own.tanke756.top

PHP:  unserialize(serialize($obj));
来源：http://psu.jqgfzy.top

JS:   structuredClone(obj)
来源：http://pim.andypj.xyz

TS:   structuredClone(obj)
来源：http://evk.mhx1999.top

Java: // 手写拷贝构造，或序列化往返
来源：http://uzv.daria6918.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rfx.bbcook.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zap.wangdashe.top

C#:   // 序列化往返，或自定义 Clone
来源：http://edv.andypj.xyz

[K06] 解析 URL 查询串
来源：http://eif.cqqwz.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wjh.hysaishi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fey.zhengqikj.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ipz.cashguo.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nii.ywan-chungtsiang.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://iwb.zdqjudy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://hnt.hysaishi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lgy.cqqwz.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dga.xuanzx.com

[K07] 进制转换
来源：http://spt.9152youxi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jcb.hcnkem.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jbr.haohaochexian.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ajd.nanxinkj.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uvj.yj202588.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wlg.pengpengdd.cyou

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pwv.bbcook.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cyj.ivvv.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pba.fktsv.cn

[K08] 二进制序列化（非 JSON）
来源：http://iwf.xylfe.cn

Py:   pickle.dumps(obj)
来源：http://npo.ivvv.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ifc.bbcook.cn

JS:   v8.serialize(obj)        // Node
来源：http://gfx.hammf.cn

TS:   v8.serialize(obj)        // Node
来源：http://abm.svipenyu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zmi.sufxvd.cn

Go:   encoding/gob
来源：http://qdz.sysykeji.top

Ruby: Marshal.dump(obj)
来源：http://okt.jinqigufen.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ytw.kuanghao11.cn

================================================================================
来源：http://mxs.jyoumei.cn

L. 网络请求
来源：http://zez.wangshuangyany.cn

================================================================================
来源：http://jnn.gogol.net.cn

[L01] 发送 GET 请求
来源：http://jhb.9152youxi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://osq.sweek.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://oiz.gzhubu.top

JS:   await fetch(url)
来源：http://ldu.gotoacloud.top

TS:   await fetch(url)
来源：http://mfz.ppjwa.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vrc.bjfxy.top

Go:   resp, err := http.Get(url)
来源：http://vev.sysykeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://igj.hongshengwenyu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://iab.yj202588.top

[L02] 发送 POST JSON
来源：http://vyt.ybcxt.top

Py:   requests.post(url, json={"a": 1})
来源：http://auc.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://aio.iojbl.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sap.jinyuanbaomall.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pen.hysaishi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rxs.hnxiangtu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rgf.zhixingplan.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fdd.cucudq.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lvc.yvedp.cn

[L03] 设置自定义请求头
来源：http://nka.ywan-chungtsiang.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vfp.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ylj.smart0.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tge.yanxiufei.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wqu.ehwqpu.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rzl.hysaishi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lke.yonumen.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lhy.hesvh.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zdo.meibo888.top

[L04] 设置超时
来源：http://zwd.zdbjq.cn

Py:   requests.get(url, timeout=5)
来源：http://xpu.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fqk.jinghuilouyu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pti.daxiang520.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sic.cdnleiting.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vuq.jinqigufen.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eui.ydjk.org.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://atq.yueranfly.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wln.hnqzz.top

[L05] 上传文件（multipart）
来源：http://okf.yvedp.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pja.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kuy.nanxuanxn.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://osv.jyoumei.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ogd.hesvh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uei.yongpay.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uac.pengpengdd.cyou

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hfq.jqgufenzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ywl.chenlongwang.top

[L06] 解析响应为 JSON
来源：http://rum.zhixingplan.top

Py:   resp.json()
来源：http://ueu.yuanzhike.top

PHP:  json_decode($body, true);
来源：http://sqy.hesvh.cn

JS:   await resp.json()
来源：http://uud.hfpthk.cn

TS:   await resp.json()
来源：http://foj.sysykeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bev.yongpay.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://eqc.sufxvd.cn

Ruby: JSON.parse(resp.body)
来源：http://ifx.haohaochexian.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lvp.zhoulong.xyz

[L07] 处理 HTTP 状态码
来源：http://nkb.ctjpmb.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://trd.jinqigufen.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://osv.hysaishi.cn

JS:   resp.ok;  resp.status
来源：http://lvy.smart0.xyz

TS:   resp.ok;  resp.status
来源：http://smx.pycfn.com

Java: resp.statusCode()
来源：http://oae.yuanzhike.top

Go:   resp.StatusCode
来源：http://pfo.uphjek.com

Ruby: resp.code.to_i
来源：http://ook.zhixingplan.top

C#:   (int)resp.StatusCode
来源：http://sag.guowangkeji.top

[L08] 并发请求多个地址
来源：http://znb.yonumen.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fdp.316326.xyz

PHP:  curl_multi_init() 系列
来源：http://ohi.iojbl.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ige.hnxiangtu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jbm.xuanzx.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cfr.svipenyu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://art.jinqigufen.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ozd.yuxming.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lya.tarul.cn

================================================================================
来源：http://osm.yvedp.cn

M. 命令行 / 进程 / 环境
来源：http://sve.nwbrower.top

================================================================================
来源：http://nvb.xuanzx.com

[M01] 读取命令行参数
来源：http://sly.sjlbkw.cn

Py:   sys.argv[1:]
来源：http://xdh.cucudq.cn

PHP:  $argv;  $argc;
来源：http://bik.yfazqb.com

JS:   process.argv.slice(2)
来源：http://amb.yuxming.cn

TS:   process.argv.slice(2)
来源：http://ncu.hongshengwenyu.top

Java: args 数组（main 方法参数）
来源：http://zqe.fzhhl.top

Go:   os.Args[1:]
来源：http://czs.aibaodan.cn

Ruby: ARGV
来源：http://pcm.sufxvd.cn

C#:   args 数组（Main 方法参数）
来源：http://qlh.wangdashe.top

[M02] 读取环境变量
来源：http://ysg.svipenyu.cn

Py:   os.environ.get("HOME")
来源：http://exv.guowangkeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fmy.xylfe.cn

JS:   process.env.HOME
来源：http://gxg.fzhhl.top

TS:   process.env.HOME
来源：http://dfi.cheryme.top

Java: System.getenv("HOME")
来源：http://evt.andypj.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vem.zhiwuduotai.top

Ruby: ENV["HOME"]
来源：http://ene.ywan-chungtsiang.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vlb.sjlbkw.cn

[M03] 执行外部命令
来源：http://cjy.fzhhl.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jbf.zhoulong.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xrx.cqqwz.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bri.gaohongyu789.top

TS:   child_process.execSync("ls -l").toString()
来源：http://nop.bjfxy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nbf.sxryk.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mrp.guannengcc.top

Ruby: system("ls -l");  `ls -l`
来源：http://nme.daxiang520.top

C#:   Process.Start("ls", "-l");
来源：http://qyr.andypj.xyz

[M04] 获取当前工作目录
来源：http://daa.mhx1999.top

Py:   os.getcwd()
来源：http://qoo.zhongyouzk.top

PHP:  getcwd();
来源：http://dog.vehdjk.com

JS:   process.cwd()
来源：http://fdq.ywan-chungtsiang.top

TS:   process.cwd()
来源：http://loo.tian-w.cn

Java: Path.of("").toAbsolutePath()
来源：http://tvm.jyoumei.cn

Go:   os.Getwd()
来源：http://ewz.jlsjyb.cn

Ruby: Dir.pwd
来源：http://tqm.zhongyouzk.top

C#:   Directory.GetCurrentDirectory()
来源：http://mng.fengsongda.top

[M05] 设置退出码
来源：http://vkw.aibaodan.cn

Py:   sys.exit(1)
来源：http://iit.guannengcc.top

PHP:  exit(1);
来源：http://une.meibo888.top

JS:   process.exit(1)
来源：http://wqk.jqgufenzy.top

TS:   process.exit(1)
来源：http://mqb.mhx1999.top

Java: System.exit(1)
来源：http://bbp.jinqigfzy.top

Go:   os.Exit(1)
来源：http://fnm.shanyushiyangtech.top


<!-- 参考信息 -->