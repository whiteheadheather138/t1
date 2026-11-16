代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://ool.sjlbkw.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xgo.haohaochexian.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xwi.kuanghao11.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pzy.yueranfly.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ppd.cucudq.cn

Go:   defer f.Close()
来源：http://dfi.zhongyouzk.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://etz.sweek.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rgt.zhaomingkeji.xyz

================================================================================
来源：http://ejw.yueranfly.top

I. 正则表达式
来源：http://qtp.xingfuxueyuan.xyz

================================================================================
来源：http://swt.hesvh.cn

[I01] 判断是否匹配
来源：http://axj.cashguo.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jzt.hnqzz.top

PHP:  preg_match('/\d+/', $s);
来源：http://eeb.zhongyouzk.top

JS:   /\d+/.test(s)
来源：http://bpz.sxryk.cn

TS:   /\d+/.test(s)
来源：http://mbr.smart0.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vqq.iojbl.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ojx.shanyushiyangkeji.top

Ruby: s.match?(/\d+/)
来源：http://qsd.sweek.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xaj.yanxiufei.cn

[I02] 提取所有匹配
来源：http://kwb.zdqjudy.top

Py:   re.findall(r"\d+", s)
来源：http://jav.nanxuanxn.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://stl.52xcode.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://spe.yvedp.cn

TS:   s.match(/\d+/g)
来源：http://tsx.zycfv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://auo.jinqigfzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cdq.zycfv.cn

Ruby: s.scan(/\d+/)
来源：http://sat.xingfuxueyuan.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kfs.cucudq.cn

[I03] 提取捕获分组
来源：http://cum.mhx1999.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wwd.bjfxy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mme.kuanghao11.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://guo.hammf.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zcn.yfazqb.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sze.tianlin.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hoo.cashguo.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qjy.dashuyun.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xfz.jqgufenzy.top

[I04] 正则替换
来源：http://pjn.zhongyouzk.top

Py:   re.sub(r"\d+", "#", s)
来源：http://mbj.jinghuilouyu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pmr.dashuyun.cn

JS:   s.replace(/\d+/g, "#")
来源：http://eyt.zhiwuduotai.top

TS:   s.replace(/\d+/g, "#")
来源：http://zcf.sweek.top

Java: s.replaceAll("\\d+", "#")
来源：http://adg.cdnleiting.top

Go:   re.ReplaceAllString(s, "#")
来源：http://glq.yfazqb.com

Ruby: s.gsub(/\d+/, "#")
来源：http://ery.ivvv.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dvb.aibaodan.cn

[I05] 按正则拆分
来源：http://kqq.jinghuilouyu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://oko.jyoumei.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://msv.andypj.xyz

JS:   s.split(/\s*,\s*/)
来源：http://rpw.c1oappe.top

TS:   s.split(/\s*,\s*/)
来源：http://odv.hfpthk.cn

Java: s.split("\\s*,\\s*")
来源：http://ugf.jinqigfzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rhb.fengsongda.top

Ruby: s.split(/\s*,\s*/)
来源：http://oso.ivvv.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mcq.zhiwuduotai.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xle.hfpthk.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hhk.c1oappe.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://buh.sxryk.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://csi.feifeiyinyue.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cnn.316326.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://any.nanxinkj.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mja.jiagoushi.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://etf.chenjidiqi.icu

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lql.ydjk.org.cn

[I07] 忽略大小写与多行模式
来源：http://cpf.yj20258.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mwr.yanxiufei.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://clb.jyoumei.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://llb.hnqzz.top

TS:   /error/gim
来源：http://pvf.yj20258888.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kbn.dashuyun.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vws.yangfankeji.com

Ruby: s.scan(/error/i)
来源：http://hee.aibaodan.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lti.yvedp.cn

[I08] 贪婪与非贪婪匹配
来源：http://fcc.redwolf501.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vkr.zhaomingkeji.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ohk.quarkkingdee.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jve.snrcjt.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sgr.yongpay.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://xcs.dashuyun.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mxr.gzhubu.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pfs.epnwcf.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uea.sjlbkw.cn

================================================================================
来源：http://cmq.yongpay.top

J. 日期与时间
来源：http://lii.chenzaomai.com

================================================================================
来源：http://vii.shangyingyoupin.top

[J01] 获取当前时间
来源：http://mae.jinqigfzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://qys.wangshuangyany.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://enc.hesvh.cn

JS:   new Date();  Date.now()
来源：http://hww.shuidangran.top

TS:   new Date();  Date.now()
来源：http://hbf.epnwcf.com

Java: LocalDateTime.now();  Instant.now()
来源：http://dyp.zhijiandao.cn

Go:   time.Now()
来源：http://jle.gzhubu.top

Ruby: Time.now
来源：http://xku.yuxming.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://aul.redwolf501.top

[J02] 格式化输出
来源：http://tuq.gzhubu.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qpw.jinyuanbaomall.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dnd.yongpay.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rzn.hysaishi.cn

TS:   d.toISOString()
来源：http://bca.cdnleiting.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ixi.xingfuxueyuan.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ywk.redwolf501.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zev.hcnkem.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gnc.nanxinkj.top

[J03] 字符串解析为日期
来源：http://gjj.hnxiangtu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://soi.zdqjudy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kqc.jianghu66.top

JS:   new Date("2024-01-02")
来源：http://mpf.zhiwuduotai.top

TS:   new Date("2024-01-02")
来源：http://vlx.chenlongwang.top

Java: LocalDate.parse("2024-01-02")
来源：http://vjg.ppjwa.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dcx.chenzaomai.com

Ruby: Date.parse("2024-01-02")
来源：http://qtd.andypj.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tue.ydzc1.top

[J04] 时间戳与日期互转
来源：http://bby.cucudq.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ynf.jinqigfzy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lcl.chenlongwang.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vbn.nwbrower.top

TS:   Math.floor(Date.now() / 1000)
来源：http://yni.yj20258.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gws.ydjk.org.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://inc.jinyuanbaomall.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wuk.ehwqpu.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ifi.wangshuangyany.cn

[J05] 时间加减（加 7 天）
来源：http://mgd.pengpengdd.cyou

Py:   now + timedelta(days=7)
来源：http://ldc.birdmap.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://xfv.chenjidiqi.icu

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://neq.nanxinkj.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hyi.shuidangran.top

Java: LocalDate.now().plusDays(7)
来源：http://xln.yongpay.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mkf.jianghu66.top

Ruby: Time.now + 7 * 86400
来源：http://mfb.gotoacloud.top

C#:   DateTime.Now.AddDays(7)
来源：http://cua.jinghuilouyu.cn

[J06] 计算两时间之差
来源：http://iqr.ivvv.top

Py:   (end - start).total_seconds()
来源：http://cxg.zycfv.cn

PHP:  $end->diff($start)->days;
来源：http://hzb.smart0.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://raa.uphjek.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mlw.52xcode.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nju.jyoumei.cn

Go:   end.Sub(start).Hours()
来源：http://mbg.zdbjq.cn

Ruby: end - start                 # 返回秒数
来源：http://rho.jianghu66.top

C#:   (end - start).TotalSeconds
来源：http://znx.zhijiandao.cn

[J07] 比较两个日期
来源：http://zzn.hcnkem.com

Py:   d1 < d2;  d1 == d2
来源：http://wir.daria6918.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://boz.havefunace.top

JS:   d1.getTime() < d2.getTime()
来源：http://djz.fehbvm.com

TS:   d1.getTime() < d2.getTime()
来源：http://hbl.andypj.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://owl.snrcjt.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://iqy.sweek.top

Ruby: d1 < d2;  d1 == d2
来源：http://vmp.52xcode.cn

C#:   d1 < d2;  d1 == d2
来源：http://eon.xziqi.cn

[J08] 提取年月日与星期
来源：http://lyg.daria6918.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ukd.tarul.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mbw.cqqwz.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://npw.yuanzhike.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://scb.hysaishi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mmu.svipenyu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ppr.shangyingyoupin.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jin.shangyingyoupin.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wdy.0kj1m.cn

[J09] 时区处理
来源：http://amh.fanxiaobao.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://upa.dianchejie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gby.daria6918.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://piz.jinqigfzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zhp.shangyingyoupin.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vpf.zhengqikj.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xek.cdnleiting.top

Ruby: Time.now.getlocal("+08:00")
来源：http://kwa.dashuyun.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://phl.redwolf501.top

[J10] 取今天 / 本月第一天
来源：http://fri.jinyuanbaomall.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gbm.52xcode.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uat.sjlbkw.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rwv.pycfn.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ybt.bjfxy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kha.smart0.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yrs.bbcook.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://igu.ctjpmb.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://unf.tian-w.cn

================================================================================
来源：http://bbx.quarkkingdee.top

K. JSON 与序列化
来源：http://aaz.daxiang520.top

================================================================================
来源：http://mlg.aibaodan.cn

[K01] 对象转 JSON 字符串
来源：http://jdx.jlsjyb.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://iok.hfpthk.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hdb.xuanzx.com

JS:   JSON.stringify(obj)
来源：http://ifn.jianghu66.top

TS:   JSON.stringify(obj)
来源：http://jpn.vehdjk.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wkk.nwbrower.top

Go:   json.Marshal(obj)
来源：http://fer.xingfuxueyuan.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://gjg.jyoumei.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kft.birdmap.top

[K02] JSON 字符串转对象
来源：http://utg.pengpengdd.cyou

Py:   json.loads(s)
来源：http://lir.guannengcc.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lps.ybcxt.top

JS:   JSON.parse(s)
来源：http://jlu.zhiwuduotai.top

TS:   JSON.parse(s)
来源：http://fcp.fktsv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nfc.andypj.xyz

Go:   json.Unmarshal(data, &v)
来源：http://xzc.jinqigfzy.top

Ruby: JSON.parse(s)
来源：http://ghu.xinyue.icu

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://biy.daxiang520.top

[K03] JSON 美化输出（带缩进）
来源：http://yiz.epnwcf.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tiu.zdqjudy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nyw.chenzaomai.com

JS:   JSON.stringify(obj, null, 2)
来源：http://ifd.chenjidiqi.icu

TS:   JSON.stringify(obj, null, 2)
来源：http://qvx.nanxuanxn.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ivj.yanxiufei.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ojp.xingfuxueyuan.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://qac.quarkkingdee.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kwo.ydzc1.top

[K04] 读取 JSON 文件
来源：http://kzj.ctjpmb.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pvr.havefunace.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ncy.xuanzx.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cen.pycfn.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hxu.uphjek.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fac.0kj1m.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wlt.jyoumei.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://oyo.xuetiantiany.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sox.sysykeji.top

[K05] 深拷贝对象
来源：http://izu.hywenlv.cn

Py:   copy.deepcopy(obj)
来源：http://jqz.xinyue.icu

PHP:  unserialize(serialize($obj));
来源：http://elo.pycfn.com

JS:   structuredClone(obj)
来源：http://ehf.tian-w.cn

TS:   structuredClone(obj)
来源：http://coj.yvedp.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kju.shanyushiyangkeji.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://okg.birdmap.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hwl.xingfuxueyuan.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://pak.gaohongyu789.top

[K06] 解析 URL 查询串
来源：http://qat.zycfv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qll.zhaomingkeji.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qcy.shuidangran.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fry.shzxlz.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jvl.daxiang520.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zcc.cdnleiting.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://erw.hywenlv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zvy.xuetiantiany.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://byd.cdnleiting.top

[K07] 进制转换
来源：http://dgf.ppjwa.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://khi.sufxvd.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fbm.ctjpmb.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hdz.chenzaomai.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wih.aibaodan.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qfk.haohaochexian.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kby.jqgfzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://eyt.cashguo.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bng.dianchejie.cn

[K08] 二进制序列化（非 JSON）
来源：http://kew.sufxvd.cn

Py:   pickle.dumps(obj)
来源：http://ulo.dashuyun.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nkg.havefunace.top

JS:   v8.serialize(obj)        // Node
来源：http://nhh.xuanzx.com

TS:   v8.serialize(obj)        // Node
来源：http://lxa.jinghuilouyu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fwj.shanyushiyangtech.top

Go:   encoding/gob
来源：http://ega.havefunace.top

Ruby: Marshal.dump(obj)
来源：http://zwm.ydjk.org.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://iaf.fktsv.cn

================================================================================
来源：http://hzb.smart0.xyz

L. 网络请求
来源：http://aqn.c1oappe.top

================================================================================
来源：http://otj.nanxuanxn.top

[L01] 发送 GET 请求
来源：http://yui.yangfankeji.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mla.yj20258.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ltp.ivvv.top

JS:   await fetch(url)
来源：http://xhs.bjfxy.top

TS:   await fetch(url)
来源：http://vre.svipenyu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://awl.yvedp.cn

Go:   resp, err := http.Get(url)
来源：http://rfu.tarul.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dhy.yongpay.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://osc.ydzc1.top

[L02] 发送 POST JSON
来源：http://owj.chenzaomai.com

Py:   requests.post(url, json={"a": 1})
来源：http://auu.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vpa.redwolf501.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://muh.yvedp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ljl.xuetiantiany.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kix.zhaomingkeji.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ytc.hnxiangtu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zah.smart0.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zip.hnxiangtu.top

[L03] 设置自定义请求头
来源：http://esq.sjlbkw.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fgu.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fud.dianchejie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ptt.yanxiufei.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bvk.cqqwz.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ukq.ybcxt.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sme.zdbjq.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ixc.birdmap.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ram.aibaodan.cn

[L04] 设置超时
来源：http://hya.zdbjq.cn

Py:   requests.get(url, timeout=5)
来源：http://qww.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wdy.jinqigufen.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bfk.cucudq.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tja.guowangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hnn.gogol.net.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nsb.zhengqikj.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bbw.ydjk.org.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pjo.zycfv.cn

[L05] 上传文件（multipart）
来源：http://jaj.9152youxi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qxi.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vlv.ehwqpu.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pbv.chenjidiqi.icu

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yoq.sweek.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mes.fzhhl.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://iwr.gotoacloud.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gzw.xuetiantiany.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ego.svipenyu.cn

[L06] 解析响应为 JSON
来源：http://fcz.havefunace.top


<!-- 参考信息 -->