代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bhd.9152youxi.cn

[I03] 提取捕获分组
来源：http://tyx.meibo888.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qef.bbcook.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lxz.hywenlv.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ijx.vehdjk.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fhi.aibaodan.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wul.52xcode.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vls.pengpengdd.cyou

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hwh.zhongyouzk.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uiu.feifeiyinyue.top

[I04] 正则替换
来源：http://unc.zdqjudy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://fmf.feifeiyinyue.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hzc.gzhubu.top

JS:   s.replace(/\d+/g, "#")
来源：http://haw.cheryme.top

TS:   s.replace(/\d+/g, "#")
来源：http://moy.jlsjyb.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dxl.jlsjyb.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://uxd.kuanghao11.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qoo.fehbvm.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qzn.hnxiangtu.top

[I05] 按正则拆分
来源：http://lye.wangdashe.top

Py:   re.split(r"\s*,\s*", s)
来源：http://bpb.jinghuilouyu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zef.aizwys.cn

JS:   s.split(/\s*,\s*/)
来源：http://tfl.yuanzhike.top

TS:   s.split(/\s*,\s*/)
来源：http://kgj.sxryk.cn

Java: s.split("\\s*,\\s*")
来源：http://mpj.epnwcf.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xyw.vehdjk.com

Ruby: s.split(/\s*,\s*/)
来源：http://bed.sysykeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oqe.hysaishi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ker.hesvh.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rzg.ydzc1.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uig.yuxming.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yei.quarkkingdee.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tjn.dashuyun.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mem.yj202588.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ups.tarul.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yye.zhongyouzk.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nee.chenlongwang.top

[I07] 忽略大小写与多行模式
来源：http://ydn.zdbjq.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xvx.0kj1m.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bax.aizwys.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lzn.guannengcc.top

TS:   /error/gim
来源：http://amg.yongpay.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://iks.mhx1999.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rcs.sjlbkw.cn

Ruby: s.scan(/error/i)
来源：http://jvo.sysykeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xlk.yueranfly.top

[I08] 贪婪与非贪婪匹配
来源：http://kxl.0kj1m.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yan.sysykeji.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://msj.guannengcc.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://drj.yuxming.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ftf.sxryk.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://msv.zdqjudy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mhr.sxryk.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kbx.tarul.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vjw.sweek.top

================================================================================
来源：http://nma.guowangkeji.top

J. 日期与时间
来源：http://iaz.jinghuilouyu.cn

================================================================================
来源：http://qab.xuanzx.com

[J01] 获取当前时间
来源：http://fxl.ydjk.org.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rbg.sxryk.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://iir.fanxiaobao.xyz

JS:   new Date();  Date.now()
来源：http://lwz.zhongyouzk.top

TS:   new Date();  Date.now()
来源：http://mtz.yuanzhike.top

Java: LocalDateTime.now();  Instant.now()
来源：http://joe.nanxinkj.top

Go:   time.Now()
来源：http://ojh.birdmap.top

Ruby: Time.now
来源：http://pss.jinqigufen.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pms.cashguo.top

[J02] 格式化输出
来源：http://inz.birdmap.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://brv.zhengqikj.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vzo.yfazqb.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mmt.jinyuanbaomall.cn

TS:   d.toISOString()
来源：http://nrp.vehdjk.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zmv.xuetiantiany.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rmt.jiagoushi.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://usy.andypj.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tsw.havefunace.top

[J03] 字符串解析为日期
来源：http://mhl.redwolf501.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wrc.tarul.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://iuh.uphjek.com

JS:   new Date("2024-01-02")
来源：http://qvk.jinqigfzy.top

TS:   new Date("2024-01-02")
来源：http://yqa.c1oappe.top

Java: LocalDate.parse("2024-01-02")
来源：http://ery.xylfe.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qjq.gotoacloud.top

Ruby: Date.parse("2024-01-02")
来源：http://phh.52xcode.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://eto.fktsv.cn

[J04] 时间戳与日期互转
来源：http://mfv.jiagoushi.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mac.birdmap.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://urr.bjfxy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mje.ppjwa.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://iec.dashuyun.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vaa.zhiwuduotai.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tqs.sxryk.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lwd.cheryme.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fqf.316326.xyz

[J05] 时间加减（加 7 天）
来源：http://qqb.cheryme.top

Py:   now + timedelta(days=7)
来源：http://fbg.jianghu66.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://xwt.sjlbkw.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tyw.chenlongwang.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dqn.yongpay.top

Java: LocalDate.now().plusDays(7)
来源：http://qzm.nanxinkj.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://iib.birdmap.top

Ruby: Time.now + 7 * 86400
来源：http://pib.chenjidiqi.icu

C#:   DateTime.Now.AddDays(7)
来源：http://owc.jinqigufen.top

[J06] 计算两时间之差
来源：http://odi.guowangkeji.top

Py:   (end - start).total_seconds()
来源：http://khd.sjlbkw.cn

PHP:  $end->diff($start)->days;
来源：http://big.uphjek.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ixe.c1oappe.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yjy.jinqigfzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://jii.xuanzx.com

Go:   end.Sub(start).Hours()
来源：http://yps.zhaomingkeji.xyz

Ruby: end - start                 # 返回秒数
来源：http://nxn.wangshuangyany.cn

C#:   (end - start).TotalSeconds
来源：http://tuw.daxiang520.top

[J07] 比较两个日期
来源：http://ixp.hysaishi.cn

Py:   d1 < d2;  d1 == d2
来源：http://los.cheryme.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bcl.redwolf501.top

JS:   d1.getTime() < d2.getTime()
来源：http://mjz.xuetiantiany.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kyd.jqgufenzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://prd.bbcook.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hyj.guowangkeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://lhg.sufxvd.cn

C#:   d1 < d2;  d1 == d2
来源：http://jcn.haohaochexian.top

[J08] 提取年月日与星期
来源：http://vah.yuxming.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://izr.zdbjq.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://eqz.jiagoushi.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bqe.ivvv.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zsj.yongpay.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ujc.cheryme.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vxo.52xcode.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://oxk.aizwys.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dcn.sjlbkw.cn

[J09] 时区处理
来源：http://hgs.xuanzx.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dig.yj20258.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sfa.chenjidiqi.icu

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pjo.pengpengdd.cyou

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ozn.tianlin.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ial.xingfuxueyuan.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qfd.sufxvd.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ruo.jyoumei.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jsp.chenjidiqi.icu

[J10] 取今天 / 本月第一天
来源：http://ead.fehbvm.com

Py:   date.today();  date.today().replace(day=1)
来源：http://whp.yongpay.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yca.xinyue.icu

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ofb.fengsongda.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vpl.yj20258888.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yqb.havefunace.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dnn.sxryk.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hrd.ivvv.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bol.cqqwz.cn

================================================================================
来源：http://wcr.jianghu66.top

K. JSON 与序列化
来源：http://fsy.iojbl.cn

================================================================================
来源：http://ory.zhijiandao.cn

[K01] 对象转 JSON 字符串
来源：http://nal.hongshengwenyu.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lzi.ywan-chungtsiang.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://prp.zhijiandao.cn

JS:   JSON.stringify(obj)
来源：http://kmk.jinqigfzy.top

TS:   JSON.stringify(obj)
来源：http://cwg.chenzaomai.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rdj.jqgufenzy.top

Go:   json.Marshal(obj)
来源：http://yuc.yongpay.top

Ruby: obj.to_json                                     // require "json"
来源：http://mej.c1oappe.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ojm.gogol.net.cn

[K02] JSON 字符串转对象
来源：http://xrw.jqgfzy.top

Py:   json.loads(s)
来源：http://kdj.snrcjt.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://aiq.dashuyun.cn

JS:   JSON.parse(s)
来源：http://ljd.jqgufenzy.top

TS:   JSON.parse(s)
来源：http://qqi.gogol.net.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jao.kuanghao11.cn

Go:   json.Unmarshal(data, &v)
来源：http://dpf.ehwqpu.com

Ruby: JSON.parse(s)
来源：http://led.cashguo.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://emn.cashguo.top

[K03] JSON 美化输出（带缩进）
来源：http://voe.xingfuxueyuan.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://inx.tian-w.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zgw.hongshengwenyu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://tpy.zhiwuduotai.top

TS:   JSON.stringify(obj, null, 2)
来源：http://bms.bjfxy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://myk.meibo888.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fyv.yueranfly.top

Ruby: JSON.pretty_generate(obj)
来源：http://sxf.xinyue.icu

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wmq.zhiwuduotai.top

[K04] 读取 JSON 文件
来源：http://tpd.aibaodan.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lyq.tian-w.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://geg.cucudq.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mcp.yvedp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://das.xingfuxueyuan.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jtx.haohaochexian.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vdf.ppjwa.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ecm.sysykeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mhq.kuanghao11.cn

[K05] 深拷贝对象
来源：http://ygc.nanxinkj.top

Py:   copy.deepcopy(obj)
来源：http://ojs.havefunace.top

PHP:  unserialize(serialize($obj));
来源：http://wsr.cucudq.cn

JS:   structuredClone(obj)
来源：http://noh.dianchejie.cn

TS:   structuredClone(obj)
来源：http://ryk.jinqigufen.top

Java: // 手写拷贝构造，或序列化往返
来源：http://vmx.gaohongyu789.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://epx.jiagoushi.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xjr.jianghu66.top

C#:   // 序列化往返，或自定义 Clone
来源：http://isd.shanyushiyangtech.top

[K06] 解析 URL 查询串
来源：http://lfb.nwbrower.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nfg.tianlin.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wbl.zdqjudy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fve.sufxvd.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://umw.fanxiaobao.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://usg.shzxlz.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://quk.ivvv.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yvw.fzhhl.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fph.meibo888.top

[K07] 进制转换
来源：http://qff.tarul.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jfy.smart0.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bhk.sjlbkw.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nsb.pengpengdd.cyou

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vyy.jqgfzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://itd.ctjpmb.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cdv.jinghuilouyu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://utp.quarkkingdee.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rpq.cqqwz.cn

[K08] 二进制序列化（非 JSON）
来源：http://uyj.zhengqikj.top

Py:   pickle.dumps(obj)
来源：http://gbl.yj20258.top

PHP:  serialize($obj);  unserialize($s);
来源：http://lip.fengsongda.top

JS:   v8.serialize(obj)        // Node
来源：http://fzu.zhoulong.xyz

TS:   v8.serialize(obj)        // Node
来源：http://ety.jiagoushi.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kgi.jinqigufen.top

Go:   encoding/gob
来源：http://koa.zhengqikj.top

Ruby: Marshal.dump(obj)
来源：http://aeu.feifeiyinyue.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jzk.hfpthk.cn

================================================================================
来源：http://rmb.havefunace.top

L. 网络请求
来源：http://lys.gotoacloud.top

================================================================================
来源：http://qyv.sweek.top

[L01] 发送 GET 请求
来源：http://rgv.xylfe.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://agc.tarul.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ail.gotoacloud.top

JS:   await fetch(url)
来源：http://xeb.xingfuxueyuan.xyz

TS:   await fetch(url)
来源：http://pfz.vqdsnc.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nea.zhiwuduotai.top

Go:   resp, err := http.Get(url)
来源：http://xcx.jinqigufen.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dvr.birdmap.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yud.tianlin.xyz

[L02] 发送 POST JSON
来源：http://mdn.yonumen.top

Py:   requests.post(url, json={"a": 1})
来源：http://tmp.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hoy.feifeiyinyue.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tbe.dianchejie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ytj.zhijiandao.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fdv.ehwqpu.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qcm.gzhubu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wdl.sxryk.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wjv.chenlongwang.top

[L03] 设置自定义请求头
来源：http://pet.ctjpmb.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rrk.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nsk.fehbvm.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zku.yongpay.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yzr.jinqigufen.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bjq.tarul.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kcy.ehwqpu.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fnp.iojbl.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pkd.ehwqpu.com

[L04] 设置超时
来源：http://sbu.fanxiaobao.xyz

Py:   requests.get(url, timeout=5)
来源：http://rcc.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jso.pengpengdd.cyou

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dus.feifeiyinyue.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lsr.sxryk.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vvu.hcnkem.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xsi.ppjwa.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tnx.316326.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ylg.shangyingyoupin.top

[L05] 上传文件（multipart）
来源：http://lzk.jinyuanbaomall.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://quu.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zjg.guannengcc.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://euc.birdmap.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ias.ydjk.org.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tup.gaohongyu789.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zue.fehbvm.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zgi.yj20258888.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hdz.nanxuanxn.top

[L06] 解析响应为 JSON
来源：http://xxc.hongshengwenyu.top

Py:   resp.json()
来源：http://rim.kuanghao11.cn

PHP:  json_decode($body, true);
来源：http://pcg.dashuyun.cn

JS:   await resp.json()
来源：http://mqw.xuanzx.com

TS:   await resp.json()
来源：http://usi.nanxuanxn.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ylh.vehdjk.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xem.wangdashe.top

Ruby: JSON.parse(resp.body)
来源：http://btk.yj20258888.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qwi.hnqzz.top

[L07] 处理 HTTP 状态码
来源：http://nwd.chenlongwang.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kzk.zdqjudy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ryc.hesvh.cn

JS:   resp.ok;  resp.status
来源：http://otc.yueranfly.top

TS:   resp.ok;  resp.status
来源：http://hid.ywan-chungtsiang.top

Java: resp.statusCode()
来源：http://wof.shzxlz.cn

Go:   resp.StatusCode
来源：http://kse.gogol.net.cn

Ruby: resp.code.to_i
来源：http://gtj.cqqwz.cn

C#:   (int)resp.StatusCode
来源：http://cto.zhaomingkeji.xyz

[L08] 并发请求多个地址
来源：http://xdy.uphjek.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lrg.yangfankeji.com

PHP:  curl_multi_init() 系列
来源：http://exx.shuidangran.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://okn.sjlbkw.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bvf.9152youxi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hhy.tianlin.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xaf.nwbrower.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vej.yvedp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hyd.sjlbkw.cn

================================================================================
来源：http://vrs.ivvv.top

M. 命令行 / 进程 / 环境
来源：http://aju.mhx1999.top


<!-- 参考信息 -->