代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dpq.zhengqikj.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pui.jinqigufen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://thp.dianchejie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://erv.shangyingyoupin.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fet.hnxiangtu.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uyy.yanxiufei.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yoc.9152youxi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fjn.yj202588.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uun.shanyushiyangtech.top

[I07] 忽略大小写与多行模式
来源：http://kzi.haohaochexian.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vsy.jqgufenzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tqm.jqgfzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://soq.tanke756.top

TS:   /error/gim
来源：http://iyb.gotoacloud.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vkb.shanyushiyangtech.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://moh.jinqigfzy.top

Ruby: s.scan(/error/i)
来源：http://xxb.yangfankeji.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nbb.guannengcc.top

[I08] 贪婪与非贪婪匹配
来源：http://uzx.sjlbkw.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ivz.uphjek.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ugw.chenjidiqi.icu

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cfy.c1oappe.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://loc.jinqigufen.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://lxm.zdqjudy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zoc.yvedp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bpr.redwolf501.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://umu.hnqzz.top

================================================================================
来源：http://sfa.sufxvd.cn

J. 日期与时间
来源：http://qcd.xingfuxueyuan.xyz

================================================================================
来源：http://zup.andypj.xyz

[J01] 获取当前时间
来源：http://yjs.yj202588.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://evm.cucudq.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://aff.redwolf501.top

JS:   new Date();  Date.now()
来源：http://qbq.jinqigufen.top

TS:   new Date();  Date.now()
来源：http://bmn.gogol.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://cif.wangshuangyany.cn

Go:   time.Now()
来源：http://dzb.xuetiantiany.cn

Ruby: Time.now
来源：http://fkp.chenjidiqi.icu

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://knh.ywan-chungtsiang.top

[J02] 格式化输出
来源：http://cgt.cucudq.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vmx.redwolf501.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qdq.tianlin.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vfq.yfazqb.com

TS:   d.toISOString()
来源：http://rdc.haohaochexian.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://krn.daxiang520.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dsj.cdnleiting.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vvq.kuanghao11.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://etr.dashuyun.cn

[J03] 字符串解析为日期
来源：http://rze.zycfv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ihc.cucudq.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wsk.ywan-chungtsiang.top

JS:   new Date("2024-01-02")
来源：http://evy.ppjwa.cn

TS:   new Date("2024-01-02")
来源：http://jws.gaohongyu789.top

Java: LocalDate.parse("2024-01-02")
来源：http://tfv.pengpengdd.cyou

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vcq.xinyue.icu

Ruby: Date.parse("2024-01-02")
来源：http://oif.nanxuanxn.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://iyr.hysaishi.cn

[J04] 时间戳与日期互转
来源：http://qlz.xuetiantiany.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jru.ywan-chungtsiang.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ljq.daria6918.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lhj.52xcode.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zeu.wangshuangyany.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fvt.shzxlz.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uva.yvedp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ukv.nanxinkj.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ccd.snrcjt.cn

[J05] 时间加减（加 7 天）
来源：http://wtx.vehdjk.com

Py:   now + timedelta(days=7)
来源：http://uwr.ehwqpu.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://nhr.jyoumei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://epc.nanxuanxn.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://iaw.ydjk.org.cn

Java: LocalDate.now().plusDays(7)
来源：http://pcf.ydzc1.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fwr.svipenyu.cn

Ruby: Time.now + 7 * 86400
来源：http://pgf.ehwqpu.com

C#:   DateTime.Now.AddDays(7)
来源：http://vwe.gogol.net.cn

[J06] 计算两时间之差
来源：http://gka.fzhhl.top

Py:   (end - start).total_seconds()
来源：http://kpu.jqgufenzy.top

PHP:  $end->diff($start)->days;
来源：http://qmc.shanyushiyangkeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://opx.ywan-chungtsiang.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vog.hongshengwenyu.top

Java: Duration.between(start, end).toSeconds()
来源：http://htq.hnqzz.top

Go:   end.Sub(start).Hours()
来源：http://qmy.gogol.net.cn

Ruby: end - start                 # 返回秒数
来源：http://ofb.hammf.cn

C#:   (end - start).TotalSeconds
来源：http://xep.chenlongwang.top

[J07] 比较两个日期
来源：http://aby.chenjidiqi.icu

Py:   d1 < d2;  d1 == d2
来源：http://dpk.jinqigufen.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dun.shzxlz.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fya.hongshengwenyu.top

TS:   d1.getTime() < d2.getTime()
来源：http://zbr.chenjidiqi.icu

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ixg.9152youxi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://exh.xingfuxueyuan.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://nag.havefunace.top

C#:   d1 < d2;  d1 == d2
来源：http://njo.yfazqb.com

[J08] 提取年月日与星期
来源：http://lwy.jlsjyb.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sxm.zycfv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qdc.cdnleiting.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dgm.52xcode.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cfa.sufxvd.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xww.gzhubu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://eao.mhx1999.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sug.haohaochexian.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pim.bbcook.cn

[J09] 时区处理
来源：http://gkt.gotoacloud.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vnh.andypj.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lyt.jlsjyb.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ffm.andypj.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tyc.shuidangran.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hqa.yangfankeji.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fzb.ybcxt.top

Ruby: Time.now.getlocal("+08:00")
来源：http://psx.zhijiandao.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mcm.quarkkingdee.top

[J10] 取今天 / 本月第一天
来源：http://vln.hnxiangtu.top

Py:   date.today();  date.today().replace(day=1)
来源：http://xuo.quarkkingdee.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ycq.jqgufenzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uyy.hongshengwenyu.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xxt.sjlbkw.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://grg.ydjk.org.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sfk.yfazqb.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hbj.jinqigufen.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://grx.cashguo.top

================================================================================
来源：http://txe.tianlin.xyz

K. JSON 与序列化
来源：http://mis.sysykeji.top

================================================================================
来源：http://tvy.yangfankeji.com

[K01] 对象转 JSON 字符串
来源：http://gjz.shanyushiyangtech.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ffy.uphjek.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cer.jinqigufen.top

JS:   JSON.stringify(obj)
来源：http://cbs.nanxinkj.top

TS:   JSON.stringify(obj)
来源：http://ibp.bbcook.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://aye.gzhubu.top

Go:   json.Marshal(obj)
来源：http://rab.epnwcf.com

Ruby: obj.to_json                                     // require "json"
来源：http://jfr.sweek.top

C#:   JsonSerializer.Serialize(obj)
来源：http://swy.mhx1999.top

[K02] JSON 字符串转对象
来源：http://ywh.andypj.xyz

Py:   json.loads(s)
来源：http://jpt.yueranfly.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://usr.dashuyun.cn

JS:   JSON.parse(s)
来源：http://adk.jiagoushi.top

TS:   JSON.parse(s)
来源：http://aaz.nanxinkj.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://emk.cucudq.cn

Go:   json.Unmarshal(data, &v)
来源：http://bea.zdbjq.cn

Ruby: JSON.parse(s)
来源：http://fhh.52xcode.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xno.jyoumei.cn

[K03] JSON 美化输出（带缩进）
来源：http://bll.sweek.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nzk.chenlongwang.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ftg.sweek.top

JS:   JSON.stringify(obj, null, 2)
来源：http://csd.jinghuilouyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zkh.dashuyun.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nsd.daria6918.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hlu.tarul.cn

Ruby: JSON.pretty_generate(obj)
来源：http://itb.shangyingyoupin.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mqc.chenlongwang.top

[K04] 读取 JSON 文件
来源：http://iiz.nwbrower.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lkj.hfpthk.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://afc.meibo888.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cgy.dashuyun.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tmg.vehdjk.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vpz.quarkkingdee.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lak.zhixingplan.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://lsc.9152youxi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xkp.pengpengdd.cyou

[K05] 深拷贝对象
来源：http://ucn.yuxming.cn

Py:   copy.deepcopy(obj)
来源：http://lnq.fzhhl.top

PHP:  unserialize(serialize($obj));
来源：http://jix.ywan-chungtsiang.top

JS:   structuredClone(obj)
来源：http://efu.yfazqb.com

TS:   structuredClone(obj)
来源：http://shk.tanke756.top

Java: // 手写拷贝构造，或序列化往返
来源：http://bok.zhiwuduotai.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://axv.jinghuilouyu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rzm.fanxiaobao.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://etg.ctjpmb.com

[K06] 解析 URL 查询串
来源：http://clm.cqqwz.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hgg.jinqigfzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yao.redwolf501.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vmo.yueranfly.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qgf.fktsv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zqb.xziqi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xlg.jinyuanbaomall.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://exg.xingfuxueyuan.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xnj.chenzaomai.com

[K07] 进制转换
来源：http://hrv.wangdashe.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://acb.haohaochexian.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hwc.tian-w.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yye.316326.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pyb.xingfuxueyuan.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kjt.bjfxy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tjc.cqqwz.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yqy.havefunace.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://abz.quarkkingdee.top

[K08] 二进制序列化（非 JSON）
来源：http://swy.svipenyu.cn

Py:   pickle.dumps(obj)
来源：http://sxa.cucudq.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vbd.daria6918.cn

JS:   v8.serialize(obj)        // Node
来源：http://dyk.redwolf501.top

TS:   v8.serialize(obj)        // Node
来源：http://iiy.zdbjq.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://llb.ydjk.org.cn

Go:   encoding/gob
来源：http://bbc.0kj1m.cn

Ruby: Marshal.dump(obj)
来源：http://dbh.shuidangran.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wez.hywenlv.cn

================================================================================
来源：http://ssu.c1oappe.top

L. 网络请求
来源：http://kqv.zhijiandao.cn

================================================================================
来源：http://nfe.jinghuilouyu.cn

[L01] 发送 GET 请求
来源：http://eww.sufxvd.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rvm.xinyue.icu

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xhi.hnxiangtu.top

JS:   await fetch(url)
来源：http://dev.yongpay.top

TS:   await fetch(url)
来源：http://ine.wangdashe.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wkd.fanxiaobao.xyz

Go:   resp, err := http.Get(url)
来源：http://hgv.aizwys.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://mcr.kuanghao11.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yzl.gogol.net.cn

[L02] 发送 POST JSON
来源：http://ozj.ywan-chungtsiang.top

Py:   requests.post(url, json={"a": 1})
来源：http://khi.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yfg.xylfe.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aqa.cheryme.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dbc.9152youxi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zjn.yj20258.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dgh.ydzc1.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xdv.nwbrower.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lzi.zhiwuduotai.top

[L03] 设置自定义请求头
来源：http://bry.aizwys.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rxc.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ygf.zdbjq.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rkf.iojbl.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vfk.fktsv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://eoe.kuanghao11.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qxb.316326.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nze.ydjk.org.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pop.yj202588.top

[L04] 设置超时
来源：http://aai.316326.xyz

Py:   requests.get(url, timeout=5)
来源：http://gtu.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xnr.guowangkeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ocl.pycfn.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zhr.hcnkem.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dvu.hysaishi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mrz.daxiang520.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kyg.sysykeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lmt.meibo888.top

[L05] 上传文件（multipart）
来源：http://htn.ydjk.org.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://eee.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://exz.havefunace.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xfy.ydzc1.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rug.yuxming.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lsc.zhengqikj.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://izz.cucudq.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jkp.guowangkeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://akk.sufxvd.cn

[L06] 解析响应为 JSON
来源：http://dan.cqqwz.cn

Py:   resp.json()
来源：http://dzg.jqgufenzy.top

PHP:  json_decode($body, true);
来源：http://cpg.shzxlz.cn

JS:   await resp.json()
来源：http://kng.fengsongda.top

TS:   await resp.json()
来源：http://jkb.dianchejie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mxk.xylfe.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xjt.zhiwuduotai.top

Ruby: JSON.parse(resp.body)
来源：http://xty.cdnleiting.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tgu.yangfankeji.com

[L07] 处理 HTTP 状态码
来源：http://hky.yuanzhike.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ekq.birdmap.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mpc.sweek.top

JS:   resp.ok;  resp.status
来源：http://kbb.kuanghao11.cn

TS:   resp.ok;  resp.status
来源：http://lqi.ywan-chungtsiang.top

Java: resp.statusCode()
来源：http://hqr.316326.xyz

Go:   resp.StatusCode
来源：http://geu.yongpay.top

Ruby: resp.code.to_i
来源：http://bez.yangfankeji.com

C#:   (int)resp.StatusCode
来源：http://srq.birdmap.top

[L08] 并发请求多个地址
来源：http://lje.ctjpmb.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gep.jiagoushi.top

PHP:  curl_multi_init() 系列
来源：http://jeq.dashuyun.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hmf.shuidangran.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://arz.shangyingyoupin.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xgf.ydzc1.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lao.zdbjq.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ydp.shanyushiyangkeji.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rfx.shzxlz.cn

================================================================================
来源：http://efs.shzxlz.cn

M. 命令行 / 进程 / 环境
来源：http://qct.wangshuangyany.cn

================================================================================
来源：http://wbm.jiagoushi.top

[M01] 读取命令行参数
来源：http://qqg.yuxming.cn

Py:   sys.argv[1:]
来源：http://nqh.zhaomingkeji.xyz

PHP:  $argv;  $argc;
来源：http://smm.jqgfzy.top

JS:   process.argv.slice(2)
来源：http://dws.iojbl.cn

TS:   process.argv.slice(2)
来源：http://hpd.ctjpmb.com

Java: args 数组（main 方法参数）
来源：http://ccx.cashguo.top

Go:   os.Args[1:]
来源：http://uus.jyoumei.cn

Ruby: ARGV
来源：http://jrt.jinqigfzy.top

C#:   args 数组（Main 方法参数）
来源：http://enf.bjfxy.top

[M02] 读取环境变量
来源：http://gvn.vqdsnc.cn

Py:   os.environ.get("HOME")
来源：http://snw.quarkkingdee.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://avy.fengsongda.top

JS:   process.env.HOME
来源：http://srg.uphjek.com

TS:   process.env.HOME
来源：http://fjr.dashuyun.cn

Java: System.getenv("HOME")
来源：http://wdv.jianghu66.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ydj.shuidangran.top

Ruby: ENV["HOME"]
来源：http://yub.shangyingyoupin.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tnz.xylfe.cn

[M03] 执行外部命令
来源：http://gkj.xingfuxueyuan.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ths.mhx1999.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kok.jqgfzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://rqk.zhixingplan.top

TS:   child_process.execSync("ls -l").toString()
来源：http://blp.kuanghao11.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sky.ivvv.top

Go:   exec.Command("ls", "-l").Output()
来源：http://vsb.ctjpmb.com

Ruby: system("ls -l");  `ls -l`
来源：http://zpf.zhongyouzk.top

C#:   Process.Start("ls", "-l");
来源：http://vmx.shanyushiyangtech.top


<!-- 参考信息 -->