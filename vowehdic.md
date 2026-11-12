代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://irh.c1oappe.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mfh.birdmap.top

Ruby: s.match?(/\d+/)
来源：http://bcg.svipenyu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gmj.xylfe.cn

[I02] 提取所有匹配
来源：http://tpu.hnxiangtu.top

Py:   re.findall(r"\d+", s)
来源：http://eel.epnwcf.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kik.fehbvm.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vub.ehwqpu.com

TS:   s.match(/\d+/g)
来源：http://idy.sufxvd.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kwf.gaohongyu789.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ckj.hywenlv.cn

Ruby: s.scan(/\d+/)
来源：http://tob.0kj1m.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qmg.ppjwa.cn

[I03] 提取捕获分组
来源：http://ylc.0kj1m.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mah.zhijiandao.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tei.yangfankeji.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://itd.xingfuxueyuan.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://epj.shanyushiyangtech.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bal.aibaodan.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ido.jiagoushi.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://upb.smart0.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xif.fengsongda.top

[I04] 正则替换
来源：http://orp.hammf.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://juu.tanke756.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://avp.cashguo.top

JS:   s.replace(/\d+/g, "#")
来源：http://fva.tian-w.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ttf.jianghu66.top

Java: s.replaceAll("\\d+", "#")
来源：http://ney.nwbrower.top

Go:   re.ReplaceAllString(s, "#")
来源：http://wba.shangyingyoupin.top

Ruby: s.gsub(/\d+/, "#")
来源：http://iud.ywan-chungtsiang.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mgm.daria6918.cn

[I05] 按正则拆分
来源：http://fbm.guannengcc.top

Py:   re.split(r"\s*,\s*", s)
来源：http://bqh.jqgufenzy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lzi.hywenlv.cn

JS:   s.split(/\s*,\s*/)
来源：http://elj.zhijiandao.cn

TS:   s.split(/\s*,\s*/)
来源：http://qlc.guannengcc.top

Java: s.split("\\s*,\\s*")
来源：http://hlr.wangdashe.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dna.jqgufenzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://euh.bjfxy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ysf.fehbvm.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ysw.bbcook.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hcb.pengpengdd.cyou

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://shh.fktsv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iai.sjlbkw.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ejm.hesvh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ewt.yuxming.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vvf.yj202588.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qjh.chenzaomai.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gop.gogol.net.cn

[I07] 忽略大小写与多行模式
来源：http://mix.chenzaomai.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ooh.sxryk.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://osn.daxiang520.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ybj.ehwqpu.com

TS:   /error/gim
来源：http://iip.quarkkingdee.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qsk.yueranfly.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jyz.xylfe.cn

Ruby: s.scan(/error/i)
来源：http://fjs.9152youxi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bwm.xingfuxueyuan.xyz

[I08] 贪婪与非贪婪匹配
来源：http://ddl.guannengcc.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qgs.yangfankeji.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fdg.jlsjyb.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gwq.aizwys.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uam.vehdjk.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://hct.9152youxi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ybu.cqqwz.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://obt.dashuyun.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hxf.0kj1m.cn

================================================================================
来源：http://vzm.yfazqb.com

J. 日期与时间
来源：http://waz.xuetiantiany.cn

================================================================================
来源：http://fhx.yanxiufei.cn

[J01] 获取当前时间
来源：http://ljc.feifeiyinyue.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://hom.ybcxt.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xwt.cucudq.cn

JS:   new Date();  Date.now()
来源：http://yfx.yonumen.top

TS:   new Date();  Date.now()
来源：http://bxp.hnxiangtu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://dcw.jyoumei.cn

Go:   time.Now()
来源：http://oix.yanxiufei.cn

Ruby: Time.now
来源：http://fic.xuanzx.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dpc.yueranfly.top

[J02] 格式化输出
来源：http://drp.shanyushiyangkeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vrd.hywenlv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://luh.yongpay.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fjr.gaohongyu789.top

TS:   d.toISOString()
来源：http://gga.zhijiandao.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://thf.sjlbkw.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nax.yongpay.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pgx.bjfxy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://srj.sufxvd.cn

[J03] 字符串解析为日期
来源：http://vly.nanxinkj.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://loc.zdbjq.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ygv.tarul.cn

JS:   new Date("2024-01-02")
来源：http://hmt.cucudq.cn

TS:   new Date("2024-01-02")
来源：http://aom.nanxuanxn.top

Java: LocalDate.parse("2024-01-02")
来源：http://xry.birdmap.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kbo.yangfankeji.com

Ruby: Date.parse("2024-01-02")
来源：http://cpg.zhijiandao.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xsy.ydzc1.top

[J04] 时间戳与日期互转
来源：http://whr.uphjek.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://esm.hammf.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ccx.guannengcc.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cbq.gzhubu.top

TS:   Math.floor(Date.now() / 1000)
来源：http://pgj.jianghu66.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gkq.jianghu66.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vkm.gogol.net.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nmw.feifeiyinyue.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://djf.tarul.cn

[J05] 时间加减（加 7 天）
来源：http://pyg.iojbl.cn

Py:   now + timedelta(days=7)
来源：http://xmi.xinyue.icu

PHP:  (new DateTime())->modify("+7 days");
来源：http://kod.yj20258.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gri.chenzaomai.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://srx.shanyushiyangtech.top

Java: LocalDate.now().plusDays(7)
来源：http://auu.aizwys.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bzu.fehbvm.com

Ruby: Time.now + 7 * 86400
来源：http://yos.hysaishi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zlt.nanxuanxn.top

[J06] 计算两时间之差
来源：http://waw.vqdsnc.cn

Py:   (end - start).total_seconds()
来源：http://kin.yueranfly.top

PHP:  $end->diff($start)->days;
来源：http://lwm.aibaodan.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://los.fengsongda.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://skt.vqdsnc.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qtx.hammf.cn

Go:   end.Sub(start).Hours()
来源：http://cnj.epnwcf.com

Ruby: end - start                 # 返回秒数
来源：http://qsr.hywenlv.cn

C#:   (end - start).TotalSeconds
来源：http://pue.gogol.net.cn

[J07] 比较两个日期
来源：http://rxi.haohaochexian.top

Py:   d1 < d2;  d1 == d2
来源：http://bxt.hesvh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rny.zhongyouzk.top

JS:   d1.getTime() < d2.getTime()
来源：http://axf.ybcxt.top

TS:   d1.getTime() < d2.getTime()
来源：http://zih.hongshengwenyu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wel.daria6918.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zxi.yj20258888.top

Ruby: d1 < d2;  d1 == d2
来源：http://xzx.jinghuilouyu.cn

C#:   d1 < d2;  d1 == d2
来源：http://zqb.zhengqikj.top

[J08] 提取年月日与星期
来源：http://dit.jinyuanbaomall.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xeb.hammf.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sds.fehbvm.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xsr.zycfv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://snn.sxryk.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mxs.jqgfzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://spp.0kj1m.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zjl.sufxvd.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jmc.nwbrower.top

[J09] 时区处理
来源：http://xqs.guannengcc.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sjc.xinyue.icu

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kgz.zhixingplan.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uwc.sweek.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://txv.xuetiantiany.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qhh.ybcxt.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tyb.pengpengdd.cyou

Ruby: Time.now.getlocal("+08:00")
来源：http://fvo.jinyuanbaomall.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://act.yfazqb.com

[J10] 取今天 / 本月第一天
来源：http://bhw.hongshengwenyu.top

Py:   date.today();  date.today().replace(day=1)
来源：http://jdc.guowangkeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vjq.jianghu66.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uvo.cheryme.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://icp.aibaodan.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hvn.c1oappe.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uub.redwolf501.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vde.yj202588.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vfh.pengpengdd.cyou

================================================================================
来源：http://vpc.xuanzx.com

K. JSON 与序列化
来源：http://bdg.tianlin.xyz

================================================================================
来源：http://jgp.aibaodan.cn

[K01] 对象转 JSON 字符串
来源：http://vvb.jinyuanbaomall.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ekm.jiagoushi.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ncv.chenzaomai.com

JS:   JSON.stringify(obj)
来源：http://exe.bbcook.cn

TS:   JSON.stringify(obj)
来源：http://yak.yvedp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://stn.hcnkem.com

Go:   json.Marshal(obj)
来源：http://aom.hfpthk.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mxl.zhaomingkeji.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://uqt.haohaochexian.top

[K02] JSON 字符串转对象
来源：http://zci.dashuyun.cn

Py:   json.loads(s)
来源：http://fyj.yvedp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bzq.yj202588.top

JS:   JSON.parse(s)
来源：http://bza.fktsv.cn

TS:   JSON.parse(s)
来源：http://gex.feifeiyinyue.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hma.shzxlz.cn

Go:   json.Unmarshal(data, &v)
来源：http://djs.sweek.top

Ruby: JSON.parse(s)
来源：http://jom.yongpay.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mrr.guannengcc.top

[K03] JSON 美化输出（带缩进）
来源：http://bry.zhiwuduotai.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fms.daxiang520.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ymw.zycfv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://eig.fktsv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zbs.wangdashe.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mrb.jyoumei.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fkq.cqqwz.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dtt.vqdsnc.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zzd.yuxming.cn

[K04] 读取 JSON 文件
来源：http://cpw.yuxming.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://twd.gotoacloud.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://erd.ppjwa.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jsm.havefunace.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://htg.tanke756.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rdo.hnqzz.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kzj.zdqjudy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://twu.quarkkingdee.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rex.sysykeji.top

[K05] 深拷贝对象
来源：http://hsl.nanxuanxn.top

Py:   copy.deepcopy(obj)
来源：http://ttj.dianchejie.cn

PHP:  unserialize(serialize($obj));
来源：http://bzc.tanke756.top

JS:   structuredClone(obj)
来源：http://kgq.vehdjk.com

TS:   structuredClone(obj)
来源：http://rkq.aizwys.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ong.ctjpmb.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ini.yonumen.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wkd.ydzc1.top

C#:   // 序列化往返，或自定义 Clone
来源：http://hcv.hysaishi.cn

[K06] 解析 URL 查询串
来源：http://odw.9152youxi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ubs.iojbl.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qsb.zhixingplan.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://krj.xingfuxueyuan.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qqf.chenzaomai.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://eje.shangyingyoupin.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://pfk.ywan-chungtsiang.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bba.jyoumei.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rgt.shanyushiyangtech.top

[K07] 进制转换
来源：http://drt.xylfe.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://soy.havefunace.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gtl.yangfankeji.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nwf.52xcode.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://oqq.cqqwz.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://iug.yj20258888.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jbf.jyoumei.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mtq.ivvv.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hdq.gaohongyu789.top

[K08] 二进制序列化（非 JSON）
来源：http://rev.zhoulong.xyz

Py:   pickle.dumps(obj)
来源：http://qbe.sufxvd.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vug.svipenyu.cn

JS:   v8.serialize(obj)        // Node
来源：http://fio.9152youxi.cn

TS:   v8.serialize(obj)        // Node
来源：http://peg.nanxinkj.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rzy.sweek.top

Go:   encoding/gob
来源：http://vqt.0kj1m.cn

Ruby: Marshal.dump(obj)
来源：http://osj.c1oappe.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lfy.sysykeji.top

================================================================================
来源：http://lrp.yongpay.top

L. 网络请求
来源：http://hrs.hcnkem.com

================================================================================
来源：http://alr.aibaodan.cn

[L01] 发送 GET 请求
来源：http://edn.vehdjk.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://iqk.c1oappe.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://eig.bjfxy.top

JS:   await fetch(url)
来源：http://vbc.cucudq.cn

TS:   await fetch(url)
来源：http://gqp.hnxiangtu.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gni.andypj.xyz

Go:   resp, err := http.Get(url)
来源：http://ivh.xuetiantiany.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gym.316326.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jtz.nwbrower.top

[L02] 发送 POST JSON
来源：http://opu.yueranfly.top

Py:   requests.post(url, json={"a": 1})
来源：http://fck.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://krl.vehdjk.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ysw.chenjidiqi.icu

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ekd.zhoulong.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nxu.ybcxt.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xwf.sjlbkw.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cfs.daxiang520.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ufd.hnxiangtu.top

[L03] 设置自定义请求头
来源：http://kaj.52xcode.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rcn.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fok.xuetiantiany.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jad.haohaochexian.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kff.jinghuilouyu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rhi.ybcxt.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tsn.ppjwa.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ibb.jianghu66.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://plp.vqdsnc.cn

[L04] 设置超时
来源：http://tko.sjlbkw.cn

Py:   requests.get(url, timeout=5)
来源：http://kku.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zzo.aibaodan.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ltx.hnxiangtu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wcr.yonumen.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vhg.epnwcf.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qkt.hysaishi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hrg.ivvv.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gud.zycfv.cn

[L05] 上传文件（multipart）
来源：http://unx.haohaochexian.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vos.jlsjyb.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vpc.yanxiufei.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://moa.zhaomingkeji.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ayl.smart0.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wkl.chenlongwang.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uch.xingfuxueyuan.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jlg.bbcook.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qwz.havefunace.top

[L06] 解析响应为 JSON
来源：http://fbh.gogol.net.cn

Py:   resp.json()
来源：http://oyh.52xcode.cn

PHP:  json_decode($body, true);
来源：http://vdg.xylfe.cn

JS:   await resp.json()
来源：http://zjw.shuidangran.top

TS:   await resp.json()
来源：http://qsm.jqgufenzy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://csj.shzxlz.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pcr.hesvh.cn

Ruby: JSON.parse(resp.body)
来源：http://dfe.guannengcc.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wbp.meibo888.top

[L07] 处理 HTTP 状态码
来源：http://shr.ywan-chungtsiang.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bph.sysykeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://puj.zhiwuduotai.top

JS:   resp.ok;  resp.status
来源：http://upo.shanyushiyangtech.top

TS:   resp.ok;  resp.status
来源：http://pli.ybcxt.top

Java: resp.statusCode()
来源：http://yer.cashguo.top

Go:   resp.StatusCode
来源：http://sdl.ehwqpu.com

Ruby: resp.code.to_i
来源：http://cph.hysaishi.cn


<!-- 参考信息 -->