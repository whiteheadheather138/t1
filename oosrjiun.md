代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lif.jlsjyb.cn

JS:   s.replace(/\d+/g, "#")
来源：http://gtu.ybcxt.top

TS:   s.replace(/\d+/g, "#")
来源：http://uti.zycfv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gam.sxryk.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jgx.yj20258.top

Ruby: s.gsub(/\d+/, "#")
来源：http://nto.yangfankeji.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gjc.epnwcf.com

[I05] 按正则拆分
来源：http://qcs.xuanzx.com

Py:   re.split(r"\s*,\s*", s)
来源：http://ekw.vehdjk.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wir.hfpthk.cn

JS:   s.split(/\s*,\s*/)
来源：http://jwg.xingfuxueyuan.xyz

TS:   s.split(/\s*,\s*/)
来源：http://cut.fanxiaobao.xyz

Java: s.split("\\s*,\\s*")
来源：http://idm.sysykeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://adv.daxiang520.top

Ruby: s.split(/\s*,\s*/)
来源：http://pya.daxiang520.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nke.fktsv.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gvm.xuetiantiany.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wqp.zycfv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fav.epnwcf.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://awy.jyoumei.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yua.shanyushiyangtech.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hgl.hnqzz.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mzk.jinyuanbaomall.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nye.haohaochexian.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mxw.pengpengdd.cyou

[I07] 忽略大小写与多行模式
来源：http://buz.ivvv.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://luy.wangshuangyany.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://snr.chenzaomai.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jqy.yj20258.top

TS:   /error/gim
来源：http://kos.9152youxi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gic.yj202588.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://muk.epnwcf.com

Ruby: s.scan(/error/i)
来源：http://lpk.dashuyun.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zbh.316326.xyz

[I08] 贪婪与非贪婪匹配
来源：http://zuy.guowangkeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sgo.vehdjk.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://umz.hesvh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mur.316326.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://euf.guannengcc.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://teq.hcnkem.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blo.jinqigufen.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cue.hesvh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mww.hysaishi.cn

================================================================================
来源：http://jgt.yanxiufei.cn

J. 日期与时间
来源：http://rih.hammf.cn

================================================================================
来源：http://mjq.dianchejie.cn

[J01] 获取当前时间
来源：http://zmy.ybcxt.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://jjv.jlsjyb.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://oil.jqgfzy.top

JS:   new Date();  Date.now()
来源：http://qvr.tanke756.top

TS:   new Date();  Date.now()
来源：http://hcs.fanxiaobao.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://utj.yongpay.top

Go:   time.Now()
来源：http://ykb.tianlin.xyz

Ruby: Time.now
来源：http://otl.yj20258888.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://iop.yanxiufei.cn

[J02] 格式化输出
来源：http://plr.yj20258.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ztj.tanke756.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hqt.shangyingyoupin.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vdg.bjfxy.top

TS:   d.toISOString()
来源：http://grz.sweek.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kly.redwolf501.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://onw.sysykeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qgk.hammf.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oqn.jinqigfzy.top

[J03] 字符串解析为日期
来源：http://uzs.vqdsnc.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fot.svipenyu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://isw.xuanzx.com

JS:   new Date("2024-01-02")
来源：http://jry.vehdjk.com

TS:   new Date("2024-01-02")
来源：http://ski.tianlin.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://irr.jyoumei.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://idb.shanyushiyangtech.top

Ruby: Date.parse("2024-01-02")
来源：http://oim.ppjwa.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ohj.hywenlv.cn

[J04] 时间戳与日期互转
来源：http://dlt.yj202588.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pbk.cheryme.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://btq.jlsjyb.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zqb.yj20258.top

TS:   Math.floor(Date.now() / 1000)
来源：http://clh.jinqigufen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kfs.gotoacloud.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ekb.feifeiyinyue.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://woo.fengsongda.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xfr.yj202588.top

[J05] 时间加减（加 7 天）
来源：http://yhi.aizwys.cn

Py:   now + timedelta(days=7)
来源：http://dmi.ehwqpu.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://dok.uphjek.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ggy.haohaochexian.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ija.xziqi.cn

Java: LocalDate.now().plusDays(7)
来源：http://hyt.hywenlv.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wvb.aibaodan.cn

Ruby: Time.now + 7 * 86400
来源：http://nif.jinqigfzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://vqw.c1oappe.top

[J06] 计算两时间之差
来源：http://drp.nwbrower.top

Py:   (end - start).total_seconds()
来源：http://jjs.ehwqpu.com

PHP:  $end->diff($start)->days;
来源：http://hoc.chenlongwang.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nbm.yongpay.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hky.yongpay.top

Java: Duration.between(start, end).toSeconds()
来源：http://eol.vehdjk.com

Go:   end.Sub(start).Hours()
来源：http://rvq.tian-w.cn

Ruby: end - start                 # 返回秒数
来源：http://nls.hnxiangtu.top

C#:   (end - start).TotalSeconds
来源：http://bde.yj202588.top

[J07] 比较两个日期
来源：http://ztr.gaohongyu789.top

Py:   d1 < d2;  d1 == d2
来源：http://pbj.jiagoushi.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lki.zhiwuduotai.top

JS:   d1.getTime() < d2.getTime()
来源：http://apg.sweek.top

TS:   d1.getTime() < d2.getTime()
来源：http://rdv.chenjidiqi.icu

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vyx.cashguo.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gac.pycfn.com

Ruby: d1 < d2;  d1 == d2
来源：http://npw.feifeiyinyue.top

C#:   d1 < d2;  d1 == d2
来源：http://lvs.gotoacloud.top

[J08] 提取年月日与星期
来源：http://bln.316326.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cgg.hcnkem.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://psk.zhiwuduotai.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hor.nanxuanxn.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jyx.sweek.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yns.nanxuanxn.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ctp.hnxiangtu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lcw.epnwcf.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://swx.fanxiaobao.xyz

[J09] 时区处理
来源：http://nqq.gzhubu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zje.jianghu66.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://emo.bbcook.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jtw.cashguo.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uom.mhx1999.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gpd.hnxiangtu.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hho.nanxinkj.top

Ruby: Time.now.getlocal("+08:00")
来源：http://bji.tanke756.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cgw.cheryme.top

[J10] 取今天 / 本月第一天
来源：http://hpw.ydzc1.top

Py:   date.today();  date.today().replace(day=1)
来源：http://npi.snrcjt.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jxb.yfazqb.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://piq.guannengcc.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://eiu.zhengqikj.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://aod.bjfxy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xop.chenjidiqi.icu

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wdc.feifeiyinyue.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jsf.fengsongda.top

================================================================================
来源：http://syd.mhx1999.top

K. JSON 与序列化
来源：http://iqh.ydjk.org.cn

================================================================================
来源：http://cjb.jqgfzy.top

[K01] 对象转 JSON 字符串
来源：http://pdb.52xcode.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ioo.uphjek.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://iee.hnxiangtu.top

JS:   JSON.stringify(obj)
来源：http://szn.dashuyun.cn

TS:   JSON.stringify(obj)
来源：http://xwi.guannengcc.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fzx.jinqigufen.top

Go:   json.Marshal(obj)
来源：http://bln.yfazqb.com

Ruby: obj.to_json                                     // require "json"
来源：http://hey.vqdsnc.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fbq.gogol.net.cn

[K02] JSON 字符串转对象
来源：http://rdt.guannengcc.top

Py:   json.loads(s)
来源：http://wiz.pengpengdd.cyou

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://oqz.yuanzhike.top

JS:   JSON.parse(s)
来源：http://xfa.zdbjq.cn

TS:   JSON.parse(s)
来源：http://xfw.zhoulong.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vtc.jinqigfzy.top

Go:   json.Unmarshal(data, &v)
来源：http://yrz.cucudq.cn

Ruby: JSON.parse(s)
来源：http://qpp.gotoacloud.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jhu.yj202588.top

[K03] JSON 美化输出（带缩进）
来源：http://dps.tanke756.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wvy.gaohongyu789.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jse.shanyushiyangkeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://tva.tianlin.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://whb.nanxinkj.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://urg.zhengqikj.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://irc.yangfankeji.com

Ruby: JSON.pretty_generate(obj)
来源：http://btu.xuetiantiany.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kmj.cashguo.top

[K04] 读取 JSON 文件
来源：http://qgs.ywan-chungtsiang.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jhd.hfpthk.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mlc.ctjpmb.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kwl.cdnleiting.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://acv.yfazqb.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tmf.hnxiangtu.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jtd.nwbrower.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://rxh.hongshengwenyu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zct.sysykeji.top

[K05] 深拷贝对象
来源：http://omh.cqqwz.cn

Py:   copy.deepcopy(obj)
来源：http://bdb.chenlongwang.top

PHP:  unserialize(serialize($obj));
来源：http://zjo.chenlongwang.top

JS:   structuredClone(obj)
来源：http://ukc.yuxming.cn

TS:   structuredClone(obj)
来源：http://jyy.jianghu66.top

Java: // 手写拷贝构造，或序列化往返
来源：http://sng.yueranfly.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mcd.guowangkeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fdl.sjlbkw.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cty.jinghuilouyu.cn

[K06] 解析 URL 查询串
来源：http://qmj.vehdjk.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://udx.mhx1999.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lxy.zycfv.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eop.vehdjk.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://urr.mhx1999.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xfc.shanyushiyangtech.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://oui.sufxvd.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qzf.jlsjyb.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rov.guowangkeji.top

[K07] 进制转换
来源：http://uzm.nwbrower.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://aym.yuanzhike.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vqr.hongshengwenyu.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lmw.xinyue.icu

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://czu.gzhubu.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zpz.birdmap.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ksw.gzhubu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://npb.dashuyun.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pbg.meibo888.top

[K08] 二进制序列化（非 JSON）
来源：http://atu.chenlongwang.top

Py:   pickle.dumps(obj)
来源：http://dfe.daria6918.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hwb.pycfn.com

JS:   v8.serialize(obj)        // Node
来源：http://fzc.bjfxy.top

TS:   v8.serialize(obj)        // Node
来源：http://udq.xuanzx.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://onw.sufxvd.cn

Go:   encoding/gob
来源：http://ewr.cdnleiting.top

Ruby: Marshal.dump(obj)
来源：http://nlb.shuidangran.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fss.fengsongda.top

================================================================================
来源：http://nsy.svipenyu.cn

L. 网络请求
来源：http://ize.snrcjt.cn

================================================================================
来源：http://yrm.sweek.top

[L01] 发送 GET 请求
来源：http://tqz.zhiwuduotai.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fiv.cheryme.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kpe.quarkkingdee.top

JS:   await fetch(url)
来源：http://xjf.wangshuangyany.cn

TS:   await fetch(url)
来源：http://jyc.xinyue.icu

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bie.fengsongda.top

Go:   resp, err := http.Get(url)
来源：http://dsr.mhx1999.top

Ruby: Net::HTTP.get(URI(url))
来源：http://pfu.hnxiangtu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bju.chenzaomai.com

[L02] 发送 POST JSON
来源：http://gpz.wangdashe.top

Py:   requests.post(url, json={"a": 1})
来源：http://iru.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vox.yueranfly.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://isr.zhaomingkeji.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sca.ivvv.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://grc.sufxvd.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oto.shangyingyoupin.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://api.hammf.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rzh.chenzaomai.com

[L03] 设置自定义请求头
来源：http://jdm.smart0.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://coa.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bya.smart0.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xnk.fktsv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uxg.yuxming.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jnh.0kj1m.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tsa.ctjpmb.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hrw.tarul.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://aho.svipenyu.cn

[L04] 设置超时
来源：http://xhn.ydzc1.top

Py:   requests.get(url, timeout=5)
来源：http://rlg.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kdh.jinqigfzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://svt.epnwcf.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aco.sjlbkw.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://alt.hnxiangtu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pss.cheryme.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yyc.sxryk.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://chj.tian-w.cn

[L05] 上传文件（multipart）
来源：http://oun.daria6918.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kpl.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rjl.zhengqikj.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mff.xuanzx.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wsa.haohaochexian.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fgl.yj202588.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jkr.zdqjudy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://map.andypj.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://div.hammf.cn

[L06] 解析响应为 JSON
来源：http://asq.andypj.xyz

Py:   resp.json()
来源：http://hui.hammf.cn

PHP:  json_decode($body, true);
来源：http://urj.jinghuilouyu.cn

JS:   await resp.json()
来源：http://ywo.fehbvm.com

TS:   await resp.json()
来源：http://fzf.dashuyun.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rto.jqgfzy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xzn.zdbjq.cn

Ruby: JSON.parse(resp.body)
来源：http://dba.yonumen.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qat.yj202588.top

[L07] 处理 HTTP 状态码
来源：http://ulv.zhaomingkeji.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ntd.yonumen.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pdi.c1oappe.top

JS:   resp.ok;  resp.status
来源：http://jqh.cashguo.top

TS:   resp.ok;  resp.status
来源：http://yzq.wangdashe.top

Java: resp.statusCode()
来源：http://kgm.yongpay.top

Go:   resp.StatusCode
来源：http://vfm.zdbjq.cn

Ruby: resp.code.to_i
来源：http://qzs.ydjk.org.cn

C#:   (int)resp.StatusCode
来源：http://idc.tanke756.top

[L08] 并发请求多个地址
来源：http://gnn.pycfn.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ddg.cashguo.top

PHP:  curl_multi_init() 系列
来源：http://fgc.xuetiantiany.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://asa.andypj.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xmi.nwbrower.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qny.ydjk.org.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hic.yj202588.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zvh.cucudq.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nhu.shzxlz.cn

================================================================================
来源：http://xba.nanxinkj.top

M. 命令行 / 进程 / 环境
来源：http://jwr.dashuyun.cn

================================================================================
来源：http://mzk.52xcode.cn

[M01] 读取命令行参数
来源：http://gqj.ydzc1.top

Py:   sys.argv[1:]
来源：http://qyz.hcnkem.com

PHP:  $argv;  $argc;
来源：http://cxj.pengpengdd.cyou

JS:   process.argv.slice(2)
来源：http://dbi.bbcook.cn

TS:   process.argv.slice(2)
来源：http://hsf.bjfxy.top

Java: args 数组（main 方法参数）
来源：http://quh.aibaodan.cn

Go:   os.Args[1:]
来源：http://wgy.mhx1999.top

Ruby: ARGV
来源：http://nmf.xuetiantiany.cn

C#:   args 数组（Main 方法参数）
来源：http://pmq.zycfv.cn

[M02] 读取环境变量
来源：http://mtb.tian-w.cn

Py:   os.environ.get("HOME")
来源：http://xlr.hesvh.cn


<!-- 参考信息 -->