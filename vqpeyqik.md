代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jzz.nanxuanxn.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kaa.zdqjudy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bjh.tian-w.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rnb.yj202588.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nfe.chenlongwang.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cpo.gotoacloud.top

[I04] 正则替换
来源：http://fbl.sxryk.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://nzg.xuetiantiany.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kvp.guowangkeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://kby.feifeiyinyue.top

TS:   s.replace(/\d+/g, "#")
来源：http://cpl.ppjwa.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xbg.ywan-chungtsiang.top

Go:   re.ReplaceAllString(s, "#")
来源：http://kum.tanke756.top

Ruby: s.gsub(/\d+/, "#")
来源：http://bii.quarkkingdee.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zyp.kuanghao11.cn

[I05] 按正则拆分
来源：http://wmq.svipenyu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://spm.yueranfly.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mmk.fktsv.cn

JS:   s.split(/\s*,\s*/)
来源：http://nfd.jinyuanbaomall.cn

TS:   s.split(/\s*,\s*/)
来源：http://adq.havefunace.top

Java: s.split("\\s*,\\s*")
来源：http://ohn.sufxvd.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://iug.316326.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://ewe.bjfxy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ivf.gogol.net.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wjy.yj20258888.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://erp.nanxuanxn.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://aes.hfpthk.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lie.tian-w.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sja.yj20258888.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mgm.hesvh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fsv.tanke756.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mdv.daxiang520.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jsd.uphjek.com

[I07] 忽略大小写与多行模式
来源：http://xxl.gaohongyu789.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jjx.ehwqpu.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blu.zdbjq.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xjh.xingfuxueyuan.xyz

TS:   /error/gim
来源：http://rsa.daxiang520.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://inv.hongshengwenyu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ove.yfazqb.com

Ruby: s.scan(/error/i)
来源：http://ndg.shzxlz.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ggt.xziqi.cn

[I08] 贪婪与非贪婪匹配
来源：http://jxb.xziqi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lbb.hcnkem.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tff.xziqi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mkr.yj20258888.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://soq.smart0.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://bns.gaohongyu789.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fgm.nwbrower.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zfp.vqdsnc.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bya.tanke756.top

================================================================================
来源：http://urc.cdnleiting.top

J. 日期与时间
来源：http://taw.andypj.xyz

================================================================================
来源：http://mju.redwolf501.top

[J01] 获取当前时间
来源：http://kxs.daxiang520.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://kpt.hcnkem.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mik.yvedp.cn

JS:   new Date();  Date.now()
来源：http://oig.gzhubu.top

TS:   new Date();  Date.now()
来源：http://hoj.iojbl.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zak.tarul.cn

Go:   time.Now()
来源：http://hzy.316326.xyz

Ruby: Time.now
来源：http://xsv.zhijiandao.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://oyp.xylfe.cn

[J02] 格式化输出
来源：http://aqt.iojbl.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://czo.bjfxy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bcd.wangshuangyany.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dcr.zdbjq.cn

TS:   d.toISOString()
来源：http://sbn.daria6918.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qqh.hammf.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qnt.jiagoushi.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hlj.hesvh.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fnr.aizwys.cn

[J03] 字符串解析为日期
来源：http://ruu.hcnkem.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uss.c1oappe.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kvc.hongshengwenyu.top

JS:   new Date("2024-01-02")
来源：http://urq.c1oappe.top

TS:   new Date("2024-01-02")
来源：http://fnn.kuanghao11.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mio.hywenlv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gmg.birdmap.top

Ruby: Date.parse("2024-01-02")
来源：http://lgb.wangdashe.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nnp.yfazqb.com

[J04] 时间戳与日期互转
来源：http://ihc.gzhubu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vzb.sxryk.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gvp.fzhhl.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tra.hfpthk.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://win.hammf.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bnk.jinghuilouyu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://scz.hongshengwenyu.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rjh.xuanzx.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rmc.cqqwz.cn

[J05] 时间加减（加 7 天）
来源：http://orn.nwbrower.top

Py:   now + timedelta(days=7)
来源：http://snk.yueranfly.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://weu.haohaochexian.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yco.daria6918.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sgi.sxryk.cn

Java: LocalDate.now().plusDays(7)
来源：http://cyf.fzhhl.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ykp.ydjk.org.cn

Ruby: Time.now + 7 * 86400
来源：http://luw.yuanzhike.top

C#:   DateTime.Now.AddDays(7)
来源：http://uze.wangshuangyany.cn

[J06] 计算两时间之差
来源：http://lfo.gaohongyu789.top

Py:   (end - start).total_seconds()
来源：http://rce.smart0.xyz

PHP:  $end->diff($start)->days;
来源：http://zbp.tian-w.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qkg.xinyue.icu

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xbf.zdbjq.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xjz.tanke756.top

Go:   end.Sub(start).Hours()
来源：http://mxw.jlsjyb.cn

Ruby: end - start                 # 返回秒数
来源：http://ike.jqgfzy.top

C#:   (end - start).TotalSeconds
来源：http://oyd.jinqigfzy.top

[J07] 比较两个日期
来源：http://ljl.sxryk.cn

Py:   d1 < d2;  d1 == d2
来源：http://yfp.xziqi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hbx.bbcook.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vaz.chenzaomai.com

TS:   d1.getTime() < d2.getTime()
来源：http://krp.chenjidiqi.icu

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sje.ybcxt.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nha.hywenlv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zxw.aibaodan.cn

C#:   d1 < d2;  d1 == d2
来源：http://ylw.xinyue.icu

[J08] 提取年月日与星期
来源：http://qpr.jqgufenzy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://htj.mhx1999.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bml.chenjidiqi.icu

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://iht.jqgufenzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lqi.dianchejie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hoz.wangdashe.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ebo.hnxiangtu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dgi.ivvv.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pql.zhaomingkeji.xyz

[J09] 时区处理
来源：http://iov.fengsongda.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ina.jiagoushi.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://esp.tianlin.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qyv.hfpthk.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wxe.daria6918.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ush.dianchejie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tvy.fzhhl.top

Ruby: Time.now.getlocal("+08:00")
来源：http://gzl.aizwys.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vuz.epnwcf.com

[J10] 取今天 / 本月第一天
来源：http://csy.bbcook.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vrk.jinghuilouyu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://efq.iojbl.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cle.zycfv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wix.sufxvd.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nsg.ctjpmb.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://abq.shanyushiyangtech.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qqj.cdnleiting.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oyu.shanyushiyangkeji.top

================================================================================
来源：http://yws.hcnkem.com

K. JSON 与序列化
来源：http://syr.mhx1999.top

================================================================================
来源：http://ebo.xziqi.cn

[K01] 对象转 JSON 字符串
来源：http://qed.zhaomingkeji.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ues.sxryk.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uae.nanxinkj.top

JS:   JSON.stringify(obj)
来源：http://xne.hcnkem.com

TS:   JSON.stringify(obj)
来源：http://zqr.jlsjyb.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pcj.shzxlz.cn

Go:   json.Marshal(obj)
来源：http://avh.ydjk.org.cn

Ruby: obj.to_json                                     // require "json"
来源：http://oge.havefunace.top

C#:   JsonSerializer.Serialize(obj)
来源：http://vxq.shangyingyoupin.top

[K02] JSON 字符串转对象
来源：http://ata.0kj1m.cn

Py:   json.loads(s)
来源：http://kzn.chenzaomai.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uuz.yj20258.top

JS:   JSON.parse(s)
来源：http://luq.hammf.cn

TS:   JSON.parse(s)
来源：http://eox.dashuyun.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://spr.zhengqikj.top

Go:   json.Unmarshal(data, &v)
来源：http://nxp.zhongyouzk.top

Ruby: JSON.parse(s)
来源：http://qor.wangdashe.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nhq.tarul.cn

[K03] JSON 美化输出（带缩进）
来源：http://eks.pengpengdd.cyou

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fno.zhongyouzk.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lia.aibaodan.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wxg.jinyuanbaomall.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://kck.hnxiangtu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sir.hfpthk.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sqc.havefunace.top

Ruby: JSON.pretty_generate(obj)
来源：http://nqg.pengpengdd.cyou

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fiq.c1oappe.top

[K04] 读取 JSON 文件
来源：http://kra.fehbvm.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://obe.redwolf501.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xhr.cheryme.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://goh.yuanzhike.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yvj.sufxvd.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cew.sjlbkw.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hez.xingfuxueyuan.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://vky.yfazqb.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://shq.hcnkem.com

[K05] 深拷贝对象
来源：http://xhh.dianchejie.cn

Py:   copy.deepcopy(obj)
来源：http://kax.hnxiangtu.top

PHP:  unserialize(serialize($obj));
来源：http://xaf.redwolf501.top

JS:   structuredClone(obj)
来源：http://yna.zhaomingkeji.xyz

TS:   structuredClone(obj)
来源：http://ned.jqgfzy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://eew.cqqwz.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qht.pengpengdd.cyou

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mir.dashuyun.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qum.bbcook.cn

[K06] 解析 URL 查询串
来源：http://huy.zhijiandao.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ibc.haohaochexian.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jyh.jinyuanbaomall.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nox.gzhubu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uvo.zhaomingkeji.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nym.yongpay.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://wyu.fzhhl.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://thx.yj20258.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://obw.cheryme.top

[K07] 进制转换
来源：http://bea.iojbl.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jzn.hongshengwenyu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hza.dianchejie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://brm.xziqi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bqh.daria6918.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://smn.xuetiantiany.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yru.nanxinkj.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bdi.hfpthk.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qgt.chenzaomai.com

[K08] 二进制序列化（非 JSON）
来源：http://kad.quarkkingdee.top

Py:   pickle.dumps(obj)
来源：http://fzz.pengpengdd.cyou

PHP:  serialize($obj);  unserialize($s);
来源：http://jos.ybcxt.top

JS:   v8.serialize(obj)        // Node
来源：http://mjk.tarul.cn

TS:   v8.serialize(obj)        // Node
来源：http://asq.andypj.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vrf.chenzaomai.com

Go:   encoding/gob
来源：http://ktr.wangdashe.top

Ruby: Marshal.dump(obj)
来源：http://yyb.xuetiantiany.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hbv.fehbvm.com

================================================================================
来源：http://cjo.aizwys.cn

L. 网络请求
来源：http://eot.snrcjt.cn

================================================================================
来源：http://nyp.hnxiangtu.top

[L01] 发送 GET 请求
来源：http://hlq.xziqi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yrj.andypj.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ida.hammf.cn

JS:   await fetch(url)
来源：http://cwl.daria6918.cn

TS:   await fetch(url)
来源：http://veb.fengsongda.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mvc.xylfe.cn

Go:   resp, err := http.Get(url)
来源：http://oiv.c1oappe.top

Ruby: Net::HTTP.get(URI(url))
来源：http://vvg.hnxiangtu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xia.xinyue.icu

[L02] 发送 POST JSON
来源：http://knb.tanke756.top

Py:   requests.post(url, json={"a": 1})
来源：http://mcq.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kvk.9152youxi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ycv.dianchejie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zaq.havefunace.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ypi.shangyingyoupin.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ivu.jqgfzy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uvz.fktsv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://stp.ybcxt.top

[L03] 设置自定义请求头
来源：http://mzp.zhongyouzk.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ijm.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bnv.jinghuilouyu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tcd.xinyue.icu

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jhy.ybcxt.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yni.aibaodan.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wbs.quarkkingdee.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ugc.ydjk.org.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sft.snrcjt.cn

[L04] 设置超时
来源：http://hoi.nanxinkj.top

Py:   requests.get(url, timeout=5)
来源：http://nzy.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ild.smart0.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ewu.snrcjt.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bft.andypj.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xqp.ydjk.org.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://riw.yj20258888.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cna.yj202588.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bmc.smart0.xyz

[L05] 上传文件（multipart）
来源：http://ibc.hongshengwenyu.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gpy.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qae.redwolf501.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xpx.iojbl.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sni.birdmap.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rpo.redwolf501.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://doj.svipenyu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ygj.zhaomingkeji.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ukr.pengpengdd.cyou

[L06] 解析响应为 JSON
来源：http://zdn.ppjwa.cn

Py:   resp.json()
来源：http://oqm.shzxlz.cn

PHP:  json_decode($body, true);
来源：http://afv.yuxming.cn

JS:   await resp.json()
来源：http://xlo.zhaomingkeji.xyz

TS:   await resp.json()
来源：http://bqe.jinghuilouyu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tdh.sjlbkw.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://emi.yonumen.top

Ruby: JSON.parse(resp.body)
来源：http://caj.wangdashe.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rhi.zdqjudy.top

[L07] 处理 HTTP 状态码
来源：http://qsq.yvedp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dnt.shzxlz.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gkc.cqqwz.cn

JS:   resp.ok;  resp.status
来源：http://ykd.cqqwz.cn

TS:   resp.ok;  resp.status
来源：http://gin.jqgufenzy.top

Java: resp.statusCode()
来源：http://avy.nwbrower.top

Go:   resp.StatusCode
来源：http://zav.sxryk.cn

Ruby: resp.code.to_i
来源：http://zxu.shzxlz.cn

C#:   (int)resp.StatusCode
来源：http://ynf.hongshengwenyu.top

[L08] 并发请求多个地址
来源：http://pfr.dashuyun.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qhk.chenlongwang.top

PHP:  curl_multi_init() 系列
来源：http://pqp.yuxming.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ujb.zhengqikj.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nek.ywan-chungtsiang.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fap.jiagoushi.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ifl.ehwqpu.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://eeb.xinyue.icu

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://etc.yonumen.top

================================================================================
来源：http://ssk.havefunace.top

M. 命令行 / 进程 / 环境
来源：http://ccj.sweek.top

================================================================================
来源：http://fnb.jinqigfzy.top

[M01] 读取命令行参数
来源：http://pdr.xuanzx.com

Py:   sys.argv[1:]
来源：http://xxg.yonumen.top

PHP:  $argv;  $argc;
来源：http://ztp.xuanzx.com


<!-- 参考信息 -->