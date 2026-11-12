代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://brl.dianchejie.cn

TS:   /error/gim
来源：http://fas.shuidangran.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rls.0kj1m.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ydt.hnxiangtu.top

Ruby: s.scan(/error/i)
来源：http://pae.hammf.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://myk.zycfv.cn

[I08] 贪婪与非贪婪匹配
来源：http://pym.pengpengdd.cyou

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cxx.gzhubu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vdp.bjfxy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hoy.cashguo.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dvk.shanyushiyangtech.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://kgr.yj20258888.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dbt.zhongyouzk.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bvo.guowangkeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mdz.shanyushiyangtech.top

================================================================================
来源：http://aff.yuanzhike.top

J. 日期与时间
来源：http://qrv.daria6918.cn

================================================================================
来源：http://gaj.quarkkingdee.top

[J01] 获取当前时间
来源：http://pjb.meibo888.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://hso.sufxvd.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nbn.cucudq.cn

JS:   new Date();  Date.now()
来源：http://fsa.feifeiyinyue.top

TS:   new Date();  Date.now()
来源：http://ene.gzhubu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://npg.cqqwz.cn

Go:   time.Now()
来源：http://vjj.tianlin.xyz

Ruby: Time.now
来源：http://cqj.cucudq.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ied.snrcjt.cn

[J02] 格式化输出
来源：http://drj.wangdashe.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uzu.uphjek.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kri.9152youxi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yfl.vehdjk.com

TS:   d.toISOString()
来源：http://zme.jlsjyb.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lmr.tianlin.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zaw.zdbjq.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://chj.kuanghao11.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://igp.jinyuanbaomall.cn

[J03] 字符串解析为日期
来源：http://lrx.wangshuangyany.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dtd.ivvv.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yyj.jqgufenzy.top

JS:   new Date("2024-01-02")
来源：http://bnb.jqgfzy.top

TS:   new Date("2024-01-02")
来源：http://nla.shangyingyoupin.top

Java: LocalDate.parse("2024-01-02")
来源：http://hll.shzxlz.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rdu.iojbl.cn

Ruby: Date.parse("2024-01-02")
来源：http://sgd.shanyushiyangtech.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zve.ydzc1.top

[J04] 时间戳与日期互转
来源：http://tvu.feifeiyinyue.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hti.nwbrower.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uga.dianchejie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mwg.52xcode.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://psm.hcnkem.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uvw.ybcxt.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uio.ivvv.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://auj.haohaochexian.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ytu.xingfuxueyuan.xyz

[J05] 时间加减（加 7 天）
来源：http://hga.cucudq.cn

Py:   now + timedelta(days=7)
来源：http://ptq.tian-w.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vno.haohaochexian.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ysx.jianghu66.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://oiv.fanxiaobao.xyz

Java: LocalDate.now().plusDays(7)
来源：http://eph.dashuyun.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nbm.hfpthk.cn

Ruby: Time.now + 7 * 86400
来源：http://yhf.316326.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://ozl.mhx1999.top

[J06] 计算两时间之差
来源：http://eaf.jqgfzy.top

Py:   (end - start).total_seconds()
来源：http://pku.nanxinkj.top

PHP:  $end->diff($start)->days;
来源：http://nja.ctjpmb.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://iys.jinqigfzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fwb.zdqjudy.top

Java: Duration.between(start, end).toSeconds()
来源：http://zzi.xingfuxueyuan.xyz

Go:   end.Sub(start).Hours()
来源：http://dlo.shzxlz.cn

Ruby: end - start                 # 返回秒数
来源：http://goj.yj20258.top

C#:   (end - start).TotalSeconds
来源：http://jjd.fanxiaobao.xyz

[J07] 比较两个日期
来源：http://kur.gotoacloud.top

Py:   d1 < d2;  d1 == d2
来源：http://rha.cdnleiting.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nth.nanxinkj.top

JS:   d1.getTime() < d2.getTime()
来源：http://yrf.ivvv.top

TS:   d1.getTime() < d2.getTime()
来源：http://ypr.gogol.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kut.ppjwa.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mbn.zhijiandao.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vot.9152youxi.cn

C#:   d1 < d2;  d1 == d2
来源：http://fso.cucudq.cn

[J08] 提取年月日与星期
来源：http://xvq.xuetiantiany.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dpy.sweek.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vij.cdnleiting.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rkd.fktsv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://utk.tarul.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pkh.xuanzx.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xkf.daxiang520.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xlp.jlsjyb.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://oqv.pycfn.com

[J09] 时区处理
来源：http://fiy.tanke756.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hvo.cqqwz.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nlc.cheryme.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qcc.ctjpmb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mtg.jiagoushi.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cbd.wangshuangyany.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yum.jinyuanbaomall.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fph.ivvv.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wul.zhijiandao.cn

[J10] 取今天 / 本月第一天
来源：http://mxx.feifeiyinyue.top

Py:   date.today();  date.today().replace(day=1)
来源：http://vlr.yuxming.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bmp.pengpengdd.cyou

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gkl.guowangkeji.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pjh.jyoumei.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://suv.gogol.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rnu.uphjek.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bvj.fehbvm.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qiw.ywan-chungtsiang.top

================================================================================
来源：http://atb.jinqigfzy.top

K. JSON 与序列化
来源：http://qam.guannengcc.top

================================================================================
来源：http://lmh.yj202588.top

[K01] 对象转 JSON 字符串
来源：http://tut.bbcook.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://izq.yuxming.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ycj.yonumen.top

JS:   JSON.stringify(obj)
来源：http://hrb.xuetiantiany.cn

TS:   JSON.stringify(obj)
来源：http://vhc.dashuyun.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://efo.shangyingyoupin.top

Go:   json.Marshal(obj)
来源：http://muv.hongshengwenyu.top

Ruby: obj.to_json                                     // require "json"
来源：http://pko.zhaomingkeji.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://zfq.jyoumei.cn

[K02] JSON 字符串转对象
来源：http://wub.zdqjudy.top

Py:   json.loads(s)
来源：http://qut.fanxiaobao.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sdx.hnxiangtu.top

JS:   JSON.parse(s)
来源：http://sqa.hongshengwenyu.top

TS:   JSON.parse(s)
来源：http://qfh.cqqwz.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vdd.hywenlv.cn

Go:   json.Unmarshal(data, &v)
来源：http://qct.aibaodan.cn

Ruby: JSON.parse(s)
来源：http://glx.ehwqpu.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ysj.52xcode.cn

[K03] JSON 美化输出（带缩进）
来源：http://mby.jianghu66.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kgi.jianghu66.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xol.chenjidiqi.icu

JS:   JSON.stringify(obj, null, 2)
来源：http://cne.fanxiaobao.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://evv.jyoumei.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kty.0kj1m.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sri.yvedp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ckr.jinghuilouyu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hvt.aibaodan.cn

[K04] 读取 JSON 文件
来源：http://qxn.wangshuangyany.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pvf.zhaomingkeji.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://llu.jqgufenzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iqt.9152youxi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rgj.jinqigufen.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yoq.shanyushiyangkeji.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xqo.aizwys.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://swb.fengsongda.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zdh.jinghuilouyu.cn

[K05] 深拷贝对象
来源：http://jwq.hfpthk.cn

Py:   copy.deepcopy(obj)
来源：http://hiw.tian-w.cn

PHP:  unserialize(serialize($obj));
来源：http://qqu.pycfn.com

JS:   structuredClone(obj)
来源：http://eoq.pycfn.com

TS:   structuredClone(obj)
来源：http://rek.xinyue.icu

Java: // 手写拷贝构造，或序列化往返
来源：http://ofn.hesvh.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://trq.feifeiyinyue.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://elf.yj202588.top

C#:   // 序列化往返，或自定义 Clone
来源：http://rqq.uphjek.com

[K06] 解析 URL 查询串
来源：http://yme.gotoacloud.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nnp.fanxiaobao.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://whq.zhixingplan.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cnw.shuidangran.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bar.jyoumei.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://slz.yongpay.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jhg.hywenlv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tsr.fzhhl.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xtr.xinyue.icu

[K07] 进制转换
来源：http://vdr.sweek.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mpj.yj202588.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ejq.jinyuanbaomall.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vle.chenlongwang.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qgl.guowangkeji.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vfh.birdmap.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://apt.ydzc1.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cbz.jinyuanbaomall.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://czi.birdmap.top

[K08] 二进制序列化（非 JSON）
来源：http://ztn.sweek.top

Py:   pickle.dumps(obj)
来源：http://rnt.uphjek.com

PHP:  serialize($obj);  unserialize($s);
来源：http://rnr.ybcxt.top

JS:   v8.serialize(obj)        // Node
来源：http://dtf.aibaodan.cn

TS:   v8.serialize(obj)        // Node
来源：http://ppk.hammf.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tti.wangshuangyany.cn

Go:   encoding/gob
来源：http://obi.dashuyun.cn

Ruby: Marshal.dump(obj)
来源：http://alp.yonumen.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lsk.zhixingplan.top

================================================================================
来源：http://iif.jiagoushi.top

L. 网络请求
来源：http://luz.yuanzhike.top

================================================================================
来源：http://zxv.ctjpmb.com

[L01] 发送 GET 请求
来源：http://ggc.guowangkeji.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jze.hammf.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://oho.shangyingyoupin.top

JS:   await fetch(url)
来源：http://exx.nanxinkj.top

TS:   await fetch(url)
来源：http://ukz.jinghuilouyu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hcx.yueranfly.top

Go:   resp, err := http.Get(url)
来源：http://zcv.c1oappe.top

Ruby: Net::HTTP.get(URI(url))
来源：http://icz.snrcjt.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gby.hammf.cn

[L02] 发送 POST JSON
来源：http://loq.zhixingplan.top

Py:   requests.post(url, json={"a": 1})
来源：http://car.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kqy.zhengqikj.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jrm.9152youxi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gck.hnqzz.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lnb.bbcook.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yev.xingfuxueyuan.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lrb.haohaochexian.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gbt.chenjidiqi.icu

[L03] 设置自定义请求头
来源：http://xzq.cdnleiting.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wpp.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jtk.hywenlv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zvq.dianchejie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rbq.cashguo.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gic.fanxiaobao.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ykr.fengsongda.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://svp.aizwys.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://swm.uphjek.com

[L04] 设置超时
来源：http://mtr.redwolf501.top

Py:   requests.get(url, timeout=5)
来源：http://sff.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ume.cqqwz.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dxd.yuanzhike.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://npw.yuanzhike.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pay.xinyue.icu

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://khw.zhiwuduotai.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nmj.dianchejie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ciq.jiagoushi.top

[L05] 上传文件（multipart）
来源：http://wxn.smart0.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kod.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ciu.pycfn.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lkj.yj20258888.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://iuu.zycfv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tkt.gaohongyu789.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://axs.jinqigfzy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kii.ctjpmb.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zve.birdmap.top

[L06] 解析响应为 JSON
来源：http://clf.yonumen.top

Py:   resp.json()
来源：http://cnx.gaohongyu789.top

PHP:  json_decode($body, true);
来源：http://rby.zhaomingkeji.xyz

JS:   await resp.json()
来源：http://nts.shuidangran.top

TS:   await resp.json()
来源：http://vni.nwbrower.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cvm.hesvh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uee.kuanghao11.cn

Ruby: JSON.parse(resp.body)
来源：http://eyq.jiagoushi.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hpn.0kj1m.cn

[L07] 处理 HTTP 状态码
来源：http://hit.wangshuangyany.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vel.ywan-chungtsiang.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wak.shanyushiyangkeji.top

JS:   resp.ok;  resp.status
来源：http://iij.yuanzhike.top

TS:   resp.ok;  resp.status
来源：http://eiy.cdnleiting.top

Java: resp.statusCode()
来源：http://maf.ydjk.org.cn

Go:   resp.StatusCode
来源：http://xrm.xuetiantiany.cn

Ruby: resp.code.to_i
来源：http://dej.fehbvm.com

C#:   (int)resp.StatusCode
来源：http://fvu.9152youxi.cn

[L08] 并发请求多个地址
来源：http://onn.yfazqb.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lii.nanxuanxn.top

PHP:  curl_multi_init() 系列
来源：http://sjd.zhoulong.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dag.snrcjt.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ioy.fktsv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dnu.hcnkem.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://stw.nanxinkj.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://win.sxryk.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mvz.xuetiantiany.cn

================================================================================
来源：http://krn.tarul.cn

M. 命令行 / 进程 / 环境
来源：http://xlv.xuetiantiany.cn

================================================================================
来源：http://lmp.tarul.cn

[M01] 读取命令行参数
来源：http://tsk.hnxiangtu.top

Py:   sys.argv[1:]
来源：http://efn.yuxming.cn

PHP:  $argv;  $argc;
来源：http://lwx.redwolf501.top

JS:   process.argv.slice(2)
来源：http://fav.yonumen.top

TS:   process.argv.slice(2)
来源：http://nep.ydjk.org.cn

Java: args 数组（main 方法参数）
来源：http://xkx.hesvh.cn

Go:   os.Args[1:]
来源：http://wil.shanyushiyangtech.top

Ruby: ARGV
来源：http://bhq.dashuyun.cn

C#:   args 数组（Main 方法参数）
来源：http://jmr.sysykeji.top

[M02] 读取环境变量
来源：http://yct.shanyushiyangtech.top

Py:   os.environ.get("HOME")
来源：http://bft.uphjek.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://enu.yonumen.top

JS:   process.env.HOME
来源：http://ats.jqgfzy.top

TS:   process.env.HOME
来源：http://vxw.fzhhl.top

Java: System.getenv("HOME")
来源：http://rsn.chenjidiqi.icu

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dre.jyoumei.cn

Ruby: ENV["HOME"]
来源：http://qnp.c1oappe.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oku.redwolf501.top

[M03] 执行外部命令
来源：http://tlu.jiagoushi.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cyv.fanxiaobao.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tuo.cdnleiting.top

JS:   child_process.execSync("ls -l").toString()
来源：http://reg.wangshuangyany.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bwp.sufxvd.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://onh.daxiang520.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ini.fengsongda.top

Ruby: system("ls -l");  `ls -l`
来源：http://dra.ybcxt.top

C#:   Process.Start("ls", "-l");
来源：http://bcw.feifeiyinyue.top

[M04] 获取当前工作目录
来源：http://fgi.daria6918.cn

Py:   os.getcwd()
来源：http://sgm.zhijiandao.cn

PHP:  getcwd();
来源：http://bjc.zdbjq.cn

JS:   process.cwd()
来源：http://dvl.zhengqikj.top

TS:   process.cwd()
来源：http://hbn.sufxvd.cn

Java: Path.of("").toAbsolutePath()
来源：http://veh.cucudq.cn

Go:   os.Getwd()
来源：http://cze.ctjpmb.com

Ruby: Dir.pwd
来源：http://hqt.meibo888.top

C#:   Directory.GetCurrentDirectory()
来源：http://qjm.feifeiyinyue.top

[M05] 设置退出码
来源：http://kco.hysaishi.cn

Py:   sys.exit(1)
来源：http://lil.meibo888.top

PHP:  exit(1);
来源：http://okg.hcnkem.com


<!-- 参考信息 -->