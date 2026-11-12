代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://wen.yfazqb.com

Ruby: s.gsub(/\d+/, "#")
来源：http://tet.hcnkem.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hav.shangyingyoupin.top

[I05] 按正则拆分
来源：http://pcd.tianlin.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://mnx.sweek.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ujg.jinqigufen.top

JS:   s.split(/\s*,\s*/)
来源：http://gyx.zhiwuduotai.top

TS:   s.split(/\s*,\s*/)
来源：http://joa.nanxuanxn.top

Java: s.split("\\s*,\\s*")
来源：http://jam.fehbvm.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kbv.zdqjudy.top

Ruby: s.split(/\s*,\s*/)
来源：http://tnn.ctjpmb.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://knc.tarul.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gox.meibo888.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qle.ehwqpu.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ocw.zhengqikj.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fei.ydzc1.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://coh.bjfxy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zsz.gogol.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vnf.iojbl.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vax.gaohongyu789.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ygo.tian-w.cn

[I07] 忽略大小写与多行模式
来源：http://dpe.hysaishi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ens.316326.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jlu.pycfn.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hae.nanxinkj.top

TS:   /error/gim
来源：http://qlk.ppjwa.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hvj.fengsongda.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://clm.zdqjudy.top

Ruby: s.scan(/error/i)
来源：http://qhn.jqgfzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qtl.cashguo.top

[I08] 贪婪与非贪婪匹配
来源：http://uoh.havefunace.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tjw.sysykeji.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qvw.xylfe.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uay.fehbvm.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gti.gzhubu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://wfq.dashuyun.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hin.dianchejie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nwi.chenzaomai.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cci.chenjidiqi.icu

================================================================================
来源：http://jjy.iojbl.cn

J. 日期与时间
来源：http://mte.tian-w.cn

================================================================================
来源：http://kwu.shanyushiyangtech.top

[J01] 获取当前时间
来源：http://oxl.xylfe.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ljd.jyoumei.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rfa.fzhhl.top

JS:   new Date();  Date.now()
来源：http://idz.tianlin.xyz

TS:   new Date();  Date.now()
来源：http://ipj.bbcook.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://prl.iojbl.cn

Go:   time.Now()
来源：http://ayu.shanyushiyangkeji.top

Ruby: Time.now
来源：http://oxr.shzxlz.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lts.yvedp.cn

[J02] 格式化输出
来源：http://xks.shanyushiyangkeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pku.316326.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uyu.zhaomingkeji.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wfw.52xcode.cn

TS:   d.toISOString()
来源：http://klj.jlsjyb.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zwm.pengpengdd.cyou

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ozl.zhongyouzk.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yjl.gaohongyu789.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://khc.iojbl.cn

[J03] 字符串解析为日期
来源：http://cnx.hammf.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wqp.ctjpmb.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zle.bjfxy.top

JS:   new Date("2024-01-02")
来源：http://uvr.jyoumei.cn

TS:   new Date("2024-01-02")
来源：http://wfb.yvedp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vsw.hfpthk.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xrg.yj202588.top

Ruby: Date.parse("2024-01-02")
来源：http://hiz.bjfxy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://oxh.ppjwa.cn

[J04] 时间戳与日期互转
来源：http://far.sjlbkw.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ixl.dianchejie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lwl.sweek.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wff.daria6918.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://nud.tianlin.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gyx.sysykeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jcn.pycfn.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mun.pengpengdd.cyou

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zoz.jianghu66.top

[J05] 时间加减（加 7 天）
来源：http://pgm.gotoacloud.top

Py:   now + timedelta(days=7)
来源：http://nof.gotoacloud.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://oda.sufxvd.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pyj.jinqigfzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pup.ydjk.org.cn

Java: LocalDate.now().plusDays(7)
来源：http://pdf.yj20258.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nsk.yonumen.top

Ruby: Time.now + 7 * 86400
来源：http://xzz.zdqjudy.top

C#:   DateTime.Now.AddDays(7)
来源：http://tlj.jiagoushi.top

[J06] 计算两时间之差
来源：http://wdm.feifeiyinyue.top

Py:   (end - start).total_seconds()
来源：http://dlf.shuidangran.top

PHP:  $end->diff($start)->days;
来源：http://njc.ydjk.org.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gol.ppjwa.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lkf.birdmap.top

Java: Duration.between(start, end).toSeconds()
来源：http://pko.yfazqb.com

Go:   end.Sub(start).Hours()
来源：http://czy.dianchejie.cn

Ruby: end - start                 # 返回秒数
来源：http://qtc.daria6918.cn

C#:   (end - start).TotalSeconds
来源：http://uxm.daria6918.cn

[J07] 比较两个日期
来源：http://sdg.ydjk.org.cn

Py:   d1 < d2;  d1 == d2
来源：http://fui.sxryk.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fcm.hywenlv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ery.xingfuxueyuan.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://lem.feifeiyinyue.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vmy.daria6918.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://iat.hcnkem.com

Ruby: d1 < d2;  d1 == d2
来源：http://uhq.hnxiangtu.top

C#:   d1 < d2;  d1 == d2
来源：http://mhm.yvedp.cn

[J08] 提取年月日与星期
来源：http://rds.tarul.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wgf.xingfuxueyuan.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lag.0kj1m.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ghg.uphjek.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qli.cheryme.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fxg.xingfuxueyuan.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wlc.cdnleiting.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pog.mhx1999.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zzg.zhixingplan.top

[J09] 时区处理
来源：http://lpa.cdnleiting.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sha.hysaishi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kfv.hongshengwenyu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gco.316326.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wyn.hfpthk.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://aiy.xuetiantiany.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://czg.nanxinkj.top

Ruby: Time.now.getlocal("+08:00")
来源：http://kdi.yonumen.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jzr.cqqwz.cn

[J10] 取今天 / 本月第一天
来源：http://dmq.fanxiaobao.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://vii.xinyue.icu

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ygo.hcnkem.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rwe.yueranfly.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ssp.zhiwuduotai.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ejw.jlsjyb.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kvq.sjlbkw.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://trb.zycfv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://doi.epnwcf.com

================================================================================
来源：http://urb.cucudq.cn

K. JSON 与序列化
来源：http://xfi.yuxming.cn

================================================================================
来源：http://ehs.epnwcf.com

[K01] 对象转 JSON 字符串
来源：http://gim.fzhhl.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://agv.sxryk.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rpc.jinqigufen.top

JS:   JSON.stringify(obj)
来源：http://rgq.zhoulong.xyz

TS:   JSON.stringify(obj)
来源：http://vys.zhiwuduotai.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fbb.svipenyu.cn

Go:   json.Marshal(obj)
来源：http://slm.shanyushiyangkeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://kjx.uphjek.com

C#:   JsonSerializer.Serialize(obj)
来源：http://jwu.daria6918.cn

[K02] JSON 字符串转对象
来源：http://gif.fktsv.cn

Py:   json.loads(s)
来源：http://dae.fehbvm.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hia.hysaishi.cn

JS:   JSON.parse(s)
来源：http://lut.shuidangran.top

TS:   JSON.parse(s)
来源：http://hto.bbcook.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://shx.yvedp.cn

Go:   json.Unmarshal(data, &v)
来源：http://izl.sweek.top

Ruby: JSON.parse(s)
来源：http://fry.zhoulong.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qdh.ywan-chungtsiang.top

[K03] JSON 美化输出（带缩进）
来源：http://cep.epnwcf.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ypu.ppjwa.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://giu.jlsjyb.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vcy.ywan-chungtsiang.top

TS:   JSON.stringify(obj, null, 2)
来源：http://fuj.gaohongyu789.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cbb.zhijiandao.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bhp.yuanzhike.top

Ruby: JSON.pretty_generate(obj)
来源：http://zqp.jianghu66.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cla.hfpthk.cn

[K04] 读取 JSON 文件
来源：http://mal.jinqigufen.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jwc.chenzaomai.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sgr.zhengqikj.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yer.ehwqpu.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qwn.guowangkeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://chw.shangyingyoupin.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://flf.smart0.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://voh.feifeiyinyue.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://grd.tarul.cn

[K05] 深拷贝对象
来源：http://mvu.birdmap.top

Py:   copy.deepcopy(obj)
来源：http://wly.yfazqb.com

PHP:  unserialize(serialize($obj));
来源：http://fzt.kuanghao11.cn

JS:   structuredClone(obj)
来源：http://vem.fzhhl.top

TS:   structuredClone(obj)
来源：http://ulc.316326.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://uly.ydjk.org.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kaa.gaohongyu789.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gyi.hfpthk.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://arc.haohaochexian.top

[K06] 解析 URL 查询串
来源：http://fdw.yj20258888.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oau.shzxlz.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kfh.zdqjudy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fon.ybcxt.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rkx.guannengcc.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uxe.zdqjudy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://zzj.52xcode.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nzn.hnxiangtu.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yus.ydzc1.top

[K07] 进制转换
来源：http://cru.birdmap.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bxo.xziqi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lji.feifeiyinyue.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pic.pycfn.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qot.birdmap.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tcm.guannengcc.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yrz.jinqigufen.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qvc.ybcxt.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lto.pycfn.com

[K08] 二进制序列化（非 JSON）
来源：http://apu.ppjwa.cn

Py:   pickle.dumps(obj)
来源：http://ecn.hongshengwenyu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://zzv.gzhubu.top

JS:   v8.serialize(obj)        // Node
来源：http://sqo.tarul.cn

TS:   v8.serialize(obj)        // Node
来源：http://cxz.jianghu66.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://grh.zhaomingkeji.xyz

Go:   encoding/gob
来源：http://ctd.ywan-chungtsiang.top

Ruby: Marshal.dump(obj)
来源：http://hog.shuidangran.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sev.andypj.xyz

================================================================================
来源：http://qfp.zhaomingkeji.xyz

L. 网络请求
来源：http://ert.ydzc1.top

================================================================================
来源：http://dbb.zhiwuduotai.top

[L01] 发送 GET 请求
来源：http://hcu.yueranfly.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vcd.yangfankeji.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dbg.gotoacloud.top

JS:   await fetch(url)
来源：http://yix.hnqzz.top

TS:   await fetch(url)
来源：http://tkm.jiagoushi.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fro.xinyue.icu

Go:   resp, err := http.Get(url)
来源：http://mxy.zhongyouzk.top

Ruby: Net::HTTP.get(URI(url))
来源：http://xtq.yonumen.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://aao.jyoumei.cn

[L02] 发送 POST JSON
来源：http://ifu.xziqi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://aee.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mnc.xuanzx.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dpp.hnqzz.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kyi.hesvh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vfw.jinqigufen.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vpw.hesvh.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pct.aizwys.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vjy.hnqzz.top

[L03] 设置自定义请求头
来源：http://poz.dianchejie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ajp.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uvt.yfazqb.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bch.hnxiangtu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://abp.yj20258.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cus.dashuyun.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://giz.gotoacloud.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cbi.ppjwa.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://olo.316326.xyz

[L04] 设置超时
来源：http://zjg.birdmap.top

Py:   requests.get(url, timeout=5)
来源：http://mur.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ipt.jiagoushi.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rin.hammf.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zxa.daxiang520.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yuw.0kj1m.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://svs.haohaochexian.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ufd.xingfuxueyuan.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ujy.shanyushiyangtech.top

[L05] 上传文件（multipart）
来源：http://uwu.cashguo.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uyr.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jhk.jinqigufen.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kpt.quarkkingdee.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cci.nanxuanxn.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bic.yongpay.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://iit.cucudq.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xay.yonumen.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wau.vehdjk.com

[L06] 解析响应为 JSON
来源：http://xlu.sjlbkw.cn

Py:   resp.json()
来源：http://seu.uphjek.com

PHP:  json_decode($body, true);
来源：http://bjy.nanxuanxn.top

JS:   await resp.json()
来源：http://bpv.fengsongda.top

TS:   await resp.json()
来源：http://aqg.tian-w.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hvj.xuanzx.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mls.hfpthk.cn

Ruby: JSON.parse(resp.body)
来源：http://rba.jiagoushi.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qxa.cheryme.top

[L07] 处理 HTTP 状态码
来源：http://kcv.fanxiaobao.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://daa.ehwqpu.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wru.gaohongyu789.top

JS:   resp.ok;  resp.status
来源：http://whs.jqgufenzy.top

TS:   resp.ok;  resp.status
来源：http://ski.daxiang520.top

Java: resp.statusCode()
来源：http://usr.yongpay.top

Go:   resp.StatusCode
来源：http://btp.zdqjudy.top

Ruby: resp.code.to_i
来源：http://yon.zycfv.cn

C#:   (int)resp.StatusCode
来源：http://rpg.0kj1m.cn

[L08] 并发请求多个地址
来源：http://stp.zdbjq.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://erj.cdnleiting.top

PHP:  curl_multi_init() 系列
来源：http://aaz.xinyue.icu

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ckx.daxiang520.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gtx.zhongyouzk.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xbj.gaohongyu789.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qjc.yongpay.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ifd.52xcode.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mak.aizwys.cn

================================================================================
来源：http://hlg.yj202588.top

M. 命令行 / 进程 / 环境
来源：http://egr.zdqjudy.top

================================================================================
来源：http://dcy.cdnleiting.top

[M01] 读取命令行参数
来源：http://tok.bjfxy.top

Py:   sys.argv[1:]
来源：http://fyn.jinyuanbaomall.cn

PHP:  $argv;  $argc;
来源：http://bth.daxiang520.top

JS:   process.argv.slice(2)
来源：http://kid.hywenlv.cn

TS:   process.argv.slice(2)
来源：http://zsb.sjlbkw.cn

Java: args 数组（main 方法参数）
来源：http://msl.tian-w.cn

Go:   os.Args[1:]
来源：http://lmr.yvedp.cn

Ruby: ARGV
来源：http://kkn.yangfankeji.com

C#:   args 数组（Main 方法参数）
来源：http://izw.haohaochexian.top

[M02] 读取环境变量
来源：http://ccy.vehdjk.com

Py:   os.environ.get("HOME")
来源：http://ykc.epnwcf.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pvd.uphjek.com

JS:   process.env.HOME
来源：http://gal.mhx1999.top

TS:   process.env.HOME
来源：http://trj.yueranfly.top

Java: System.getenv("HOME")
来源：http://qhs.ywan-chungtsiang.top


<!-- 参考信息 -->