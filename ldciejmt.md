代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://eks.vqdsnc.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ueg.guannengcc.top

TS:   s.replace(/\d+/g, "#")
来源：http://eln.sweek.top

Java: s.replaceAll("\\d+", "#")
来源：http://zgk.feifeiyinyue.top

Go:   re.ReplaceAllString(s, "#")
来源：http://eqf.hcnkem.com

Ruby: s.gsub(/\d+/, "#")
来源：http://ltr.svipenyu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ynh.xylfe.cn

[I05] 按正则拆分
来源：http://nxr.yj202588.top

Py:   re.split(r"\s*,\s*", s)
来源：http://zhs.svipenyu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nbw.yueranfly.top

JS:   s.split(/\s*,\s*/)
来源：http://vgr.9152youxi.cn

TS:   s.split(/\s*,\s*/)
来源：http://vox.xuetiantiany.cn

Java: s.split("\\s*,\\s*")
来源：http://ywz.guowangkeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nap.iojbl.cn

Ruby: s.split(/\s*,\s*/)
来源：http://azf.jiagoushi.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xcn.cashguo.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pkw.bbcook.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vhv.jqgufenzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hvr.andypj.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vru.yanxiufei.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cxr.gzhubu.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wrd.tanke756.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mxc.xinyue.icu

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gwo.uphjek.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kmh.fktsv.cn

[I07] 忽略大小写与多行模式
来源：http://xpr.chenzaomai.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://atb.9152youxi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xzh.dashuyun.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jma.nwbrower.top

TS:   /error/gim
来源：http://qrw.yvedp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pby.yueranfly.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wnz.yuxming.cn

Ruby: s.scan(/error/i)
来源：http://uuc.fengsongda.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kvj.ywan-chungtsiang.top

[I08] 贪婪与非贪婪匹配
来源：http://ekq.gogol.net.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fkd.xylfe.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jaf.iojbl.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://erk.nanxinkj.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bej.fengsongda.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://zdg.nanxinkj.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ecy.jinyuanbaomall.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pri.daria6918.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qrw.wangdashe.top

================================================================================
来源：http://jsz.hcnkem.com

J. 日期与时间
来源：http://yzl.cdnleiting.top

================================================================================
来源：http://cko.gogol.net.cn

[J01] 获取当前时间
来源：http://rzz.zhongyouzk.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://nbd.zhaomingkeji.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mxw.hywenlv.cn

JS:   new Date();  Date.now()
来源：http://ufn.shzxlz.cn

TS:   new Date();  Date.now()
来源：http://ifp.jianghu66.top

Java: LocalDateTime.now();  Instant.now()
来源：http://pbd.gaohongyu789.top

Go:   time.Now()
来源：http://jcl.shuidangran.top

Ruby: Time.now
来源：http://bho.wangdashe.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://thl.epnwcf.com

[J02] 格式化输出
来源：http://wdp.gaohongyu789.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://azr.xziqi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bzi.tian-w.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jow.nanxinkj.top

TS:   d.toISOString()
来源：http://dgk.ehwqpu.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pkp.jlsjyb.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://btv.birdmap.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://amj.fehbvm.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://amm.wangdashe.top

[J03] 字符串解析为日期
来源：http://qhy.c1oappe.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ovv.jianghu66.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dgt.kuanghao11.cn

JS:   new Date("2024-01-02")
来源：http://myo.nwbrower.top

TS:   new Date("2024-01-02")
来源：http://vjo.xuetiantiany.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fxx.jinqigufen.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pmh.yj202588.top

Ruby: Date.parse("2024-01-02")
来源：http://qpp.kuanghao11.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://soh.fzhhl.top

[J04] 时间戳与日期互转
来源：http://hdp.chenlongwang.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gix.jlsjyb.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://drb.fktsv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lta.sufxvd.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cfp.ehwqpu.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dzc.9152youxi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hxj.pengpengdd.cyou

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lhm.zhiwuduotai.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://aav.uphjek.com

[J05] 时间加减（加 7 天）
来源：http://xic.zdqjudy.top

Py:   now + timedelta(days=7)
来源：http://twp.zhoulong.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://xgw.fktsv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hwa.yuanzhike.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fej.52xcode.cn

Java: LocalDate.now().plusDays(7)
来源：http://dps.yj20258888.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dpp.shanyushiyangkeji.top

Ruby: Time.now + 7 * 86400
来源：http://lkh.52xcode.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lya.hfpthk.cn

[J06] 计算两时间之差
来源：http://agg.sxryk.cn

Py:   (end - start).total_seconds()
来源：http://gzz.guowangkeji.top

PHP:  $end->diff($start)->days;
来源：http://dfq.sxryk.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://eud.fengsongda.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bop.shanyushiyangtech.top

Java: Duration.between(start, end).toSeconds()
来源：http://xud.yongpay.top

Go:   end.Sub(start).Hours()
来源：http://pms.andypj.xyz

Ruby: end - start                 # 返回秒数
来源：http://avx.epnwcf.com

C#:   (end - start).TotalSeconds
来源：http://dkp.cqqwz.cn

[J07] 比较两个日期
来源：http://ptn.hfpthk.cn

Py:   d1 < d2;  d1 == d2
来源：http://qjp.dianchejie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kaj.zhengqikj.top

JS:   d1.getTime() < d2.getTime()
来源：http://kkc.ywan-chungtsiang.top

TS:   d1.getTime() < d2.getTime()
来源：http://zjx.bbcook.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pdj.uphjek.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zxb.xziqi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vsb.vehdjk.com

C#:   d1 < d2;  d1 == d2
来源：http://mdz.mhx1999.top

[J08] 提取年月日与星期
来源：http://jky.yj20258888.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://prs.dashuyun.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sxk.sufxvd.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vit.xuetiantiany.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://phq.zhiwuduotai.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gyw.fktsv.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jrr.xuanzx.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ekm.cashguo.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vxz.shanyushiyangkeji.top

[J09] 时区处理
来源：http://izr.yanxiufei.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gve.ehwqpu.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tpv.xuanzx.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sqn.yuxming.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dsp.hysaishi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pml.ywan-chungtsiang.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://eow.hongshengwenyu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://wau.nanxuanxn.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hna.kuanghao11.cn

[J10] 取今天 / 本月第一天
来源：http://knc.meibo888.top

Py:   date.today();  date.today().replace(day=1)
来源：http://gub.hnxiangtu.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://itc.sysykeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://isl.gogol.net.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mut.zhoulong.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wwm.yanxiufei.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ixs.sjlbkw.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vsy.yonumen.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ixr.fengsongda.top

================================================================================
来源：http://jmt.pycfn.com

K. JSON 与序列化
来源：http://knv.tianlin.xyz

================================================================================
来源：http://mfi.meibo888.top

[K01] 对象转 JSON 字符串
来源：http://ucl.hnqzz.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pfy.nwbrower.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://laz.uphjek.com

JS:   JSON.stringify(obj)
来源：http://yqj.sjlbkw.cn

TS:   JSON.stringify(obj)
来源：http://xob.guannengcc.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ybv.yfazqb.com

Go:   json.Marshal(obj)
来源：http://mvg.pycfn.com

Ruby: obj.to_json                                     // require "json"
来源：http://gvn.gogol.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://eaa.gaohongyu789.top

[K02] JSON 字符串转对象
来源：http://pec.cheryme.top

Py:   json.loads(s)
来源：http://inz.52xcode.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lde.sxryk.cn

JS:   JSON.parse(s)
来源：http://ram.jinqigufen.top

TS:   JSON.parse(s)
来源：http://hgo.smart0.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://aup.jinyuanbaomall.cn

Go:   json.Unmarshal(data, &v)
来源：http://ojx.ppjwa.cn

Ruby: JSON.parse(s)
来源：http://qzx.0kj1m.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ewf.svipenyu.cn

[K03] JSON 美化输出（带缩进）
来源：http://swr.cucudq.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ikm.fengsongda.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rpi.yueranfly.top

JS:   JSON.stringify(obj, null, 2)
来源：http://wjh.xingfuxueyuan.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://eec.shanyushiyangtech.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ycy.chenjidiqi.icu

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qxu.hongshengwenyu.top

Ruby: JSON.pretty_generate(obj)
来源：http://xpg.jianghu66.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dhz.vqdsnc.cn

[K04] 读取 JSON 文件
来源：http://hnb.ydjk.org.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hmd.guowangkeji.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xrh.iojbl.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yqk.daxiang520.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xnt.yongpay.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vpx.hammf.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mqr.zdqjudy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://fnd.havefunace.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://set.yj20258.top

[K05] 深拷贝对象
来源：http://qei.ivvv.top

Py:   copy.deepcopy(obj)
来源：http://kaq.xziqi.cn

PHP:  unserialize(serialize($obj));
来源：http://eem.cashguo.top

JS:   structuredClone(obj)
来源：http://cpp.birdmap.top

TS:   structuredClone(obj)
来源：http://rdn.zhongyouzk.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ccc.xingfuxueyuan.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sya.dianchejie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ver.jinyuanbaomall.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://eto.cucudq.cn

[K06] 解析 URL 查询串
来源：http://xem.zhiwuduotai.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qos.dashuyun.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://iha.0kj1m.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://srh.hcnkem.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://izi.ppjwa.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hzi.chenzaomai.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://aki.shangyingyoupin.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cef.shanyushiyangkeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ywp.guannengcc.top

[K07] 进制转换
来源：http://odr.svipenyu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wxe.cdnleiting.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dcj.hesvh.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hvm.shangyingyoupin.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xen.quarkkingdee.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dcc.zycfv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wtq.yanxiufei.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qne.epnwcf.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xbj.xuanzx.com

[K08] 二进制序列化（非 JSON）
来源：http://via.ivvv.top

Py:   pickle.dumps(obj)
来源：http://xvb.zycfv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ojf.zdbjq.cn

JS:   v8.serialize(obj)        // Node
来源：http://ejp.yj20258.top

TS:   v8.serialize(obj)        // Node
来源：http://qjd.jqgfzy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ual.xuanzx.com

Go:   encoding/gob
来源：http://ytu.shanyushiyangtech.top

Ruby: Marshal.dump(obj)
来源：http://etq.sysykeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hsk.yuanzhike.top

================================================================================
来源：http://dee.xingfuxueyuan.xyz

L. 网络请求
来源：http://khd.iojbl.cn

================================================================================
来源：http://hqo.aibaodan.cn

[L01] 发送 GET 请求
来源：http://sgg.jyoumei.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zkr.andypj.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://grr.birdmap.top

JS:   await fetch(url)
来源：http://fxn.ywan-chungtsiang.top

TS:   await fetch(url)
来源：http://myf.shangyingyoupin.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uqu.hnqzz.top

Go:   resp, err := http.Get(url)
来源：http://xcz.zhoulong.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://hqv.yj20258888.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kay.iojbl.cn

[L02] 发送 POST JSON
来源：http://ggg.cqqwz.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mii.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://czb.hongshengwenyu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vij.birdmap.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oml.chenjidiqi.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://eky.meibo888.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://drs.zhiwuduotai.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hmk.ydzc1.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://eec.xuetiantiany.cn

[L03] 设置自定义请求头
来源：http://zwz.shuidangran.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hym.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nxr.hammf.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dla.ctjpmb.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nax.zhengqikj.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lid.gzhubu.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uex.shangyingyoupin.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zvm.fanxiaobao.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uks.yvedp.cn

[L04] 设置超时
来源：http://ker.jqgfzy.top

Py:   requests.get(url, timeout=5)
来源：http://lry.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://eyg.redwolf501.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://idv.shangyingyoupin.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eaw.tian-w.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qrv.sweek.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ngc.yuanzhike.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://smd.sweek.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gcf.iojbl.cn

[L05] 上传文件（multipart）
来源：http://gcj.ywan-chungtsiang.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vws.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kyi.zhaomingkeji.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mky.dianchejie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kji.ydjk.org.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nti.zhijiandao.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dtt.yueranfly.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://stk.xziqi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pkr.xingfuxueyuan.xyz

[L06] 解析响应为 JSON
来源：http://qkp.quarkkingdee.top

Py:   resp.json()
来源：http://liw.hfpthk.cn

PHP:  json_decode($body, true);
来源：http://seq.zycfv.cn

JS:   await resp.json()
来源：http://tbf.jiagoushi.top

TS:   await resp.json()
来源：http://vgp.fzhhl.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tqw.9152youxi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://omk.iojbl.cn

Ruby: JSON.parse(resp.body)
来源：http://ghx.vehdjk.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fxa.daria6918.cn

[L07] 处理 HTTP 状态码
来源：http://zgm.epnwcf.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jzj.yanxiufei.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vvj.yfazqb.com

JS:   resp.ok;  resp.status
来源：http://qpo.aibaodan.cn

TS:   resp.ok;  resp.status
来源：http://wya.tarul.cn

Java: resp.statusCode()
来源：http://wok.feifeiyinyue.top

Go:   resp.StatusCode
来源：http://ukg.xziqi.cn

Ruby: resp.code.to_i
来源：http://kvu.ydzc1.top

C#:   (int)resp.StatusCode
来源：http://mct.tian-w.cn

[L08] 并发请求多个地址
来源：http://cyd.mhx1999.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://exn.tian-w.cn

PHP:  curl_multi_init() 系列
来源：http://ouv.xuanzx.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://slt.hammf.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xhp.fktsv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mfu.shanyushiyangtech.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vhv.chenjidiqi.icu

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wbk.hywenlv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yro.zhiwuduotai.top

================================================================================
来源：http://smk.zhoulong.xyz

M. 命令行 / 进程 / 环境
来源：http://efy.yvedp.cn

================================================================================
来源：http://uvn.jinyuanbaomall.cn

[M01] 读取命令行参数
来源：http://hhd.chenlongwang.top

Py:   sys.argv[1:]
来源：http://ase.redwolf501.top

PHP:  $argv;  $argc;
来源：http://bqm.vehdjk.com

JS:   process.argv.slice(2)
来源：http://ecs.svipenyu.cn

TS:   process.argv.slice(2)
来源：http://tzr.sweek.top

Java: args 数组（main 方法参数）
来源：http://nxz.zhoulong.xyz

Go:   os.Args[1:]
来源：http://zee.zhiwuduotai.top

Ruby: ARGV
来源：http://rrc.sysykeji.top

C#:   args 数组（Main 方法参数）
来源：http://nvp.haohaochexian.top

[M02] 读取环境变量
来源：http://lza.yuanzhike.top

Py:   os.environ.get("HOME")
来源：http://qnm.jinqigufen.top


<!-- 参考信息 -->