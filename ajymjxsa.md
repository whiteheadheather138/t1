代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bjj.shuidangran.top

Go:   defer f.Close()
来源：http://lvj.vehdjk.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wax.quarkkingdee.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bwu.xingfuxueyuan.xyz

================================================================================
来源：http://dzz.hfpthk.cn

I. 正则表达式
来源：http://cth.jinghuilouyu.cn

================================================================================
来源：http://odp.hywenlv.cn

[I01] 判断是否匹配
来源：http://nge.sufxvd.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://maf.shuidangran.top

PHP:  preg_match('/\d+/', $s);
来源：http://xjd.epnwcf.com

JS:   /\d+/.test(s)
来源：http://dau.ivvv.top

TS:   /\d+/.test(s)
来源：http://iqq.zhongyouzk.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xlg.pengpengdd.cyou

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wzc.xylfe.cn

Ruby: s.match?(/\d+/)
来源：http://eon.ctjpmb.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hqr.jqgufenzy.top

[I02] 提取所有匹配
来源：http://rvj.vqdsnc.cn

Py:   re.findall(r"\d+", s)
来源：http://vta.sxryk.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zld.yongpay.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nly.hfpthk.cn

TS:   s.match(/\d+/g)
来源：http://odn.havefunace.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lay.c1oappe.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pxf.yj202588.top

Ruby: s.scan(/\d+/)
来源：http://pdo.shzxlz.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kzw.dianchejie.cn

[I03] 提取捕获分组
来源：http://hqs.xuetiantiany.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uui.fzhhl.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hoe.zhijiandao.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fyg.quarkkingdee.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://whn.fengsongda.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://atu.aibaodan.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://eol.dianchejie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jeo.tanke756.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yqq.zdbjq.cn

[I04] 正则替换
来源：http://lqp.zhongyouzk.top

Py:   re.sub(r"\d+", "#", s)
来源：http://upk.tanke756.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wog.dashuyun.cn

JS:   s.replace(/\d+/g, "#")
来源：http://rfp.redwolf501.top

TS:   s.replace(/\d+/g, "#")
来源：http://oji.hfpthk.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ufm.ybcxt.top

Go:   re.ReplaceAllString(s, "#")
来源：http://hiy.uphjek.com

Ruby: s.gsub(/\d+/, "#")
来源：http://hye.xuetiantiany.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dgq.c1oappe.top

[I05] 按正则拆分
来源：http://dvt.guowangkeji.top

Py:   re.split(r"\s*,\s*", s)
来源：http://iuw.0kj1m.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kda.cucudq.cn

JS:   s.split(/\s*,\s*/)
来源：http://ozv.jqgfzy.top

TS:   s.split(/\s*,\s*/)
来源：http://qfe.fanxiaobao.xyz

Java: s.split("\\s*,\\s*")
来源：http://vhc.shuidangran.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qpo.gogol.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pvq.yongpay.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bdw.jlsjyb.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mgi.ivvv.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kdb.shangyingyoupin.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jef.chenlongwang.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fhw.zycfv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ksp.wangshuangyany.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ydv.havefunace.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://oag.ivvv.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tdw.zhengqikj.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cxa.hfpthk.cn

[I07] 忽略大小写与多行模式
来源：http://rlx.jinyuanbaomall.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xyx.vehdjk.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nao.sufxvd.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rib.vehdjk.com

TS:   /error/gim
来源：http://ejp.gzhubu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://knu.ywan-chungtsiang.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lio.quarkkingdee.top

Ruby: s.scan(/error/i)
来源：http://tyw.iojbl.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kxk.cdnleiting.top

[I08] 贪婪与非贪婪匹配
来源：http://wkw.vehdjk.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uad.zhoulong.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yhm.tarul.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fdr.fanxiaobao.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uwt.316326.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://qjd.shanyushiyangtech.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yzk.uphjek.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gsl.hongshengwenyu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gbe.jqgfzy.top

================================================================================
来源：http://szu.wangdashe.top

J. 日期与时间
来源：http://luu.tarul.cn

================================================================================
来源：http://syc.xinyue.icu

[J01] 获取当前时间
来源：http://lvb.snrcjt.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://icp.vqdsnc.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hpn.jinqigufen.top

JS:   new Date();  Date.now()
来源：http://vsi.cqqwz.cn

TS:   new Date();  Date.now()
来源：http://fkd.gogol.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yhs.yfazqb.com

Go:   time.Now()
来源：http://max.havefunace.top

Ruby: Time.now
来源：http://zwl.jyoumei.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zje.yangfankeji.com

[J02] 格式化输出
来源：http://dgp.wangshuangyany.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://byg.fengsongda.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://szb.sufxvd.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gbk.jinyuanbaomall.cn

TS:   d.toISOString()
来源：http://xkg.zdqjudy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wje.dianchejie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://llt.zdqjudy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pnv.xziqi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://eds.zhongyouzk.top

[J03] 字符串解析为日期
来源：http://kgm.nwbrower.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wdy.chenjidiqi.icu

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ocb.hesvh.cn

JS:   new Date("2024-01-02")
来源：http://dey.sysykeji.top

TS:   new Date("2024-01-02")
来源：http://eik.tarul.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ilj.xylfe.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://irb.smart0.xyz

Ruby: Date.parse("2024-01-02")
来源：http://ikm.hammf.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jfw.tian-w.cn

[J04] 时间戳与日期互转
来源：http://lkq.yanxiufei.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qce.hnxiangtu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fsp.jinqigfzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uhu.gzhubu.top

TS:   Math.floor(Date.now() / 1000)
来源：http://kmw.yvedp.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ozj.yfazqb.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dws.shanyushiyangkeji.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fpn.jyoumei.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mty.epnwcf.com

[J05] 时间加减（加 7 天）
来源：http://cvi.yueranfly.top

Py:   now + timedelta(days=7)
来源：http://akh.guowangkeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://akt.ydjk.org.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rzf.sjlbkw.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qxd.zhoulong.xyz

Java: LocalDate.now().plusDays(7)
来源：http://tfc.xingfuxueyuan.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ixl.xuanzx.com

Ruby: Time.now + 7 * 86400
来源：http://jif.zycfv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bxt.yueranfly.top

[J06] 计算两时间之差
来源：http://tsf.feifeiyinyue.top

Py:   (end - start).total_seconds()
来源：http://xmn.nanxuanxn.top

PHP:  $end->diff($start)->days;
来源：http://wkn.shanyushiyangkeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qey.daria6918.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jzo.xylfe.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jpk.zhongyouzk.top

Go:   end.Sub(start).Hours()
来源：http://mkq.dashuyun.cn

Ruby: end - start                 # 返回秒数
来源：http://vlw.zhixingplan.top

C#:   (end - start).TotalSeconds
来源：http://wsn.pengpengdd.cyou

[J07] 比较两个日期
来源：http://axg.iojbl.cn

Py:   d1 < d2;  d1 == d2
来源：http://vpt.yuxming.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ngk.kuanghao11.cn

JS:   d1.getTime() < d2.getTime()
来源：http://abt.ydzc1.top

TS:   d1.getTime() < d2.getTime()
来源：http://qif.vqdsnc.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kpq.birdmap.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://enh.redwolf501.top

Ruby: d1 < d2;  d1 == d2
来源：http://grc.hammf.cn

C#:   d1 < d2;  d1 == d2
来源：http://vsq.tian-w.cn

[J08] 提取年月日与星期
来源：http://otw.fktsv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kpz.haohaochexian.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pgf.fktsv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xve.hfpthk.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cro.daria6918.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ftj.jlsjyb.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rmu.gogol.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fzv.0kj1m.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://efa.0kj1m.cn

[J09] 时区处理
来源：http://tzr.hysaishi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://oys.jinyuanbaomall.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://utu.hnqzz.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kux.ehwqpu.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kvh.kuanghao11.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hif.xuetiantiany.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ayn.sufxvd.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://oxs.wangshuangyany.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yft.ybcxt.top

[J10] 取今天 / 本月第一天
来源：http://tnr.shzxlz.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ndz.yj20258888.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yly.tarul.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rvs.wangshuangyany.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kmd.dashuyun.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://eok.hnxiangtu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vff.xuanzx.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wmn.yueranfly.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pha.daxiang520.top

================================================================================
来源：http://duf.xingfuxueyuan.xyz

K. JSON 与序列化
来源：http://wdd.guowangkeji.top

================================================================================
来源：http://uhx.nanxinkj.top

[K01] 对象转 JSON 字符串
来源：http://mpd.jianghu66.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jfr.zhongyouzk.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tou.yonumen.top

JS:   JSON.stringify(obj)
来源：http://gbm.cucudq.cn

TS:   JSON.stringify(obj)
来源：http://khn.nanxuanxn.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cll.epnwcf.com

Go:   json.Marshal(obj)
来源：http://dfd.hysaishi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://col.9152youxi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://aqv.nanxuanxn.top

[K02] JSON 字符串转对象
来源：http://mhy.sweek.top

Py:   json.loads(s)
来源：http://mrv.yuxming.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://oau.ppjwa.cn

JS:   JSON.parse(s)
来源：http://jtn.hcnkem.com

TS:   JSON.parse(s)
来源：http://quc.tianlin.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hca.kuanghao11.cn

Go:   json.Unmarshal(data, &v)
来源：http://jys.fzhhl.top

Ruby: JSON.parse(s)
来源：http://vjt.hammf.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hst.cucudq.cn

[K03] JSON 美化输出（带缩进）
来源：http://cai.aibaodan.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mfn.jqgufenzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://quv.yongpay.top

JS:   JSON.stringify(obj, null, 2)
来源：http://myx.nwbrower.top

TS:   JSON.stringify(obj, null, 2)
来源：http://mva.yfazqb.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ayi.cqqwz.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fin.snrcjt.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wbg.tianlin.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vhg.svipenyu.cn

[K04] 读取 JSON 文件
来源：http://ipa.c1oappe.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rop.bbcook.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kyj.ctjpmb.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jkh.aibaodan.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://upz.zycfv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yqc.hysaishi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fnp.chenlongwang.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ptf.xylfe.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gje.guowangkeji.top

[K05] 深拷贝对象
来源：http://tet.vehdjk.com

Py:   copy.deepcopy(obj)
来源：http://ldw.jlsjyb.cn

PHP:  unserialize(serialize($obj));
来源：http://adc.chenjidiqi.icu

JS:   structuredClone(obj)
来源：http://huy.zycfv.cn

TS:   structuredClone(obj)
来源：http://sok.shzxlz.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wni.zhaomingkeji.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ife.jinyuanbaomall.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oye.shangyingyoupin.top

C#:   // 序列化往返，或自定义 Clone
来源：http://nky.ywan-chungtsiang.top

[K06] 解析 URL 查询串
来源：http://oeg.zhengqikj.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kyr.andypj.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://siy.52xcode.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://doo.ywan-chungtsiang.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://keu.tarul.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ibs.pycfn.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://pli.shanyushiyangtech.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fkx.fktsv.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qxm.jianghu66.top

[K07] 进制转换
来源：http://jlq.wangshuangyany.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bvg.fehbvm.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rff.hfpthk.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kkr.ydzc1.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://apj.nwbrower.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ufj.svipenyu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hmy.svipenyu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://frl.jiagoushi.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gvu.daria6918.cn

[K08] 二进制序列化（非 JSON）
来源：http://ieu.xylfe.cn

Py:   pickle.dumps(obj)
来源：http://hkb.birdmap.top

PHP:  serialize($obj);  unserialize($s);
来源：http://spa.hfpthk.cn

JS:   v8.serialize(obj)        // Node
来源：http://qjl.zhoulong.xyz

TS:   v8.serialize(obj)        // Node
来源：http://pvj.hesvh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tur.xziqi.cn

Go:   encoding/gob
来源：http://znb.yongpay.top

Ruby: Marshal.dump(obj)
来源：http://bcm.haohaochexian.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kiy.shangyingyoupin.top

================================================================================
来源：http://uqa.daria6918.cn

L. 网络请求
来源：http://lxl.redwolf501.top

================================================================================
来源：http://sso.shanyushiyangtech.top

[L01] 发送 GET 请求
来源：http://glh.bjfxy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://opj.gogol.net.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dna.dianchejie.cn

JS:   await fetch(url)
来源：http://hvi.pycfn.com

TS:   await fetch(url)
来源：http://rin.hnxiangtu.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uxy.xinyue.icu

Go:   resp, err := http.Get(url)
来源：http://elp.zhixingplan.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ipe.tianlin.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jar.chenzaomai.com

[L02] 发送 POST JSON
来源：http://bqo.mhx1999.top

Py:   requests.post(url, json={"a": 1})
来源：http://ktw.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pwm.sufxvd.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pdu.hcnkem.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mlq.gotoacloud.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://onf.gaohongyu789.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jlk.fehbvm.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tgp.yuanzhike.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tdt.redwolf501.top

[L03] 设置自定义请求头
来源：http://lhw.snrcjt.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ahh.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fuj.wangshuangyany.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ydr.hnqzz.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rxm.meibo888.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qnm.xylfe.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wrd.chenlongwang.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sak.smart0.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cib.xuanzx.com

[L04] 设置超时
来源：http://gws.yuanzhike.top

Py:   requests.get(url, timeout=5)
来源：http://ltf.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ocn.xuetiantiany.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tph.ydzc1.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nlt.ivvv.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://suz.smart0.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ibm.xuetiantiany.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tam.epnwcf.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dff.zhixingplan.top

[L05] 上传文件（multipart）
来源：http://ynu.gaohongyu789.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://osz.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://itw.yanxiufei.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://skj.jiagoushi.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hax.hysaishi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wyv.ydjk.org.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nuv.sysykeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ukc.dianchejie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qhc.zhaomingkeji.xyz

[L06] 解析响应为 JSON
来源：http://jxt.yj20258.top

Py:   resp.json()
来源：http://pmo.redwolf501.top

PHP:  json_decode($body, true);
来源：http://ism.chenjidiqi.icu

JS:   await resp.json()
来源：http://yyq.jqgufenzy.top

TS:   await resp.json()
来源：http://hws.ppjwa.cn


<!-- 参考信息 -->