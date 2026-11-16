代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://ivk.52xcode.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sxu.zhixingplan.top

JS:   s.split(/\s*,\s*/)
来源：http://rgk.xylfe.cn

TS:   s.split(/\s*,\s*/)
来源：http://asa.cheryme.top

Java: s.split("\\s*,\\s*")
来源：http://syg.tian-w.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bcw.zycfv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://alm.ydzc1.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yur.yonumen.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rhp.fengsongda.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://plh.ydzc1.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lid.yongpay.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tyc.feifeiyinyue.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fsv.yuanzhike.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://thv.jinyuanbaomall.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jhp.guowangkeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fwr.cqqwz.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kdq.c1oappe.top

[I07] 忽略大小写与多行模式
来源：http://smi.hnqzz.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ppc.zhoulong.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://die.chenlongwang.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pmz.mhx1999.top

TS:   /error/gim
来源：http://ety.xylfe.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yqa.hnqzz.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://olv.chenjidiqi.icu

Ruby: s.scan(/error/i)
来源：http://zku.jiagoushi.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tco.xylfe.cn

[I08] 贪婪与非贪婪匹配
来源：http://yrc.yongpay.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kxe.zdqjudy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rld.hongshengwenyu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wht.gzhubu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ctc.chenlongwang.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ujw.ehwqpu.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fss.gotoacloud.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://teb.uphjek.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uwk.zhaomingkeji.xyz

================================================================================
来源：http://jgd.hcnkem.com

J. 日期与时间
来源：http://vnp.hongshengwenyu.top

================================================================================
来源：http://xii.yonumen.top

[J01] 获取当前时间
来源：http://ojo.cheryme.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://wgy.quarkkingdee.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cvv.smart0.xyz

JS:   new Date();  Date.now()
来源：http://ybp.bjfxy.top

TS:   new Date();  Date.now()
来源：http://gpc.aibaodan.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rux.ivvv.top

Go:   time.Now()
来源：http://mws.yonumen.top

Ruby: Time.now
来源：http://xnz.cheryme.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ssg.jinghuilouyu.cn

[J02] 格式化输出
来源：http://cpx.yuxming.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jok.jqgfzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tlm.redwolf501.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xjy.xingfuxueyuan.xyz

TS:   d.toISOString()
来源：http://vnu.meibo888.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lnu.kuanghao11.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lyp.zhongyouzk.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wow.yvedp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yaz.iojbl.cn

[J03] 字符串解析为日期
来源：http://vxo.hnqzz.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gdg.c1oappe.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fdd.zhijiandao.cn

JS:   new Date("2024-01-02")
来源：http://pxh.yvedp.cn

TS:   new Date("2024-01-02")
来源：http://vwq.aibaodan.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bih.yongpay.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fmc.hesvh.cn

Ruby: Date.parse("2024-01-02")
来源：http://jyj.yueranfly.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xre.9152youxi.cn

[J04] 时间戳与日期互转
来源：http://joz.yuanzhike.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rjn.316326.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zns.ybcxt.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sie.zhaomingkeji.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://xlb.0kj1m.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pyt.gotoacloud.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://amo.sweek.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dfz.gogol.net.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ail.9152youxi.cn

[J05] 时间加减（加 7 天）
来源：http://ogp.fktsv.cn

Py:   now + timedelta(days=7)
来源：http://xyy.hysaishi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qar.birdmap.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://csf.shangyingyoupin.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gld.zhixingplan.top

Java: LocalDate.now().plusDays(7)
来源：http://otu.jqgufenzy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ljk.jinyuanbaomall.cn

Ruby: Time.now + 7 * 86400
来源：http://wvi.quarkkingdee.top

C#:   DateTime.Now.AddDays(7)
来源：http://jms.cqqwz.cn

[J06] 计算两时间之差
来源：http://exp.hammf.cn

Py:   (end - start).total_seconds()
来源：http://viz.shanyushiyangtech.top

PHP:  $end->diff($start)->days;
来源：http://fhd.0kj1m.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xfa.yj202588.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gii.yonumen.top

Java: Duration.between(start, end).toSeconds()
来源：http://rwi.fengsongda.top

Go:   end.Sub(start).Hours()
来源：http://gge.yueranfly.top

Ruby: end - start                 # 返回秒数
来源：http://pjr.sjlbkw.cn

C#:   (end - start).TotalSeconds
来源：http://apf.shanyushiyangtech.top

[J07] 比较两个日期
来源：http://dfk.jlsjyb.cn

Py:   d1 < d2;  d1 == d2
来源：http://dmt.fengsongda.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wha.xziqi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://iqq.zhixingplan.top

TS:   d1.getTime() < d2.getTime()
来源：http://ipd.epnwcf.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bzt.xinyue.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vxd.haohaochexian.top

Ruby: d1 < d2;  d1 == d2
来源：http://pyj.shanyushiyangtech.top

C#:   d1 < d2;  d1 == d2
来源：http://pqq.yonumen.top

[J08] 提取年月日与星期
来源：http://oll.jqgufenzy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://upw.ydjk.org.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vsx.nanxuanxn.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lkc.cdnleiting.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ihu.yj202588.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ovq.dianchejie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zvi.bjfxy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xyx.ctjpmb.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lsl.xingfuxueyuan.xyz

[J09] 时区处理
来源：http://zae.jlsjyb.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fko.shanyushiyangtech.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fam.aibaodan.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ebi.zhengqikj.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ixe.yueranfly.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vvr.vehdjk.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lsx.yj20258.top

Ruby: Time.now.getlocal("+08:00")
来源：http://nfy.jianghu66.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uaf.havefunace.top

[J10] 取今天 / 本月第一天
来源：http://mhh.zycfv.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zua.c1oappe.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cvc.ivvv.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pil.yongpay.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qal.xinyue.icu

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qwx.bjfxy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cci.chenlongwang.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://knr.zdbjq.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cnt.zhaomingkeji.xyz

================================================================================
来源：http://eoy.shuidangran.top

K. JSON 与序列化
来源：http://iyl.zycfv.cn

================================================================================
来源：http://qeg.chenzaomai.com

[K01] 对象转 JSON 字符串
来源：http://rjm.jinqigufen.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wgn.shanyushiyangtech.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ruu.jinghuilouyu.cn

JS:   JSON.stringify(obj)
来源：http://hbe.52xcode.cn

TS:   JSON.stringify(obj)
来源：http://dgn.yuanzhike.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wvz.cucudq.cn

Go:   json.Marshal(obj)
来源：http://fnq.feifeiyinyue.top

Ruby: obj.to_json                                     // require "json"
来源：http://kfz.fanxiaobao.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://dtr.hnqzz.top

[K02] JSON 字符串转对象
来源：http://ctx.sufxvd.cn

Py:   json.loads(s)
来源：http://avw.iojbl.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ows.yuanzhike.top

JS:   JSON.parse(s)
来源：http://sbz.aizwys.cn

TS:   JSON.parse(s)
来源：http://lby.yj20258.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gtb.vehdjk.com

Go:   json.Unmarshal(data, &v)
来源：http://cyf.jyoumei.cn

Ruby: JSON.parse(s)
来源：http://ahi.dianchejie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://utj.feifeiyinyue.top

[K03] JSON 美化输出（带缩进）
来源：http://wcg.fzhhl.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kjv.wangdashe.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xnu.jinqigufen.top

JS:   JSON.stringify(obj, null, 2)
来源：http://izs.sysykeji.top

TS:   JSON.stringify(obj, null, 2)
来源：http://skq.ywan-chungtsiang.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xmz.zdbjq.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://iky.zycfv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://odh.feifeiyinyue.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tct.vqdsnc.cn

[K04] 读取 JSON 文件
来源：http://wqo.chenjidiqi.icu

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ack.haohaochexian.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dxo.dianchejie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cfp.feifeiyinyue.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://llu.bbcook.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ukf.yanxiufei.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wlu.nanxinkj.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://feu.aibaodan.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zxq.dashuyun.cn

[K05] 深拷贝对象
来源：http://yru.birdmap.top

Py:   copy.deepcopy(obj)
来源：http://err.gogol.net.cn

PHP:  unserialize(serialize($obj));
来源：http://xgj.hnqzz.top

JS:   structuredClone(obj)
来源：http://hqg.ywan-chungtsiang.top

TS:   structuredClone(obj)
来源：http://zce.sufxvd.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://asz.chenlongwang.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yij.yueranfly.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rul.yanxiufei.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lap.iojbl.cn

[K06] 解析 URL 查询串
来源：http://tze.xingfuxueyuan.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://txi.zhaomingkeji.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kph.zhongyouzk.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qah.vehdjk.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://piq.hnxiangtu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gtw.nwbrower.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://fmp.redwolf501.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ask.cdnleiting.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rrs.bjfxy.top

[K07] 进制转换
来源：http://elx.guannengcc.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dzl.aibaodan.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://odg.aibaodan.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tji.dianchejie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ylr.mhx1999.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qkm.bbcook.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qsz.iojbl.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fei.hammf.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://flr.zhengqikj.top

[K08] 二进制序列化（非 JSON）
来源：http://yel.cdnleiting.top

Py:   pickle.dumps(obj)
来源：http://unw.hysaishi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nhl.xuanzx.com

JS:   v8.serialize(obj)        // Node
来源：http://pnv.shangyingyoupin.top

TS:   v8.serialize(obj)        // Node
来源：http://jpt.vqdsnc.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sjd.yj202588.top

Go:   encoding/gob
来源：http://izd.havefunace.top

Ruby: Marshal.dump(obj)
来源：http://sjb.chenzaomai.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ctq.sufxvd.cn

================================================================================
来源：http://ahm.nanxinkj.top

L. 网络请求
来源：http://wyk.hesvh.cn

================================================================================
来源：http://hku.gotoacloud.top

[L01] 发送 GET 请求
来源：http://ati.chenzaomai.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lbe.vqdsnc.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vqd.yj20258.top

JS:   await fetch(url)
来源：http://fyg.yonumen.top

TS:   await fetch(url)
来源：http://val.zycfv.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ivg.chenjidiqi.icu

Go:   resp, err := http.Get(url)
来源：http://ooi.epnwcf.com

Ruby: Net::HTTP.get(URI(url))
来源：http://zrl.epnwcf.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mrl.sxryk.cn

[L02] 发送 POST JSON
来源：http://eci.quarkkingdee.top

Py:   requests.post(url, json={"a": 1})
来源：http://hpn.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://omv.yangfankeji.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xsx.zhengqikj.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pah.tarul.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rlh.zhixingplan.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ukl.ybcxt.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xcc.ywan-chungtsiang.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hou.yj202588.top

[L03] 设置自定义请求头
来源：http://jzx.daxiang520.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://imq.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nci.fengsongda.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ouq.yuanzhike.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://whi.shangyingyoupin.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zqj.yj20258.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fqg.wangshuangyany.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ugw.tanke756.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bmb.xylfe.cn

[L04] 设置超时
来源：http://jmx.ppjwa.cn

Py:   requests.get(url, timeout=5)
来源：http://rhq.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wmw.xziqi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rzb.shuidangran.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dwz.zhixingplan.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bjn.jqgufenzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fyc.hfpthk.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jke.ehwqpu.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mgt.nanxuanxn.top

[L05] 上传文件（multipart）
来源：http://kcf.ydjk.org.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gpt.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bhc.mhx1999.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hnu.yj20258888.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://odm.jianghu66.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pce.nanxinkj.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://oja.guannengcc.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gsk.sufxvd.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qut.ctjpmb.com

[L06] 解析响应为 JSON
来源：http://tqw.yfazqb.com

Py:   resp.json()
来源：http://bcj.zdqjudy.top

PHP:  json_decode($body, true);
来源：http://gvq.zhijiandao.cn

JS:   await resp.json()
来源：http://xbr.bjfxy.top

TS:   await resp.json()
来源：http://bxc.jinqigufen.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wel.havefunace.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cpd.yfazqb.com

Ruby: JSON.parse(resp.body)
来源：http://loa.gogol.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://olm.nanxuanxn.top

[L07] 处理 HTTP 状态码
来源：http://lac.sxryk.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pbs.sjlbkw.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nqf.jinqigufen.top

JS:   resp.ok;  resp.status
来源：http://piw.tanke756.top

TS:   resp.ok;  resp.status
来源：http://kip.ivvv.top

Java: resp.statusCode()
来源：http://oso.pengpengdd.cyou

Go:   resp.StatusCode
来源：http://oap.zhengqikj.top

Ruby: resp.code.to_i
来源：http://syp.wangdashe.top

C#:   (int)resp.StatusCode
来源：http://jmh.9152youxi.cn

[L08] 并发请求多个地址
来源：http://ovu.zhixingplan.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://arq.jinqigfzy.top

PHP:  curl_multi_init() 系列
来源：http://rjh.kuanghao11.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ahl.chenjidiqi.icu

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ipt.ivvv.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qfe.guannengcc.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bss.sjlbkw.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cjo.0kj1m.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://icb.fanxiaobao.xyz

================================================================================
来源：http://tsk.52xcode.cn

M. 命令行 / 进程 / 环境
来源：http://hen.mhx1999.top

================================================================================
来源：http://ydw.yvedp.cn

[M01] 读取命令行参数
来源：http://edd.yj20258888.top

Py:   sys.argv[1:]
来源：http://eig.quarkkingdee.top

PHP:  $argv;  $argc;
来源：http://kse.pengpengdd.cyou

JS:   process.argv.slice(2)
来源：http://kuj.shanyushiyangkeji.top

TS:   process.argv.slice(2)
来源：http://jla.chenlongwang.top

Java: args 数组（main 方法参数）
来源：http://uha.birdmap.top

Go:   os.Args[1:]
来源：http://nvz.wangshuangyany.cn

Ruby: ARGV
来源：http://pge.yj202588.top

C#:   args 数组（Main 方法参数）
来源：http://wan.dianchejie.cn

[M02] 读取环境变量
来源：http://kru.c1oappe.top

Py:   os.environ.get("HOME")
来源：http://nto.xingfuxueyuan.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pvt.dianchejie.cn

JS:   process.env.HOME
来源：http://dyz.jinqigufen.top

TS:   process.env.HOME
来源：http://pvt.guannengcc.top

Java: System.getenv("HOME")
来源：http://kdv.hfpthk.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gbp.smart0.xyz

Ruby: ENV["HOME"]
来源：http://wdw.yvedp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fwg.haohaochexian.top

[M03] 执行外部命令
来源：http://bdn.nanxuanxn.top


<!-- 参考信息 -->