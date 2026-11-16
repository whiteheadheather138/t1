代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ocz.yj20258.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lon.hcnkem.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mdy.gzhubu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aio.ppjwa.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://msw.kuanghao11.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://taf.jianghu66.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gfy.jqgufenzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ile.dianchejie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cfw.wangshuangyany.cn

[I07] 忽略大小写与多行模式
来源：http://jwo.feifeiyinyue.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hpw.gzhubu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dtm.tanke756.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zea.cucudq.cn

TS:   /error/gim
来源：http://zlc.jqgufenzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lom.guowangkeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gza.zhixingplan.top

Ruby: s.scan(/error/i)
来源：http://jlz.yueranfly.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wjs.cashguo.top

[I08] 贪婪与非贪婪匹配
来源：http://azp.jlsjyb.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://osu.fehbvm.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uik.316326.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mkx.tianlin.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lca.xziqi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ncy.chenjidiqi.icu

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ert.chenzaomai.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mve.xylfe.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://epa.hcnkem.com

================================================================================
来源：http://nqv.zycfv.cn

J. 日期与时间
来源：http://pqg.jianghu66.top

================================================================================
来源：http://mua.bjfxy.top

[J01] 获取当前时间
来源：http://luk.quarkkingdee.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://kqa.ehwqpu.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ptw.cashguo.top

JS:   new Date();  Date.now()
来源：http://qmg.ywan-chungtsiang.top

TS:   new Date();  Date.now()
来源：http://wqh.zycfv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://goq.xinyue.icu

Go:   time.Now()
来源：http://rtg.shanyushiyangtech.top

Ruby: Time.now
来源：http://pgj.pengpengdd.cyou

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gir.ywan-chungtsiang.top

[J02] 格式化输出
来源：http://hlj.9152youxi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yyj.sufxvd.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jae.aibaodan.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://woz.xingfuxueyuan.xyz

TS:   d.toISOString()
来源：http://fdl.ydjk.org.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kuo.yongpay.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jyz.fanxiaobao.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dqs.wangdashe.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nqb.aizwys.cn

[J03] 字符串解析为日期
来源：http://adq.ehwqpu.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xkx.hongshengwenyu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lil.hfpthk.cn

JS:   new Date("2024-01-02")
来源：http://wzg.daxiang520.top

TS:   new Date("2024-01-02")
来源：http://heo.bjfxy.top

Java: LocalDate.parse("2024-01-02")
来源：http://oig.pycfn.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jzg.cdnleiting.top

Ruby: Date.parse("2024-01-02")
来源：http://bsx.daria6918.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mtt.ctjpmb.com

[J04] 时间戳与日期互转
来源：http://rjt.vehdjk.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vev.fzhhl.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://syn.epnwcf.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fpi.hesvh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qry.ybcxt.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zcf.guowangkeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dbq.hysaishi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fuo.zhixingplan.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jnv.shanyushiyangkeji.top

[J05] 时间加减（加 7 天）
来源：http://sfn.hongshengwenyu.top

Py:   now + timedelta(days=7)
来源：http://rge.epnwcf.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://bgu.zdbjq.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vrx.yangfankeji.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mst.0kj1m.cn

Java: LocalDate.now().plusDays(7)
来源：http://fmi.hammf.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ott.yvedp.cn

Ruby: Time.now + 7 * 86400
来源：http://uef.ctjpmb.com

C#:   DateTime.Now.AddDays(7)
来源：http://qwg.cashguo.top

[J06] 计算两时间之差
来源：http://nqe.ywan-chungtsiang.top

Py:   (end - start).total_seconds()
来源：http://oyk.wangdashe.top

PHP:  $end->diff($start)->days;
来源：http://gwy.uphjek.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mjy.ydzc1.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xsf.jiagoushi.top

Java: Duration.between(start, end).toSeconds()
来源：http://aky.yj20258888.top

Go:   end.Sub(start).Hours()
来源：http://bez.chenjidiqi.icu

Ruby: end - start                 # 返回秒数
来源：http://yqw.havefunace.top

C#:   (end - start).TotalSeconds
来源：http://rqt.sjlbkw.cn

[J07] 比较两个日期
来源：http://hrw.hongshengwenyu.top

Py:   d1 < d2;  d1 == d2
来源：http://zcg.zdbjq.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ptt.pengpengdd.cyou

JS:   d1.getTime() < d2.getTime()
来源：http://xhf.yuxming.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ypg.xuetiantiany.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ali.shanyushiyangtech.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zyh.quarkkingdee.top

Ruby: d1 < d2;  d1 == d2
来源：http://dvb.zhixingplan.top

C#:   d1 < d2;  d1 == d2
来源：http://wnx.hysaishi.cn

[J08] 提取年月日与星期
来源：http://nyz.c1oappe.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zim.jqgufenzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://aqm.jyoumei.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://goz.chenjidiqi.icu

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xpo.fktsv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sny.daxiang520.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wix.ivvv.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mey.316326.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dij.zhijiandao.cn

[J09] 时区处理
来源：http://raa.tarul.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://eks.tianlin.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wit.quarkkingdee.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gbw.epnwcf.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ios.fehbvm.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mmw.gaohongyu789.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xwh.ivvv.top

Ruby: Time.now.getlocal("+08:00")
来源：http://zrs.cqqwz.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://aca.hysaishi.cn

[J10] 取今天 / 本月第一天
来源：http://cge.ppjwa.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rme.shanyushiyangkeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nog.jqgufenzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jts.ctjpmb.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://byk.gaohongyu789.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lfw.fzhhl.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dzu.daxiang520.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yre.hfpthk.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://eeo.ivvv.top

================================================================================
来源：http://mjo.yj20258.top

K. JSON 与序列化
来源：http://rlt.jinghuilouyu.cn

================================================================================
来源：http://yhz.zdbjq.cn

[K01] 对象转 JSON 字符串
来源：http://viq.guannengcc.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gom.chenlongwang.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jyt.yueranfly.top

JS:   JSON.stringify(obj)
来源：http://dfp.tianlin.xyz

TS:   JSON.stringify(obj)
来源：http://hlp.fanxiaobao.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zhj.cqqwz.cn

Go:   json.Marshal(obj)
来源：http://eoq.pycfn.com

Ruby: obj.to_json                                     // require "json"
来源：http://bgj.chenlongwang.top

C#:   JsonSerializer.Serialize(obj)
来源：http://sje.zhaomingkeji.xyz

[K02] JSON 字符串转对象
来源：http://lwz.fzhhl.top

Py:   json.loads(s)
来源：http://xig.ywan-chungtsiang.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zzp.sysykeji.top

JS:   JSON.parse(s)
来源：http://yfa.pengpengdd.cyou

TS:   JSON.parse(s)
来源：http://for.tian-w.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rfa.dashuyun.cn

Go:   json.Unmarshal(data, &v)
来源：http://opp.vehdjk.com

Ruby: JSON.parse(s)
来源：http://xoe.sysykeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cor.sjlbkw.cn

[K03] JSON 美化输出（带缩进）
来源：http://hoi.snrcjt.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uqo.ydzc1.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yof.tian-w.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ist.dianchejie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sqj.pengpengdd.cyou

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gqs.ppjwa.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xaw.ybcxt.top

Ruby: JSON.pretty_generate(obj)
来源：http://ppe.zhijiandao.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mge.gotoacloud.top

[K04] 读取 JSON 文件
来源：http://pej.xylfe.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lhb.sweek.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hxx.jlsjyb.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eio.yangfankeji.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xei.shanyushiyangtech.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dpy.ehwqpu.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oeq.gzhubu.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://tma.kuanghao11.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wss.yonumen.top

[K05] 深拷贝对象
来源：http://ouw.daxiang520.top

Py:   copy.deepcopy(obj)
来源：http://vta.ywan-chungtsiang.top

PHP:  unserialize(serialize($obj));
来源：http://olo.ehwqpu.com

JS:   structuredClone(obj)
来源：http://nnl.sufxvd.cn

TS:   structuredClone(obj)
来源：http://tdt.ywan-chungtsiang.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ftq.0kj1m.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wtc.bjfxy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rxf.redwolf501.top

C#:   // 序列化往返，或自定义 Clone
来源：http://uee.shanyushiyangtech.top

[K06] 解析 URL 查询串
来源：http://xwi.guowangkeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lgd.quarkkingdee.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xda.zhijiandao.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://upg.haohaochexian.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xgn.zhengqikj.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tun.cdnleiting.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jpa.hcnkem.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kio.xuanzx.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://czr.shzxlz.cn

[K07] 进制转换
来源：http://yjp.bjfxy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sgr.shuidangran.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wqp.gzhubu.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ltw.yongpay.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xbz.aibaodan.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hic.cheryme.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zco.daria6918.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://reg.yfazqb.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://olo.sjlbkw.cn

[K08] 二进制序列化（非 JSON）
来源：http://lda.xingfuxueyuan.xyz

Py:   pickle.dumps(obj)
来源：http://snl.yangfankeji.com

PHP:  serialize($obj);  unserialize($s);
来源：http://tos.yj202588.top

JS:   v8.serialize(obj)        // Node
来源：http://pkm.yongpay.top

TS:   v8.serialize(obj)        // Node
来源：http://mki.smart0.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://psh.sjlbkw.cn

Go:   encoding/gob
来源：http://asn.zhiwuduotai.top

Ruby: Marshal.dump(obj)
来源：http://rvw.zhengqikj.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uzw.nanxinkj.top

================================================================================
来源：http://yrp.gotoacloud.top

L. 网络请求
来源：http://ymz.zhengqikj.top

================================================================================
来源：http://dcr.mhx1999.top

[L01] 发送 GET 请求
来源：http://ttz.chenlongwang.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ria.hcnkem.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uhq.aizwys.cn

JS:   await fetch(url)
来源：http://pae.cdnleiting.top

TS:   await fetch(url)
来源：http://rec.sufxvd.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rjt.hnqzz.top

Go:   resp, err := http.Get(url)
来源：http://sia.hcnkem.com

Ruby: Net::HTTP.get(URI(url))
来源：http://mqc.havefunace.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hwk.yfazqb.com

[L02] 发送 POST JSON
来源：http://lsn.quarkkingdee.top

Py:   requests.post(url, json={"a": 1})
来源：http://ixv.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ous.jqgfzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://btl.kuanghao11.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bch.hfpthk.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vok.fehbvm.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gnd.bbcook.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://axq.haohaochexian.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zoc.hongshengwenyu.top

[L03] 设置自定义请求头
来源：http://dgm.gaohongyu789.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gan.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nij.fehbvm.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lpj.hcnkem.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ncl.xziqi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fzm.zhijiandao.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gec.zhengqikj.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fak.zhongyouzk.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lyx.xuetiantiany.cn

[L04] 设置超时
来源：http://snw.ivvv.top

Py:   requests.get(url, timeout=5)
来源：http://xdo.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pxl.yuanzhike.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hdj.zdqjudy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ckx.hesvh.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lhp.chenjidiqi.icu

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nef.mhx1999.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bkx.pengpengdd.cyou

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zeg.shuidangran.top

[L05] 上传文件（multipart）
来源：http://and.andypj.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dlt.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ikt.cheryme.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dhs.daxiang520.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nve.hesvh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wvx.zdqjudy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dxs.shangyingyoupin.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xcq.cdnleiting.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://clr.sufxvd.cn

[L06] 解析响应为 JSON
来源：http://krl.316326.xyz

Py:   resp.json()
来源：http://kpj.quarkkingdee.top

PHP:  json_decode($body, true);
来源：http://vhm.vehdjk.com

JS:   await resp.json()
来源：http://exm.sxryk.cn

TS:   await resp.json()
来源：http://mli.yvedp.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ptg.jqgufenzy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jjp.zhixingplan.top

Ruby: JSON.parse(resp.body)
来源：http://mpl.ppjwa.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ajr.chenlongwang.top

[L07] 处理 HTTP 状态码
来源：http://jeu.xziqi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://idw.guowangkeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fuu.chenjidiqi.icu

JS:   resp.ok;  resp.status
来源：http://cwz.havefunace.top

TS:   resp.ok;  resp.status
来源：http://yct.vqdsnc.cn

Java: resp.statusCode()
来源：http://zio.zdqjudy.top

Go:   resp.StatusCode
来源：http://zfj.zhongyouzk.top

Ruby: resp.code.to_i
来源：http://etb.xuetiantiany.cn

C#:   (int)resp.StatusCode
来源：http://tga.hywenlv.cn

[L08] 并发请求多个地址
来源：http://vfx.jinyuanbaomall.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ypo.jianghu66.top

PHP:  curl_multi_init() 系列
来源：http://ifj.jinghuilouyu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ajp.cashguo.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dat.ppjwa.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pvj.zhongyouzk.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kzf.iojbl.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yno.hfpthk.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pkv.hcnkem.com

================================================================================
来源：http://yoa.9152youxi.cn

M. 命令行 / 进程 / 环境
来源：http://asn.zhiwuduotai.top

================================================================================
来源：http://idy.sweek.top

[M01] 读取命令行参数
来源：http://gnm.jyoumei.cn

Py:   sys.argv[1:]
来源：http://snv.aibaodan.cn

PHP:  $argv;  $argc;
来源：http://rwf.jianghu66.top

JS:   process.argv.slice(2)
来源：http://wnh.zhijiandao.cn

TS:   process.argv.slice(2)
来源：http://pza.xylfe.cn

Java: args 数组（main 方法参数）
来源：http://ayp.andypj.xyz

Go:   os.Args[1:]
来源：http://pcz.aizwys.cn

Ruby: ARGV
来源：http://vxf.yangfankeji.com

C#:   args 数组（Main 方法参数）
来源：http://nyj.feifeiyinyue.top

[M02] 读取环境变量
来源：http://ykz.yuanzhike.top

Py:   os.environ.get("HOME")
来源：http://qei.cheryme.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ugo.cashguo.top

JS:   process.env.HOME
来源：http://rel.jyoumei.cn

TS:   process.env.HOME
来源：http://yqv.jinqigfzy.top

Java: System.getenv("HOME")
来源：http://nij.chenjidiqi.icu

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bzq.xziqi.cn

Ruby: ENV["HOME"]
来源：http://ktu.nanxuanxn.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xfa.cheryme.top

[M03] 执行外部命令
来源：http://cae.feifeiyinyue.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bkx.quarkkingdee.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://oxr.kuanghao11.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bbw.smart0.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://sed.hnxiangtu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://loo.ywan-chungtsiang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ydl.yj20258888.top

Ruby: system("ls -l");  `ls -l`
来源：http://hei.xziqi.cn

C#:   Process.Start("ls", "-l");
来源：http://pxx.shangyingyoupin.top


<!-- 参考信息 -->