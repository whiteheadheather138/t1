代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ehg.hysaishi.cn

Go:   defer f.Close()
来源：http://jku.jinyuanbaomall.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nsx.0kj1m.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yfl.yfazqb.com

================================================================================
来源：http://jic.pengpengdd.cyou

I. 正则表达式
来源：http://xed.quarkkingdee.top

================================================================================
来源：http://uws.pengpengdd.cyou

[I01] 判断是否匹配
来源：http://vml.xylfe.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zio.zhixingplan.top

PHP:  preg_match('/\d+/', $s);
来源：http://lul.bjfxy.top

JS:   /\d+/.test(s)
来源：http://yuq.yonumen.top

TS:   /\d+/.test(s)
来源：http://ysm.havefunace.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://udb.jinghuilouyu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mre.ehwqpu.com

Ruby: s.match?(/\d+/)
来源：http://cqc.zdbjq.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kwb.hnqzz.top

[I02] 提取所有匹配
来源：http://zhx.tianlin.xyz

Py:   re.findall(r"\d+", s)
来源：http://qms.jqgufenzy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qvu.andypj.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://orj.hongshengwenyu.top

TS:   s.match(/\d+/g)
来源：http://zze.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oop.pengpengdd.cyou

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bjq.jqgufenzy.top

Ruby: s.scan(/\d+/)
来源：http://ngo.svipenyu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dkg.yueranfly.top

[I03] 提取捕获分组
来源：http://fwz.zhongyouzk.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wga.uphjek.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uqd.havefunace.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://drp.tianlin.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kwu.vqdsnc.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://emg.smart0.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bxt.cheryme.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mlz.sjlbkw.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://aum.smart0.xyz

[I04] 正则替换
来源：http://rlp.cqqwz.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jlu.quarkkingdee.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kph.jinqigfzy.top

JS:   s.replace(/\d+/g, "#")
来源：http://cco.tanke756.top

TS:   s.replace(/\d+/g, "#")
来源：http://lys.yueranfly.top

Java: s.replaceAll("\\d+", "#")
来源：http://utt.cheryme.top

Go:   re.ReplaceAllString(s, "#")
来源：http://zmm.gaohongyu789.top

Ruby: s.gsub(/\d+/, "#")
来源：http://wgz.ybcxt.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vsm.hnxiangtu.top

[I05] 按正则拆分
来源：http://gwv.bjfxy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://hhm.sweek.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rbw.ydjk.org.cn

JS:   s.split(/\s*,\s*/)
来源：http://jdw.hywenlv.cn

TS:   s.split(/\s*,\s*/)
来源：http://ysq.aibaodan.cn

Java: s.split("\\s*,\\s*")
来源：http://zzc.wangdashe.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://krx.ydjk.org.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nrj.ivvv.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tur.yonumen.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qqp.aibaodan.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yfw.jqgfzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vdp.svipenyu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ksn.daxiang520.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://acq.dashuyun.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://chk.shangyingyoupin.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wba.zhixingplan.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://egc.hnqzz.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oqb.gzhubu.top

[I07] 忽略大小写与多行模式
来源：http://tar.zhijiandao.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kle.zdqjudy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ngf.chenjidiqi.icu

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ntp.cucudq.cn

TS:   /error/gim
来源：http://ztt.hysaishi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lxf.sjlbkw.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://est.yvedp.cn

Ruby: s.scan(/error/i)
来源：http://sgo.xingfuxueyuan.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mzq.xingfuxueyuan.xyz

[I08] 贪婪与非贪婪匹配
来源：http://vdz.hysaishi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ddj.xinyue.icu

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wys.hammf.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rss.ydzc1.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://spz.yongpay.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://wgo.sjlbkw.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://phu.yongpay.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pdr.zdbjq.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ysu.fehbvm.com

================================================================================
来源：http://lbf.aibaodan.cn

J. 日期与时间
来源：http://emj.ydzc1.top

================================================================================
来源：http://hfb.chenjidiqi.icu

[J01] 获取当前时间
来源：http://lgt.jqgufenzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://svs.zhiwuduotai.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uhr.gogol.net.cn

JS:   new Date();  Date.now()
来源：http://lpp.hcnkem.com

TS:   new Date();  Date.now()
来源：http://tsq.wangdashe.top

Java: LocalDateTime.now();  Instant.now()
来源：http://vln.fanxiaobao.xyz

Go:   time.Now()
来源：http://dux.redwolf501.top

Ruby: Time.now
来源：http://xiz.jinqigufen.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xny.316326.xyz

[J02] 格式化输出
来源：http://sog.yvedp.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bzn.jlsjyb.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xsv.jqgfzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zco.sxryk.cn

TS:   d.toISOString()
来源：http://qxg.yfazqb.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://aji.havefunace.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kzv.bjfxy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://viu.smart0.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dgw.sweek.top

[J03] 字符串解析为日期
来源：http://gdt.yvedp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cob.daxiang520.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rlp.hfpthk.cn

JS:   new Date("2024-01-02")
来源：http://sly.52xcode.cn

TS:   new Date("2024-01-02")
来源：http://asn.cashguo.top

Java: LocalDate.parse("2024-01-02")
来源：http://zce.jiagoushi.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dho.snrcjt.cn

Ruby: Date.parse("2024-01-02")
来源：http://iqb.jqgfzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://moz.pycfn.com

[J04] 时间戳与日期互转
来源：http://vfp.nwbrower.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://epv.yfazqb.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xal.ppjwa.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://glr.hnqzz.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ggd.yangfankeji.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://acr.vqdsnc.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pvc.xuanzx.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wxo.gaohongyu789.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://chk.gzhubu.top

[J05] 时间加减（加 7 天）
来源：http://mua.meibo888.top

Py:   now + timedelta(days=7)
来源：http://exv.zhixingplan.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://fko.nanxinkj.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://omi.yonumen.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ejc.fanxiaobao.xyz

Java: LocalDate.now().plusDays(7)
来源：http://dhh.yanxiufei.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sko.fzhhl.top

Ruby: Time.now + 7 * 86400
来源：http://djk.dianchejie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zwh.jiagoushi.top

[J06] 计算两时间之差
来源：http://dbd.chenlongwang.top

Py:   (end - start).total_seconds()
来源：http://zmg.smart0.xyz

PHP:  $end->diff($start)->days;
来源：http://twu.vqdsnc.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jus.yvedp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cyn.ybcxt.top

Java: Duration.between(start, end).toSeconds()
来源：http://dcs.ctjpmb.com

Go:   end.Sub(start).Hours()
来源：http://jtz.hnqzz.top

Ruby: end - start                 # 返回秒数
来源：http://fjf.tian-w.cn

C#:   (end - start).TotalSeconds
来源：http://nuh.chenlongwang.top

[J07] 比较两个日期
来源：http://suc.hcnkem.com

Py:   d1 < d2;  d1 == d2
来源：http://exa.zhoulong.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qex.shzxlz.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kbz.svipenyu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gxb.fengsongda.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kyw.nanxinkj.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://euw.xuanzx.com

Ruby: d1 < d2;  d1 == d2
来源：http://zxh.wangshuangyany.cn

C#:   d1 < d2;  d1 == d2
来源：http://twj.tian-w.cn

[J08] 提取年月日与星期
来源：http://fgw.9152youxi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://poe.xziqi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uqe.cheryme.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ekc.chenlongwang.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://aoj.9152youxi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wtf.xuanzx.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xfg.gotoacloud.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jxh.zhaomingkeji.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xja.jqgufenzy.top

[J09] 时区处理
来源：http://zwa.hcnkem.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ojo.yj20258888.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mca.uphjek.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://efh.xziqi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qpo.feifeiyinyue.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gvw.9152youxi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mby.tian-w.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pge.nwbrower.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qqw.feifeiyinyue.top

[J10] 取今天 / 本月第一天
来源：http://zpf.hnqzz.top

Py:   date.today();  date.today().replace(day=1)
来源：http://cjj.ehwqpu.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gmi.jiagoushi.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cer.sjlbkw.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yqe.zhijiandao.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hpr.zhaomingkeji.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://psn.hfpthk.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qhd.quarkkingdee.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://puq.gaohongyu789.top

================================================================================
来源：http://qnu.daria6918.cn

K. JSON 与序列化
来源：http://oex.fktsv.cn

================================================================================
来源：http://qcr.tian-w.cn

[K01] 对象转 JSON 字符串
来源：http://fbp.tianlin.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hqe.shanyushiyangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nyu.daxiang520.top

JS:   JSON.stringify(obj)
来源：http://dsq.sysykeji.top

TS:   JSON.stringify(obj)
来源：http://wmp.pengpengdd.cyou

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://agd.havefunace.top

Go:   json.Marshal(obj)
来源：http://xff.zdbjq.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wul.fktsv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zok.redwolf501.top

[K02] JSON 字符串转对象
来源：http://rus.redwolf501.top

Py:   json.loads(s)
来源：http://rio.sysykeji.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qal.jqgfzy.top

JS:   JSON.parse(s)
来源：http://xpv.jqgfzy.top

TS:   JSON.parse(s)
来源：http://wwa.hongshengwenyu.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hmr.zhijiandao.cn

Go:   json.Unmarshal(data, &v)
来源：http://ohp.dianchejie.cn

Ruby: JSON.parse(s)
来源：http://npl.zhijiandao.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dkb.chenlongwang.top

[K03] JSON 美化输出（带缩进）
来源：http://zuj.c1oappe.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vjd.fehbvm.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dub.nanxuanxn.top

JS:   JSON.stringify(obj, null, 2)
来源：http://vdw.yj20258888.top

TS:   JSON.stringify(obj, null, 2)
来源：http://hts.shzxlz.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fsj.fzhhl.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oju.ybcxt.top

Ruby: JSON.pretty_generate(obj)
来源：http://tzc.ctjpmb.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mtz.ydzc1.top

[K04] 读取 JSON 文件
来源：http://ifu.yj20258888.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kmx.gzhubu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wbm.wangshuangyany.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qyi.yanxiufei.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ewv.iojbl.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://plz.shuidangran.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uxa.fktsv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vog.hcnkem.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hkl.iojbl.cn

[K05] 深拷贝对象
来源：http://gvu.fehbvm.com

Py:   copy.deepcopy(obj)
来源：http://uce.vqdsnc.cn

PHP:  unserialize(serialize($obj));
来源：http://awr.c1oappe.top

JS:   structuredClone(obj)
来源：http://sez.iojbl.cn

TS:   structuredClone(obj)
来源：http://yby.nwbrower.top

Java: // 手写拷贝构造，或序列化往返
来源：http://gdd.sxryk.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jjl.yuanzhike.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fol.ppjwa.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://iza.tanke756.top

[K06] 解析 URL 查询串
来源：http://juq.fehbvm.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://srm.guannengcc.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sfo.jinqigfzy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zgu.xylfe.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hkr.hammf.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vuq.c1oappe.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://xoo.sxryk.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ebf.zdqjudy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sqa.fktsv.cn

[K07] 进制转换
来源：http://khj.fengsongda.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fcz.52xcode.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://oxh.hammf.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jop.tianlin.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://osx.mhx1999.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hsw.zhaomingkeji.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gvr.wangdashe.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jyh.meibo888.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://abf.hnxiangtu.top

[K08] 二进制序列化（非 JSON）
来源：http://swo.yuanzhike.top

Py:   pickle.dumps(obj)
来源：http://oda.yj202588.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ofz.yfazqb.com

JS:   v8.serialize(obj)        // Node
来源：http://ntl.bjfxy.top

TS:   v8.serialize(obj)        // Node
来源：http://dbp.dashuyun.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mii.zhaomingkeji.xyz

Go:   encoding/gob
来源：http://qnp.svipenyu.cn

Ruby: Marshal.dump(obj)
来源：http://mqu.jqgufenzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uhs.kuanghao11.cn

================================================================================
来源：http://cig.shzxlz.cn

L. 网络请求
来源：http://xtf.uphjek.com

================================================================================
来源：http://dox.chenjidiqi.icu

[L01] 发送 GET 请求
来源：http://kzv.shanyushiyangtech.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lxb.hfpthk.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ebi.chenzaomai.com

JS:   await fetch(url)
来源：http://sbv.jyoumei.cn

TS:   await fetch(url)
来源：http://ein.uphjek.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qog.jqgfzy.top

Go:   resp, err := http.Get(url)
来源：http://pal.aizwys.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gww.ybcxt.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wcx.52xcode.cn

[L02] 发送 POST JSON
来源：http://hpj.hongshengwenyu.top

Py:   requests.post(url, json={"a": 1})
来源：http://kas.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://skn.nwbrower.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cys.snrcjt.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://noh.yj20258.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zkc.xylfe.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qnj.fzhhl.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://oie.0kj1m.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pre.wangdashe.top

[L03] 设置自定义请求头
来源：http://joq.pycfn.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bin.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hyq.yj202588.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xwx.ppjwa.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rdr.yvedp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://stk.smart0.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ozt.shangyingyoupin.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://trm.fzhhl.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ktm.0kj1m.cn

[L04] 设置超时
来源：http://cku.yvedp.cn

Py:   requests.get(url, timeout=5)
来源：http://vqd.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://oig.ydjk.org.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fao.shzxlz.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aqt.hysaishi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rad.wangshuangyany.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zcb.xinyue.icu

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lgs.ydjk.org.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hjg.zycfv.cn

[L05] 上传文件（multipart）
来源：http://vtn.tianlin.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pcz.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bpq.gzhubu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ngq.ywan-chungtsiang.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fyl.epnwcf.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://aku.pycfn.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ofb.fzhhl.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qyp.wangshuangyany.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iex.yvedp.cn

[L06] 解析响应为 JSON
来源：http://mmb.cheryme.top

Py:   resp.json()
来源：http://pfx.316326.xyz

PHP:  json_decode($body, true);
来源：http://yep.wangshuangyany.cn

JS:   await resp.json()
来源：http://wua.ivvv.top

TS:   await resp.json()
来源：http://upx.jyoumei.cn


<!-- 参考信息 -->