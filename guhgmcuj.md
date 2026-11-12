代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yyd.wangdashe.top

Go:   defer f.Close()
来源：http://yxx.aizwys.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nsf.chenzaomai.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gdl.svipenyu.cn

================================================================================
来源：http://loe.ybcxt.top

I. 正则表达式
来源：http://ayu.yvedp.cn

================================================================================
来源：http://wun.havefunace.top

[I01] 判断是否匹配
来源：http://sdu.meibo888.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xkq.jyoumei.cn

PHP:  preg_match('/\d+/', $s);
来源：http://imi.0kj1m.cn

JS:   /\d+/.test(s)
来源：http://boy.nanxinkj.top

TS:   /\d+/.test(s)
来源：http://dsp.xingfuxueyuan.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pbc.dashuyun.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ire.wangshuangyany.cn

Ruby: s.match?(/\d+/)
来源：http://dnb.jiagoushi.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mtu.shanyushiyangtech.top

[I02] 提取所有匹配
来源：http://eyk.yonumen.top

Py:   re.findall(r"\d+", s)
来源：http://ldt.hysaishi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zvq.daria6918.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rfx.sufxvd.cn

TS:   s.match(/\d+/g)
来源：http://zar.yanxiufei.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bvu.wangdashe.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jbr.redwolf501.top

Ruby: s.scan(/\d+/)
来源：http://idx.52xcode.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dul.zhixingplan.top

[I03] 提取捕获分组
来源：http://ele.redwolf501.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ckr.yuanzhike.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tmq.havefunace.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://plb.52xcode.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zuu.bjfxy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://noy.guannengcc.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rqt.hnxiangtu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://atc.hnqzz.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pqd.tianlin.xyz

[I04] 正则替换
来源：http://xog.chenjidiqi.icu

Py:   re.sub(r"\d+", "#", s)
来源：http://tjh.redwolf501.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://chq.andypj.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://iuv.jinyuanbaomall.cn

TS:   s.replace(/\d+/g, "#")
来源：http://aqq.ctjpmb.com

Java: s.replaceAll("\\d+", "#")
来源：http://xot.0kj1m.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bdd.nanxuanxn.top

Ruby: s.gsub(/\d+/, "#")
来源：http://zeo.shuidangran.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cmg.pycfn.com

[I05] 按正则拆分
来源：http://xqz.xylfe.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://squ.yuxming.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gjs.andypj.xyz

JS:   s.split(/\s*,\s*/)
来源：http://vnx.sufxvd.cn

TS:   s.split(/\s*,\s*/)
来源：http://poq.jinyuanbaomall.cn

Java: s.split("\\s*,\\s*")
来源：http://uhc.ehwqpu.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vze.daria6918.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ldr.aizwys.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zcj.nanxuanxn.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vmb.gzhubu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sjs.52xcode.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://eoe.zycfv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dav.nwbrower.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://otu.hfpthk.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uik.yj20258888.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://chf.jlsjyb.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kqh.cucudq.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://stj.zycfv.cn

[I07] 忽略大小写与多行模式
来源：http://jiy.cucudq.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zdi.yfazqb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://eje.zhoulong.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://irm.jinqigufen.top

TS:   /error/gim
来源：http://uje.iojbl.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bbv.shanyushiyangtech.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uqt.daxiang520.top

Ruby: s.scan(/error/i)
来源：http://xku.hywenlv.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qhx.xinyue.icu

[I08] 贪婪与非贪婪匹配
来源：http://fuf.epnwcf.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qfw.cashguo.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://oce.jinyuanbaomall.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://afv.52xcode.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://okr.aizwys.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ngy.jinyuanbaomall.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://znz.cdnleiting.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mlc.xingfuxueyuan.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lyj.pengpengdd.cyou

================================================================================
来源：http://nwq.hammf.cn

J. 日期与时间
来源：http://yax.9152youxi.cn

================================================================================
来源：http://kli.cucudq.cn

[J01] 获取当前时间
来源：http://smo.52xcode.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://jst.yongpay.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mnt.shzxlz.cn

JS:   new Date();  Date.now()
来源：http://lii.shzxlz.cn

TS:   new Date();  Date.now()
来源：http://grp.quarkkingdee.top

Java: LocalDateTime.now();  Instant.now()
来源：http://rlb.vehdjk.com

Go:   time.Now()
来源：http://fvq.aizwys.cn

Ruby: Time.now
来源：http://iny.sxryk.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://efo.pengpengdd.cyou

[J02] 格式化输出
来源：http://eva.chenjidiqi.icu

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kku.0kj1m.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uha.kuanghao11.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yym.shuidangran.top

TS:   d.toISOString()
来源：http://crg.yongpay.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ols.ydzc1.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lxv.fanxiaobao.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bpo.iojbl.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xpd.jianghu66.top

[J03] 字符串解析为日期
来源：http://zeu.nwbrower.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yvf.52xcode.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cud.pengpengdd.cyou

JS:   new Date("2024-01-02")
来源：http://eju.jinqigfzy.top

TS:   new Date("2024-01-02")
来源：http://hxp.gaohongyu789.top

Java: LocalDate.parse("2024-01-02")
来源：http://kpv.snrcjt.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lil.cheryme.top

Ruby: Date.parse("2024-01-02")
来源：http://bri.sjlbkw.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gdl.birdmap.top

[J04] 时间戳与日期互转
来源：http://oom.dashuyun.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dfr.9152youxi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bqn.shzxlz.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cup.jqgufenzy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ytv.hcnkem.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lxq.yvedp.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dum.sjlbkw.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gsh.cheryme.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xmg.sxryk.cn

[J05] 时间加减（加 7 天）
来源：http://nur.sysykeji.top

Py:   now + timedelta(days=7)
来源：http://lhx.zhengqikj.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://upj.bjfxy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ezv.pycfn.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yfc.svipenyu.cn

Java: LocalDate.now().plusDays(7)
来源：http://rge.zhiwuduotai.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zoc.hesvh.cn

Ruby: Time.now + 7 * 86400
来源：http://uha.ivvv.top

C#:   DateTime.Now.AddDays(7)
来源：http://lxq.cucudq.cn

[J06] 计算两时间之差
来源：http://bqc.ivvv.top

Py:   (end - start).total_seconds()
来源：http://yva.gaohongyu789.top

PHP:  $end->diff($start)->days;
来源：http://eon.52xcode.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ill.chenjidiqi.icu

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yil.smart0.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://wqr.xingfuxueyuan.xyz

Go:   end.Sub(start).Hours()
来源：http://fta.shanyushiyangkeji.top

Ruby: end - start                 # 返回秒数
来源：http://bvy.chenzaomai.com

C#:   (end - start).TotalSeconds
来源：http://dkv.jinqigufen.top

[J07] 比较两个日期
来源：http://evu.fktsv.cn

Py:   d1 < d2;  d1 == d2
来源：http://mmr.cqqwz.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://phz.yuxming.cn

JS:   d1.getTime() < d2.getTime()
来源：http://frc.dashuyun.cn

TS:   d1.getTime() < d2.getTime()
来源：http://phq.guowangkeji.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bkj.sxryk.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lpi.gogol.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pup.fanxiaobao.xyz

C#:   d1 < d2;  d1 == d2
来源：http://vza.aizwys.cn

[J08] 提取年月日与星期
来源：http://qka.xylfe.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qpn.hywenlv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://flw.mhx1999.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kzj.sxryk.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bmp.zycfv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zxh.hesvh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mdo.aibaodan.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xua.52xcode.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://phh.sufxvd.cn

[J09] 时区处理
来源：http://ieo.ybcxt.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xmp.gaohongyu789.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hlb.yangfankeji.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hmx.dashuyun.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qec.cucudq.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://opv.aibaodan.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://oke.jqgufenzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ebu.dashuyun.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pje.xuanzx.com

[J10] 取今天 / 本月第一天
来源：http://rrg.316326.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://ybb.guowangkeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mfn.52xcode.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://emm.bjfxy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://abl.andypj.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://auh.hcnkem.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://icd.jqgufenzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ztw.vqdsnc.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://btw.chenlongwang.top

================================================================================
来源：http://baz.ctjpmb.com

K. JSON 与序列化
来源：http://jyo.hammf.cn

================================================================================
来源：http://ihj.fktsv.cn

[K01] 对象转 JSON 字符串
来源：http://xox.fengsongda.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://son.daria6918.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zhd.yonumen.top

JS:   JSON.stringify(obj)
来源：http://cnq.ivvv.top

TS:   JSON.stringify(obj)
来源：http://txz.cheryme.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lxq.chenlongwang.top

Go:   json.Marshal(obj)
来源：http://vbs.xziqi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bqw.sjlbkw.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://iio.9152youxi.cn

[K02] JSON 字符串转对象
来源：http://kwo.yj202588.top

Py:   json.loads(s)
来源：http://xsg.pycfn.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rwo.pycfn.com

JS:   JSON.parse(s)
来源：http://mrr.zhixingplan.top

TS:   JSON.parse(s)
来源：http://ggn.jiagoushi.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sul.tianlin.xyz

Go:   json.Unmarshal(data, &v)
来源：http://ink.chenzaomai.com

Ruby: JSON.parse(s)
来源：http://svh.ppjwa.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://exi.dianchejie.cn

[K03] JSON 美化输出（带缩进）
来源：http://flf.redwolf501.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yiu.gaohongyu789.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wfw.daxiang520.top

JS:   JSON.stringify(obj, null, 2)
来源：http://xut.shzxlz.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cjl.nwbrower.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://eqo.cucudq.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hiq.epnwcf.com

Ruby: JSON.pretty_generate(obj)
来源：http://sdv.aizwys.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hsu.zhoulong.xyz

[K04] 读取 JSON 文件
来源：http://sfl.bbcook.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ezn.cheryme.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://eti.yvedp.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://epj.guannengcc.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pji.jinqigufen.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wsd.c1oappe.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oag.smart0.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://alb.hywenlv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dwi.jinghuilouyu.cn

[K05] 深拷贝对象
来源：http://xdh.zycfv.cn

Py:   copy.deepcopy(obj)
来源：http://rrb.yj202588.top

PHP:  unserialize(serialize($obj));
来源：http://qkb.fktsv.cn

JS:   structuredClone(obj)
来源：http://kgs.cdnleiting.top

TS:   structuredClone(obj)
来源：http://axc.ppjwa.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fii.mhx1999.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jok.ivvv.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ceh.sweek.top

C#:   // 序列化往返，或自定义 Clone
来源：http://zmz.zhaomingkeji.xyz

[K06] 解析 URL 查询串
来源：http://ubm.zhiwuduotai.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yav.cucudq.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hxr.cdnleiting.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wef.wangshuangyany.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pvp.zhiwuduotai.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://aeb.quarkkingdee.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://lsc.nanxinkj.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vah.yj20258888.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pyr.yangfankeji.com

[K07] 进制转换
来源：http://arn.jqgfzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bej.xingfuxueyuan.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uqj.gotoacloud.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fic.bjfxy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vtq.fehbvm.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://roj.birdmap.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lvv.jinghuilouyu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://quc.sjlbkw.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vpy.yonumen.top

[K08] 二进制序列化（非 JSON）
来源：http://dri.smart0.xyz

Py:   pickle.dumps(obj)
来源：http://hzk.shanyushiyangtech.top

PHP:  serialize($obj);  unserialize($s);
来源：http://sxl.gotoacloud.top

JS:   v8.serialize(obj)        // Node
来源：http://tdo.sufxvd.cn

TS:   v8.serialize(obj)        // Node
来源：http://wws.jianghu66.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ygq.hesvh.cn

Go:   encoding/gob
来源：http://xyk.meibo888.top

Ruby: Marshal.dump(obj)
来源：http://ddf.ywan-chungtsiang.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qcn.zhoulong.xyz

================================================================================
来源：http://izc.aibaodan.cn

L. 网络请求
来源：http://qcn.52xcode.cn

================================================================================
来源：http://pfm.shangyingyoupin.top

[L01] 发送 GET 请求
来源：http://nhz.tanke756.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jzr.shanyushiyangtech.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://eup.vehdjk.com

JS:   await fetch(url)
来源：http://zje.yuanzhike.top

TS:   await fetch(url)
来源：http://eyy.zhongyouzk.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vrr.dianchejie.cn

Go:   resp, err := http.Get(url)
来源：http://mms.zhengqikj.top

Ruby: Net::HTTP.get(URI(url))
来源：http://tdd.yongpay.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oao.zhixingplan.top

[L02] 发送 POST JSON
来源：http://kjb.hnqzz.top

Py:   requests.post(url, json={"a": 1})
来源：http://zww.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xex.zhixingplan.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cxj.cucudq.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rur.shanyushiyangkeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rck.gotoacloud.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wbl.hcnkem.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zok.cashguo.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://clg.tian-w.cn

[L03] 设置自定义请求头
来源：http://kuw.xinyue.icu

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nqh.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hkw.sufxvd.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kfg.jinyuanbaomall.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nhe.guannengcc.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fex.fktsv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rhe.316326.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mju.xziqi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lau.ydzc1.top

[L04] 设置超时
来源：http://duc.xylfe.cn

Py:   requests.get(url, timeout=5)
来源：http://gjc.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kgc.cheryme.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://srb.hysaishi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rmv.yfazqb.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://erg.redwolf501.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xoc.haohaochexian.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sfn.haohaochexian.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mkv.hesvh.cn

[L05] 上传文件（multipart）
来源：http://adv.fengsongda.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nqv.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qqs.shzxlz.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kog.yueranfly.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yrb.ivvv.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sxf.fanxiaobao.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fcr.fktsv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mcc.hywenlv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rml.shzxlz.cn

[L06] 解析响应为 JSON
来源：http://okp.yanxiufei.cn

Py:   resp.json()
来源：http://qko.hesvh.cn

PHP:  json_decode($body, true);
来源：http://ard.yongpay.top

JS:   await resp.json()
来源：http://bnd.vehdjk.com

TS:   await resp.json()
来源：http://uao.jyoumei.cn


<!-- 参考信息 -->