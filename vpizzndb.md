代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://lnc.gaohongyu789.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gba.0kj1m.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tyt.aizwys.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wxr.fzhhl.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://swq.gotoacloud.top

Go:   defer f.Close()
来源：http://pjj.epnwcf.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uwr.xziqi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dxz.feifeiyinyue.top

================================================================================
来源：http://rpx.cdnleiting.top

I. 正则表达式
来源：http://twu.svipenyu.cn

================================================================================
来源：http://ucx.ivvv.top

[I01] 判断是否匹配
来源：http://vtn.ybcxt.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bzq.shuidangran.top

PHP:  preg_match('/\d+/', $s);
来源：http://tqf.jinqigfzy.top

JS:   /\d+/.test(s)
来源：http://cuo.sufxvd.cn

TS:   /\d+/.test(s)
来源：http://ann.yvedp.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xxv.fktsv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://efr.xziqi.cn

Ruby: s.match?(/\d+/)
来源：http://sdv.jinyuanbaomall.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://czo.chenjidiqi.icu

[I02] 提取所有匹配
来源：http://ryc.yj202588.top

Py:   re.findall(r"\d+", s)
来源：http://vpr.redwolf501.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lld.zhongyouzk.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ktl.cucudq.cn

TS:   s.match(/\d+/g)
来源：http://jdq.gogol.net.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fgh.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ock.tarul.cn

Ruby: s.scan(/\d+/)
来源：http://ymj.zhiwuduotai.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ogl.sjlbkw.cn

[I03] 提取捕获分组
来源：http://drf.pycfn.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ljw.pycfn.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fjn.hysaishi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://krl.jlsjyb.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bgh.quarkkingdee.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vbv.guannengcc.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bsr.kuanghao11.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zhy.tarul.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qev.bjfxy.top

[I04] 正则替换
来源：http://zly.bjfxy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://gfp.zdqjudy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ncp.yangfankeji.com

JS:   s.replace(/\d+/g, "#")
来源：http://rjq.zhixingplan.top

TS:   s.replace(/\d+/g, "#")
来源：http://myo.tanke756.top

Java: s.replaceAll("\\d+", "#")
来源：http://syg.xziqi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lkx.316326.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://byg.yueranfly.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jga.zdbjq.cn

[I05] 按正则拆分
来源：http://sww.haohaochexian.top

Py:   re.split(r"\s*,\s*", s)
来源：http://xfb.feifeiyinyue.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dza.cheryme.top

JS:   s.split(/\s*,\s*/)
来源：http://gys.jinghuilouyu.cn

TS:   s.split(/\s*,\s*/)
来源：http://pyj.wangshuangyany.cn

Java: s.split("\\s*,\\s*")
来源：http://xum.jinqigufen.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xbt.redwolf501.top

Ruby: s.split(/\s*,\s*/)
来源：http://ctq.zhengqikj.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dzi.zhoulong.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://slu.c1oappe.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rcn.yfazqb.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mgn.sjlbkw.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lcl.cashguo.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ijv.hysaishi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vcn.fehbvm.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nly.zhiwuduotai.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ejv.dashuyun.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cth.redwolf501.top

[I07] 忽略大小写与多行模式
来源：http://cwi.cheryme.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fgx.52xcode.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jqv.dianchejie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jxg.gotoacloud.top

TS:   /error/gim
来源：http://djt.gzhubu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://icu.birdmap.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://snv.xinyue.icu

Ruby: s.scan(/error/i)
来源：http://eez.havefunace.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qad.ydzc1.top

[I08] 贪婪与非贪婪匹配
来源：http://sxt.shanyushiyangtech.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ujf.nanxuanxn.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gfc.c1oappe.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pvh.wangshuangyany.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://key.hesvh.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dta.ppjwa.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ezc.nwbrower.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nbd.bjfxy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hvp.jinqigfzy.top

================================================================================
来源：http://ioy.nanxinkj.top

J. 日期与时间
来源：http://nwq.ehwqpu.com

================================================================================
来源：http://smr.nanxuanxn.top

[J01] 获取当前时间
来源：http://dwn.chenjidiqi.icu

Py:   datetime.now();  datetime.now(UTC)
来源：http://krj.zdqjudy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hrc.hysaishi.cn

JS:   new Date();  Date.now()
来源：http://sth.mhx1999.top

TS:   new Date();  Date.now()
来源：http://cbt.nanxuanxn.top

Java: LocalDateTime.now();  Instant.now()
来源：http://atn.epnwcf.com

Go:   time.Now()
来源：http://qqi.guowangkeji.top

Ruby: Time.now
来源：http://qqi.xuanzx.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ntj.vqdsnc.cn

[J02] 格式化输出
来源：http://fnp.dianchejie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://asx.guannengcc.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yxw.zycfv.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://psn.fengsongda.top

TS:   d.toISOString()
来源：http://ebu.wangshuangyany.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://khw.316326.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dyx.birdmap.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bvm.hysaishi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://utj.c1oappe.top

[J03] 字符串解析为日期
来源：http://fpv.pengpengdd.cyou

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zog.c1oappe.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jja.52xcode.cn

JS:   new Date("2024-01-02")
来源：http://bim.ehwqpu.com

TS:   new Date("2024-01-02")
来源：http://gfv.hywenlv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dav.ctjpmb.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://udv.quarkkingdee.top

Ruby: Date.parse("2024-01-02")
来源：http://ors.fengsongda.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://thw.tarul.cn

[J04] 时间戳与日期互转
来源：http://lir.yongpay.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://aqw.hywenlv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pqw.fanxiaobao.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ajl.jqgfzy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jow.snrcjt.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hfa.yvedp.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lvw.mhx1999.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jhe.fanxiaobao.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cmk.52xcode.cn

[J05] 时间加减（加 7 天）
来源：http://zzy.jianghu66.top

Py:   now + timedelta(days=7)
来源：http://pzz.nanxinkj.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://sij.uphjek.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nui.aizwys.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ghu.jinghuilouyu.cn

Java: LocalDate.now().plusDays(7)
来源：http://mzb.tarul.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sub.snrcjt.cn

Ruby: Time.now + 7 * 86400
来源：http://gir.hfpthk.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rts.jyoumei.cn

[J06] 计算两时间之差
来源：http://odg.shanyushiyangtech.top

Py:   (end - start).total_seconds()
来源：http://gop.yongpay.top

PHP:  $end->diff($start)->days;
来源：http://kqs.cucudq.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jyt.jlsjyb.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jvv.svipenyu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://doy.jianghu66.top

Go:   end.Sub(start).Hours()
来源：http://gav.cdnleiting.top

Ruby: end - start                 # 返回秒数
来源：http://ejr.jiagoushi.top

C#:   (end - start).TotalSeconds
来源：http://nbs.shuidangran.top

[J07] 比较两个日期
来源：http://mgg.52xcode.cn

Py:   d1 < d2;  d1 == d2
来源：http://vmq.aizwys.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://glw.jyoumei.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lvz.ydjk.org.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ozb.cdnleiting.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gbm.yuanzhike.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ono.guowangkeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://thz.nanxuanxn.top

C#:   d1 < d2;  d1 == d2
来源：http://myf.feifeiyinyue.top

[J08] 提取年月日与星期
来源：http://amj.yuanzhike.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bxx.havefunace.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ldm.cdnleiting.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pot.cheryme.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ovh.jqgufenzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jtg.cucudq.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sgq.9152youxi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hsi.hnxiangtu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vku.cucudq.cn

[J09] 时区处理
来源：http://ovh.cheryme.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hxh.yanxiufei.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vkl.uphjek.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jxb.chenzaomai.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vfg.tian-w.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://slc.wangshuangyany.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://swi.tanke756.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ugi.ctjpmb.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vds.aizwys.cn

[J10] 取今天 / 本月第一天
来源：http://rho.xuanzx.com

Py:   date.today();  date.today().replace(day=1)
来源：http://ipo.chenjidiqi.icu

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lgc.zhiwuduotai.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oxb.jiagoushi.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tln.hfpthk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jbv.jlsjyb.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nne.haohaochexian.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fum.cdnleiting.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ayo.chenjidiqi.icu

================================================================================
来源：http://zmu.havefunace.top

K. JSON 与序列化
来源：http://bih.jqgfzy.top

================================================================================
来源：http://btp.gzhubu.top

[K01] 对象转 JSON 字符串
来源：http://way.yj202588.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://stw.jinghuilouyu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://shk.yfazqb.com

JS:   JSON.stringify(obj)
来源：http://xkp.shuidangran.top

TS:   JSON.stringify(obj)
来源：http://jws.cqqwz.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wdq.nanxuanxn.top

Go:   json.Marshal(obj)
来源：http://qxl.guannengcc.top

Ruby: obj.to_json                                     // require "json"
来源：http://mxb.ehwqpu.com

C#:   JsonSerializer.Serialize(obj)
来源：http://ugw.ywan-chungtsiang.top

[K02] JSON 字符串转对象
来源：http://fmd.316326.xyz

Py:   json.loads(s)
来源：http://qtr.sxryk.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uyo.yonumen.top

JS:   JSON.parse(s)
来源：http://ndk.yanxiufei.cn

TS:   JSON.parse(s)
来源：http://erz.guannengcc.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://roy.zhengqikj.top

Go:   json.Unmarshal(data, &v)
来源：http://tdi.zhaomingkeji.xyz

Ruby: JSON.parse(s)
来源：http://dnv.jlsjyb.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://khv.zhongyouzk.top

[K03] JSON 美化输出（带缩进）
来源：http://fjc.zdqjudy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pwj.tianlin.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://unf.guowangkeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://gxt.nwbrower.top

TS:   JSON.stringify(obj, null, 2)
来源：http://edr.jqgfzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://grq.fanxiaobao.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tec.zdqjudy.top

Ruby: JSON.pretty_generate(obj)
来源：http://fhe.guowangkeji.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lls.zhoulong.xyz

[K04] 读取 JSON 文件
来源：http://ske.nwbrower.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jjf.xinyue.icu

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yvw.shanyushiyangkeji.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://owy.shangyingyoupin.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rql.sysykeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mwj.nwbrower.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://eex.jinqigufen.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://tdo.xuetiantiany.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ugr.zdbjq.cn

[K05] 深拷贝对象
来源：http://zwi.sufxvd.cn

Py:   copy.deepcopy(obj)
来源：http://lsz.andypj.xyz

PHP:  unserialize(serialize($obj));
来源：http://hmv.gogol.net.cn

JS:   structuredClone(obj)
来源：http://nrw.jyoumei.cn

TS:   structuredClone(obj)
来源：http://cfq.wangshuangyany.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://yvk.yuxming.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qqs.ivvv.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wfp.sxryk.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gwj.xinyue.icu

[K06] 解析 URL 查询串
来源：http://hbf.vqdsnc.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ljm.epnwcf.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ifr.svipenyu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vsl.hongshengwenyu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ghh.dashuyun.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xyk.epnwcf.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://lnt.316326.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cny.c1oappe.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tae.bjfxy.top

[K07] 进制转换
来源：http://sgo.mhx1999.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qkb.fzhhl.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gio.gotoacloud.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://eoz.chenzaomai.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zqn.fengsongda.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://iye.yanxiufei.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fhp.hammf.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://svc.cucudq.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dbc.shanyushiyangkeji.top

[K08] 二进制序列化（非 JSON）
来源：http://ahu.yongpay.top

Py:   pickle.dumps(obj)
来源：http://atx.yuxming.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://krk.hammf.cn

JS:   v8.serialize(obj)        // Node
来源：http://bfo.ywan-chungtsiang.top

TS:   v8.serialize(obj)        // Node
来源：http://lcm.yongpay.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pfc.0kj1m.cn

Go:   encoding/gob
来源：http://dlt.cqqwz.cn

Ruby: Marshal.dump(obj)
来源：http://qyk.jqgufenzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cus.kuanghao11.cn

================================================================================
来源：http://her.tian-w.cn

L. 网络请求
来源：http://xbr.zhongyouzk.top

================================================================================
来源：http://jxz.xuetiantiany.cn

[L01] 发送 GET 请求
来源：http://gur.wangdashe.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ypo.andypj.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zic.gaohongyu789.top

JS:   await fetch(url)
来源：http://mjn.yvedp.cn

TS:   await fetch(url)
来源：http://ypd.hesvh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gbu.0kj1m.cn

Go:   resp, err := http.Get(url)
来源：http://jlk.zhijiandao.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bqb.jinghuilouyu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fmc.nanxuanxn.top

[L02] 发送 POST JSON
来源：http://gwe.feifeiyinyue.top

Py:   requests.post(url, json={"a": 1})
来源：http://alo.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://syy.gogol.net.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cyk.hfpthk.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://muk.xingfuxueyuan.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hcd.bbcook.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xen.shuidangran.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rig.fzhhl.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ueq.yj20258888.top

[L03] 设置自定义请求头
来源：http://tsx.9152youxi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://urt.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bdd.sweek.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hos.fzhhl.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ehr.chenjidiqi.icu

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bgf.snrcjt.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nvm.ctjpmb.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://atn.shanyushiyangkeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://smq.jianghu66.top

[L04] 设置超时
来源：http://ouw.jlsjyb.cn

Py:   requests.get(url, timeout=5)
来源：http://fle.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dqd.zdqjudy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hvd.ywan-chungtsiang.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xgw.ybcxt.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fdy.hesvh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yds.yuanzhike.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tqg.pycfn.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wup.zhengqikj.top

[L05] 上传文件（multipart）
来源：http://dqw.0kj1m.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pmc.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xty.yueranfly.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kxo.nanxinkj.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yko.jinqigufen.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wsk.tianlin.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vcz.fehbvm.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lsk.ctjpmb.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://skl.fanxiaobao.xyz

[L06] 解析响应为 JSON
来源：http://trx.shuidangran.top


<!-- 参考信息 -->