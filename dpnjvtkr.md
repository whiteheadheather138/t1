代发 wailian999

================================================================================
来源：http://ckn.hywenlv.cn

I. 正则表达式
来源：http://nmo.uphjek.com

================================================================================
来源：http://zqh.guowangkeji.top

[I01] 判断是否匹配
来源：http://pgy.yueranfly.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://azb.nanxinkj.top

PHP:  preg_match('/\d+/', $s);
来源：http://azf.birdmap.top

JS:   /\d+/.test(s)
来源：http://yqb.feifeiyinyue.top

TS:   /\d+/.test(s)
来源：http://mlj.cashguo.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ebt.haohaochexian.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vmz.epnwcf.com

Ruby: s.match?(/\d+/)
来源：http://arr.daria6918.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gfu.nwbrower.top

[I02] 提取所有匹配
来源：http://utq.52xcode.cn

Py:   re.findall(r"\d+", s)
来源：http://ttt.hongshengwenyu.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dvc.dashuyun.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mgs.ivvv.top

TS:   s.match(/\d+/g)
来源：http://uag.sjlbkw.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xnk.sxryk.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jdx.guowangkeji.top

Ruby: s.scan(/\d+/)
来源：http://tvx.xinyue.icu

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kvc.hammf.cn

[I03] 提取捕获分组
来源：http://ael.bbcook.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://suq.guowangkeji.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qwv.sufxvd.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sgj.xinyue.icu

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yds.jqgufenzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mvo.pengpengdd.cyou

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hey.pycfn.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gce.fzhhl.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zuj.sweek.top

[I04] 正则替换
来源：http://mky.cucudq.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://knj.yj20258888.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://afh.jianghu66.top

JS:   s.replace(/\d+/g, "#")
来源：http://ixd.tarul.cn

TS:   s.replace(/\d+/g, "#")
来源：http://oty.andypj.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://eiu.yanxiufei.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pfz.iojbl.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cmk.ydzc1.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mvu.ctjpmb.com

[I05] 按正则拆分
来源：http://jeg.zycfv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://pwg.cashguo.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dlu.andypj.xyz

JS:   s.split(/\s*,\s*/)
来源：http://ytu.meibo888.top

TS:   s.split(/\s*,\s*/)
来源：http://chw.iojbl.cn

Java: s.split("\\s*,\\s*")
来源：http://gvy.gotoacloud.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vag.sysykeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://msb.0kj1m.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mwx.ydjk.org.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rqy.xuetiantiany.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cpp.zdqjudy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lhm.hnxiangtu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uyy.ppjwa.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ghm.iojbl.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qvu.chenlongwang.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yzj.meibo888.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://soy.cashguo.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jks.316326.xyz

[I07] 忽略大小写与多行模式
来源：http://qgt.tanke756.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ysy.yanxiufei.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zzv.hesvh.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nhg.jinqigfzy.top

TS:   /error/gim
来源：http://pwb.zhiwuduotai.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uys.jqgfzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xct.sysykeji.top

Ruby: s.scan(/error/i)
来源：http://xlw.jinghuilouyu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://veg.c1oappe.top

[I08] 贪婪与非贪婪匹配
来源：http://fjr.bbcook.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://luq.fengsongda.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://azb.jlsjyb.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zpv.jinghuilouyu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ggb.shanyushiyangtech.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://wnk.shangyingyoupin.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fuu.yongpay.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ofy.andypj.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uwk.shanyushiyangkeji.top

================================================================================
来源：http://ute.yj20258888.top

J. 日期与时间
来源：http://mkq.nwbrower.top

================================================================================
来源：http://boy.zhongyouzk.top

[J01] 获取当前时间
来源：http://ien.cashguo.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ysc.fanxiaobao.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fsh.jqgufenzy.top

JS:   new Date();  Date.now()
来源：http://ydi.shanyushiyangkeji.top

TS:   new Date();  Date.now()
来源：http://zug.nwbrower.top

Java: LocalDateTime.now();  Instant.now()
来源：http://jxf.c1oappe.top

Go:   time.Now()
来源：http://yso.vqdsnc.cn

Ruby: Time.now
来源：http://cej.cheryme.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bvd.dianchejie.cn

[J02] 格式化输出
来源：http://mrk.tarul.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ssy.birdmap.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nez.hesvh.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gkq.snrcjt.cn

TS:   d.toISOString()
来源：http://tnj.sufxvd.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kvy.hnqzz.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vjq.jinqigfzy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qyp.havefunace.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jgk.0kj1m.cn

[J03] 字符串解析为日期
来源：http://dnp.jinghuilouyu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hgt.bjfxy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dbj.ppjwa.cn

JS:   new Date("2024-01-02")
来源：http://fmy.pengpengdd.cyou

TS:   new Date("2024-01-02")
来源：http://gis.cucudq.cn

Java: LocalDate.parse("2024-01-02")
来源：http://uym.hesvh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gbz.yvedp.cn

Ruby: Date.parse("2024-01-02")
来源：http://ovr.dashuyun.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wwm.ctjpmb.com

[J04] 时间戳与日期互转
来源：http://nlp.bjfxy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pte.ctjpmb.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mkv.cqqwz.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vbj.andypj.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://bje.uphjek.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mol.havefunace.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://afq.jianghu66.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wex.daxiang520.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kdw.aizwys.cn

[J05] 时间加减（加 7 天）
来源：http://zyz.sysykeji.top

Py:   now + timedelta(days=7)
来源：http://rry.jinqigufen.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ozr.aizwys.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lrj.0kj1m.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rsb.birdmap.top

Java: LocalDate.now().plusDays(7)
来源：http://yjc.pycfn.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wod.jiagoushi.top

Ruby: Time.now + 7 * 86400
来源：http://fnh.vehdjk.com

C#:   DateTime.Now.AddDays(7)
来源：http://cjr.hysaishi.cn

[J06] 计算两时间之差
来源：http://qvr.hysaishi.cn

Py:   (end - start).total_seconds()
来源：http://xqy.jinyuanbaomall.cn

PHP:  $end->diff($start)->days;
来源：http://lpy.zhoulong.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://clv.yongpay.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://osh.hysaishi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://kgt.ppjwa.cn

Go:   end.Sub(start).Hours()
来源：http://sgv.dashuyun.cn

Ruby: end - start                 # 返回秒数
来源：http://tzq.yueranfly.top

C#:   (end - start).TotalSeconds
来源：http://kvj.ivvv.top

[J07] 比较两个日期
来源：http://njk.pycfn.com

Py:   d1 < d2;  d1 == d2
来源：http://udb.ppjwa.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zlk.zycfv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bou.guowangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://hom.bbcook.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nry.ydzc1.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sou.quarkkingdee.top

Ruby: d1 < d2;  d1 == d2
来源：http://klu.hongshengwenyu.top

C#:   d1 < d2;  d1 == d2
来源：http://gom.gzhubu.top

[J08] 提取年月日与星期
来源：http://yhf.zdqjudy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xru.uphjek.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uyc.jinqigufen.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jzr.shangyingyoupin.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://drf.tarul.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://flk.sjlbkw.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qwq.jiagoushi.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gsu.svipenyu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ebv.316326.xyz

[J09] 时区处理
来源：http://szj.cqqwz.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://iin.yuanzhike.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kmq.daxiang520.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kee.nanxinkj.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lql.316326.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yds.fengsongda.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vdz.cucudq.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://uwp.xuetiantiany.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://znh.jyoumei.cn

[J10] 取今天 / 本月第一天
来源：http://crx.yvedp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://yaq.jinghuilouyu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ogk.jinghuilouyu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jlq.9152youxi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cwn.jyoumei.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ihw.hongshengwenyu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xnl.dashuyun.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fth.dianchejie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cxr.sxryk.cn

================================================================================
来源：http://zci.hywenlv.cn

K. JSON 与序列化
来源：http://umt.cashguo.top

================================================================================
来源：http://oru.yuanzhike.top

[K01] 对象转 JSON 字符串
来源：http://umn.iojbl.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kxy.shangyingyoupin.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fgx.hywenlv.cn

JS:   JSON.stringify(obj)
来源：http://ckw.epnwcf.com

TS:   JSON.stringify(obj)
来源：http://vsc.sxryk.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://byp.mhx1999.top

Go:   json.Marshal(obj)
来源：http://hap.andypj.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://pjt.smart0.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://olu.ydzc1.top

[K02] JSON 字符串转对象
来源：http://fpp.0kj1m.cn

Py:   json.loads(s)
来源：http://xsf.jinyuanbaomall.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ymf.xingfuxueyuan.xyz

JS:   JSON.parse(s)
来源：http://izd.yj202588.top

TS:   JSON.parse(s)
来源：http://igg.zhiwuduotai.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sgl.9152youxi.cn

Go:   json.Unmarshal(data, &v)
来源：http://orp.pycfn.com

Ruby: JSON.parse(s)
来源：http://gjt.sjlbkw.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yus.meibo888.top

[K03] JSON 美化输出（带缩进）
来源：http://jsa.zhijiandao.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jwo.zhixingplan.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jwp.gzhubu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://xcq.yj202588.top

TS:   JSON.stringify(obj, null, 2)
来源：http://rok.zdbjq.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yri.cashguo.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gik.guannengcc.top

Ruby: JSON.pretty_generate(obj)
来源：http://wsu.fanxiaobao.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zxy.dashuyun.cn

[K04] 读取 JSON 文件
来源：http://zyy.gotoacloud.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xun.jinqigfzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dtl.zhiwuduotai.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ovt.epnwcf.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://goj.haohaochexian.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tea.yueranfly.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xeu.0kj1m.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pbo.jinyuanbaomall.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://knu.sjlbkw.cn

[K05] 深拷贝对象
来源：http://zvv.c1oappe.top

Py:   copy.deepcopy(obj)
来源：http://wpx.xziqi.cn

PHP:  unserialize(serialize($obj));
来源：http://uxg.316326.xyz

JS:   structuredClone(obj)
来源：http://fnp.shzxlz.cn

TS:   structuredClone(obj)
来源：http://nvm.zhixingplan.top

Java: // 手写拷贝构造，或序列化往返
来源：http://wwt.meibo888.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bkc.shzxlz.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ift.wangshuangyany.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tpy.hesvh.cn

[K06] 解析 URL 查询串
来源：http://ene.jiagoushi.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hyi.zdbjq.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://syi.tianlin.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wui.jyoumei.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tji.316326.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mpd.tanke756.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://hba.hnxiangtu.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://src.yangfankeji.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://seu.fktsv.cn

[K07] 进制转换
来源：http://efd.tianlin.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://acf.svipenyu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nzk.xuanzx.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lqq.jinghuilouyu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ccj.ivvv.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://iux.ydzc1.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kdw.sysykeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tta.xuetiantiany.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jxv.vehdjk.com

[K08] 二进制序列化（非 JSON）
来源：http://yrt.havefunace.top

Py:   pickle.dumps(obj)
来源：http://hwq.chenlongwang.top

PHP:  serialize($obj);  unserialize($s);
来源：http://nbx.kuanghao11.cn

JS:   v8.serialize(obj)        // Node
来源：http://eaz.zhoulong.xyz

TS:   v8.serialize(obj)        // Node
来源：http://ofa.jinghuilouyu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bnv.epnwcf.com

Go:   encoding/gob
来源：http://pgk.yfazqb.com

Ruby: Marshal.dump(obj)
来源：http://cpr.fanxiaobao.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rkg.ctjpmb.com

================================================================================
来源：http://yrt.fzhhl.top

L. 网络请求
来源：http://lsn.ybcxt.top

================================================================================
来源：http://rjx.havefunace.top

[L01] 发送 GET 请求
来源：http://kox.gotoacloud.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gyw.gzhubu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jku.yuanzhike.top

JS:   await fetch(url)
来源：http://kyc.jiagoushi.top

TS:   await fetch(url)
来源：http://yrl.bjfxy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qfi.nanxinkj.top

Go:   resp, err := http.Get(url)
来源：http://bdq.pengpengdd.cyou

Ruby: Net::HTTP.get(URI(url))
来源：http://jkl.hysaishi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ozu.sysykeji.top

[L02] 发送 POST JSON
来源：http://bnv.ybcxt.top

Py:   requests.post(url, json={"a": 1})
来源：http://uxs.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hvw.shanyushiyangtech.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gij.mhx1999.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iam.pengpengdd.cyou

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://amt.jqgfzy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tor.ehwqpu.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://art.jiagoushi.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ddo.yj20258.top

[L03] 设置自定义请求头
来源：http://noq.yuxming.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ctu.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gba.mhx1999.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bau.chenlongwang.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yml.aizwys.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dsf.9152youxi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gnz.meibo888.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://poz.haohaochexian.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nbb.jinyuanbaomall.cn

[L04] 设置超时
来源：http://usi.yj202588.top

Py:   requests.get(url, timeout=5)
来源：http://vju.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://npf.havefunace.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hkz.guowangkeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://epz.jianghu66.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vxr.guowangkeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://acx.kuanghao11.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cui.ywan-chungtsiang.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sjj.vqdsnc.cn

[L05] 上传文件（multipart）
来源：http://gqp.zhijiandao.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ttu.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cyy.jinqigfzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vwq.tanke756.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://llk.yongpay.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rfx.guannengcc.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mwe.haohaochexian.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://iso.jqgfzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pdp.jqgfzy.top

[L06] 解析响应为 JSON
来源：http://eri.hnqzz.top

Py:   resp.json()
来源：http://uog.hesvh.cn

PHP:  json_decode($body, true);
来源：http://rhj.shangyingyoupin.top

JS:   await resp.json()
来源：http://dti.sysykeji.top

TS:   await resp.json()
来源：http://ifv.redwolf501.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ttd.fzhhl.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hlz.xingfuxueyuan.xyz

Ruby: JSON.parse(resp.body)
来源：http://jov.jqgufenzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jml.sxryk.cn


<!-- 参考信息 -->