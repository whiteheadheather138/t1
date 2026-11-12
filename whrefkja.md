代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dga.yuanzhike.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yjk.shuidangran.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gvs.kuanghao11.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://efi.hnxiangtu.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vyn.vehdjk.com

[I07] 忽略大小写与多行模式
来源：http://amp.yj202588.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qil.zycfv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://oql.zhoulong.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hos.smart0.xyz

TS:   /error/gim
来源：http://hey.sysykeji.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hiq.hesvh.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://quv.smart0.xyz

Ruby: s.scan(/error/i)
来源：http://itr.sxryk.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lkw.vqdsnc.cn

[I08] 贪婪与非贪婪匹配
来源：http://cws.wangdashe.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lwx.xuanzx.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://col.tianlin.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://poo.shanyushiyangkeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mwm.hammf.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hzp.hysaishi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ura.yj20258.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ebp.dianchejie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://edh.yangfankeji.com

================================================================================
来源：http://cms.hnqzz.top

J. 日期与时间
来源：http://wjm.feifeiyinyue.top

================================================================================
来源：http://fam.fktsv.cn

[J01] 获取当前时间
来源：http://xhw.zhengqikj.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://aye.yfazqb.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://srs.xuanzx.com

JS:   new Date();  Date.now()
来源：http://zgx.ppjwa.cn

TS:   new Date();  Date.now()
来源：http://qjy.shanyushiyangtech.top

Java: LocalDateTime.now();  Instant.now()
来源：http://eij.hesvh.cn

Go:   time.Now()
来源：http://kzc.jianghu66.top

Ruby: Time.now
来源：http://xmb.yj20258888.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hkg.haohaochexian.top

[J02] 格式化输出
来源：http://etz.zhaomingkeji.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eet.wangdashe.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ejw.ywan-chungtsiang.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kow.yfazqb.com

TS:   d.toISOString()
来源：http://www.zdbjq.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jtu.shzxlz.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://slg.guannengcc.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zgc.jinghuilouyu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vgw.gogol.net.cn

[J03] 字符串解析为日期
来源：http://tho.jianghu66.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tub.tian-w.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://byu.tianlin.xyz

JS:   new Date("2024-01-02")
来源：http://dzc.zdbjq.cn

TS:   new Date("2024-01-02")
来源：http://kni.cashguo.top

Java: LocalDate.parse("2024-01-02")
来源：http://mrf.shanyushiyangkeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dms.zhengqikj.top

Ruby: Date.parse("2024-01-02")
来源：http://bug.yj202588.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nhr.zdbjq.cn

[J04] 时间戳与日期互转
来源：http://poq.xylfe.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wsw.smart0.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mkf.fehbvm.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tep.c1oappe.top

TS:   Math.floor(Date.now() / 1000)
来源：http://xxe.xingfuxueyuan.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fuw.c1oappe.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mia.sxryk.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vpr.shzxlz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jmo.ydjk.org.cn

[J05] 时间加减（加 7 天）
来源：http://nxu.guowangkeji.top

Py:   now + timedelta(days=7)
来源：http://wnu.fehbvm.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://fle.birdmap.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uin.zhongyouzk.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qex.yuanzhike.top

Java: LocalDate.now().plusDays(7)
来源：http://zni.meibo888.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qct.fzhhl.top

Ruby: Time.now + 7 * 86400
来源：http://cei.dashuyun.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wpp.feifeiyinyue.top

[J06] 计算两时间之差
来源：http://qsf.jiagoushi.top

Py:   (end - start).total_seconds()
来源：http://bnl.tanke756.top

PHP:  $end->diff($start)->days;
来源：http://owf.chenzaomai.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tey.svipenyu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pwe.haohaochexian.top

Java: Duration.between(start, end).toSeconds()
来源：http://cec.xylfe.cn

Go:   end.Sub(start).Hours()
来源：http://els.0kj1m.cn

Ruby: end - start                 # 返回秒数
来源：http://qjy.iojbl.cn

C#:   (end - start).TotalSeconds
来源：http://dbl.epnwcf.com

[J07] 比较两个日期
来源：http://oxo.shangyingyoupin.top

Py:   d1 < d2;  d1 == d2
来源：http://alc.ybcxt.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ckl.zhiwuduotai.top

JS:   d1.getTime() < d2.getTime()
来源：http://ygd.tanke756.top

TS:   d1.getTime() < d2.getTime()
来源：http://ahf.fehbvm.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fnw.epnwcf.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uup.shangyingyoupin.top

Ruby: d1 < d2;  d1 == d2
来源：http://epw.ywan-chungtsiang.top

C#:   d1 < d2;  d1 == d2
来源：http://bux.0kj1m.cn

[J08] 提取年月日与星期
来源：http://kzl.ydjk.org.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://oca.ydzc1.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mrm.uphjek.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yil.bbcook.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oxl.snrcjt.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bbx.daria6918.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pcz.fehbvm.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://imi.yanxiufei.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wxd.zhaomingkeji.xyz

[J09] 时区处理
来源：http://ibu.yangfankeji.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wpf.yuxming.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gwh.xingfuxueyuan.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dqp.c1oappe.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lyq.havefunace.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nez.snrcjt.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qbo.zdqjudy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://jdm.zhixingplan.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uhp.ctjpmb.com

[J10] 取今天 / 本月第一天
来源：http://dwm.dianchejie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xlw.fehbvm.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xgl.fehbvm.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wuf.zhiwuduotai.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qsf.zhengqikj.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zuc.ybcxt.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sqg.ybcxt.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yzc.zhijiandao.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nfc.zhixingplan.top

================================================================================
来源：http://ngc.fzhhl.top

K. JSON 与序列化
来源：http://rfc.hfpthk.cn

================================================================================
来源：http://hep.wangshuangyany.cn

[K01] 对象转 JSON 字符串
来源：http://vmf.cqqwz.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xjy.wangdashe.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hnr.chenjidiqi.icu

JS:   JSON.stringify(obj)
来源：http://tjc.iojbl.cn

TS:   JSON.stringify(obj)
来源：http://xwu.daria6918.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://klx.dashuyun.cn

Go:   json.Marshal(obj)
来源：http://syp.chenzaomai.com

Ruby: obj.to_json                                     // require "json"
来源：http://tzh.yonumen.top

C#:   JsonSerializer.Serialize(obj)
来源：http://eld.aibaodan.cn

[K02] JSON 字符串转对象
来源：http://sqa.ydzc1.top

Py:   json.loads(s)
来源：http://pdk.zdqjudy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gam.feifeiyinyue.top

JS:   JSON.parse(s)
来源：http://wen.zhoulong.xyz

TS:   JSON.parse(s)
来源：http://jba.yueranfly.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bfu.yj20258888.top

Go:   json.Unmarshal(data, &v)
来源：http://pho.tanke756.top

Ruby: JSON.parse(s)
来源：http://lpv.daria6918.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://knh.jyoumei.cn

[K03] JSON 美化输出（带缩进）
来源：http://coz.ydzc1.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qlt.sxryk.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xpk.hywenlv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hvl.dianchejie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sql.feifeiyinyue.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zuo.fehbvm.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hwe.cdnleiting.top

Ruby: JSON.pretty_generate(obj)
来源：http://pze.mhx1999.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hwi.gotoacloud.top

[K04] 读取 JSON 文件
来源：http://jwv.gzhubu.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mpl.zhengqikj.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fos.yj20258.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://edg.cheryme.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yai.tian-w.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bwx.yj20258.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oll.shanyushiyangkeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://hfv.xinyue.icu

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xtv.jinyuanbaomall.cn

[K05] 深拷贝对象
来源：http://sfk.vehdjk.com

Py:   copy.deepcopy(obj)
来源：http://tpf.dianchejie.cn

PHP:  unserialize(serialize($obj));
来源：http://dqv.xziqi.cn

JS:   structuredClone(obj)
来源：http://lgp.yongpay.top

TS:   structuredClone(obj)
来源：http://bww.jianghu66.top

Java: // 手写拷贝构造，或序列化往返
来源：http://fkk.wangdashe.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://iwg.zhaomingkeji.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gzm.iojbl.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://iwe.fengsongda.top

[K06] 解析 URL 查询串
来源：http://fki.yonumen.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lam.daria6918.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fte.andypj.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bsb.dianchejie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lgg.gotoacloud.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jow.dianchejie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://jch.daxiang520.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fdd.yj202588.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://env.ehwqpu.com

[K07] 进制转换
来源：http://dkx.wangshuangyany.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tln.yuxming.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://olm.tianlin.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xvc.52xcode.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xen.daria6918.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://iyh.ctjpmb.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cal.chenlongwang.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pei.zhixingplan.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kbo.hcnkem.com

[K08] 二进制序列化（非 JSON）
来源：http://elx.xuanzx.com

Py:   pickle.dumps(obj)
来源：http://nrj.zhoulong.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://afe.hesvh.cn

JS:   v8.serialize(obj)        // Node
来源：http://maa.daxiang520.top

TS:   v8.serialize(obj)        // Node
来源：http://yte.jqgufenzy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wrm.vehdjk.com

Go:   encoding/gob
来源：http://mkb.sufxvd.cn

Ruby: Marshal.dump(obj)
来源：http://sow.bjfxy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cft.shangyingyoupin.top

================================================================================
来源：http://zel.mhx1999.top

L. 网络请求
来源：http://dxq.tanke756.top

================================================================================
来源：http://hpq.shuidangran.top

[L01] 发送 GET 请求
来源：http://nzl.aibaodan.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dgn.shzxlz.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zyh.fengsongda.top

JS:   await fetch(url)
来源：http://grj.ctjpmb.com

TS:   await fetch(url)
来源：http://ewk.jinyuanbaomall.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xum.uphjek.com

Go:   resp, err := http.Get(url)
来源：http://cin.feifeiyinyue.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dii.jianghu66.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qjs.ctjpmb.com

[L02] 发送 POST JSON
来源：http://gcd.0kj1m.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gds.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://eyt.vehdjk.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ynj.iojbl.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jpm.tianlin.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uqy.yongpay.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ubi.feifeiyinyue.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ahp.jinqigufen.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pac.yvedp.cn

[L03] 设置自定义请求头
来源：http://qqm.ybcxt.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ehc.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nnj.jinyuanbaomall.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hbc.pengpengdd.cyou

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qym.nanxuanxn.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rse.ywan-chungtsiang.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mip.nwbrower.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://szo.tianlin.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pio.xinyue.icu

[L04] 设置超时
来源：http://tsc.nanxinkj.top

Py:   requests.get(url, timeout=5)
来源：http://han.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qsl.cdnleiting.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yyo.52xcode.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://imc.iojbl.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bvg.ppjwa.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://glg.yj20258888.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xoi.sufxvd.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hgo.c1oappe.top

[L05] 上传文件（multipart）
来源：http://xgj.gotoacloud.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://olg.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lfy.guowangkeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cjj.fzhhl.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://khf.fktsv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bcn.ehwqpu.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hvr.zhaomingkeji.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wdx.jqgufenzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pbj.hysaishi.cn

[L06] 解析响应为 JSON
来源：http://ylw.shanyushiyangkeji.top

Py:   resp.json()
来源：http://tmx.pycfn.com

PHP:  json_decode($body, true);
来源：http://vtc.fengsongda.top

JS:   await resp.json()
来源：http://lgn.shzxlz.cn

TS:   await resp.json()
来源：http://czi.chenjidiqi.icu

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fgp.iojbl.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ebx.chenlongwang.top

Ruby: JSON.parse(resp.body)
来源：http://vjn.jqgufenzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kwj.zhaomingkeji.xyz

[L07] 处理 HTTP 状态码
来源：http://ngb.316326.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://haa.sweek.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://isz.xingfuxueyuan.xyz

JS:   resp.ok;  resp.status
来源：http://wwo.hesvh.cn

TS:   resp.ok;  resp.status
来源：http://orh.c1oappe.top

Java: resp.statusCode()
来源：http://jsu.sufxvd.cn

Go:   resp.StatusCode
来源：http://rdh.jinqigfzy.top

Ruby: resp.code.to_i
来源：http://scu.sxryk.cn

C#:   (int)resp.StatusCode
来源：http://nkv.guowangkeji.top

[L08] 并发请求多个地址
来源：http://ett.xylfe.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bpa.feifeiyinyue.top

PHP:  curl_multi_init() 系列
来源：http://fln.yueranfly.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ovm.snrcjt.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ylb.9152youxi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://chd.jlsjyb.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kli.sysykeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://syb.xziqi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mqe.zycfv.cn

================================================================================
来源：http://blj.cashguo.top

M. 命令行 / 进程 / 环境
来源：http://aoa.bjfxy.top

================================================================================
来源：http://wdd.iojbl.cn

[M01] 读取命令行参数
来源：http://blx.cdnleiting.top

Py:   sys.argv[1:]
来源：http://ggu.aibaodan.cn

PHP:  $argv;  $argc;
来源：http://dpq.tian-w.cn

JS:   process.argv.slice(2)
来源：http://ttl.zhoulong.xyz

TS:   process.argv.slice(2)
来源：http://vru.shzxlz.cn

Java: args 数组（main 方法参数）
来源：http://yjv.cqqwz.cn

Go:   os.Args[1:]
来源：http://cgu.sjlbkw.cn

Ruby: ARGV
来源：http://zea.c1oappe.top

C#:   args 数组（Main 方法参数）
来源：http://zen.xuanzx.com

[M02] 读取环境变量
来源：http://mhu.aibaodan.cn

Py:   os.environ.get("HOME")
来源：http://gqv.shanyushiyangkeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ono.zdqjudy.top

JS:   process.env.HOME
来源：http://qkd.zdbjq.cn

TS:   process.env.HOME
来源：http://xgw.xingfuxueyuan.xyz

Java: System.getenv("HOME")
来源：http://ixm.gogol.net.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jkd.zhiwuduotai.top

Ruby: ENV["HOME"]
来源：http://jse.9152youxi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vum.hcnkem.com

[M03] 执行外部命令
来源：http://vxh.uphjek.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yhd.jlsjyb.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vtk.sysykeji.top

JS:   child_process.execSync("ls -l").toString()
来源：http://mvc.fanxiaobao.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://kdu.pengpengdd.cyou

Java: new ProcessBuilder("ls", "-l").start()
来源：http://eeq.52xcode.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://atl.zhiwuduotai.top

Ruby: system("ls -l");  `ls -l`
来源：http://zod.zhixingplan.top

C#:   Process.Start("ls", "-l");
来源：http://egw.yangfankeji.com

[M04] 获取当前工作目录
来源：http://wao.bbcook.cn

Py:   os.getcwd()
来源：http://cqw.xziqi.cn

PHP:  getcwd();
来源：http://sqd.yanxiufei.cn

JS:   process.cwd()
来源：http://ttc.pengpengdd.cyou


<!-- 参考信息 -->