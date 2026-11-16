代发 wailian999

TS:   console.assert(x > 0);
来源：http://jih.jinqigfzy.top

Java: assert x > 0 : "必须为正";
来源：http://wtq.hnxiangtu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qcl.yvedp.cn

Ruby: raise "必须为正" unless x > 0
来源：http://nji.zhengqikj.top

C#:   Debug.Assert(x > 0);
来源：http://xil.tian-w.cn

[H08] 获取错误信息与堆栈
来源：http://ldx.bjfxy.top

Py:   str(e);  traceback.format_exc()
来源：http://fve.zhaomingkeji.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ttn.zdqjudy.top

JS:   e.message;  e.stack
来源：http://giz.uphjek.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://zci.andypj.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://rym.hnqzz.top

Go:   err.Error()
来源：http://keh.jinghuilouyu.cn

Ruby: e.message;  e.backtrace
来源：http://pts.zdbjq.cn

C#:   e.Message;  e.StackTrace
来源：http://yfm.sxryk.cn

[H09] 带错误码的异常
来源：http://esg.vehdjk.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ydt.fktsv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hct.jqgfzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bjx.aibaodan.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wdt.xingfuxueyuan.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sls.pengpengdd.cyou

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ihh.yangfankeji.com

Ruby: raise MyError.new("fail", 500)
来源：http://hqw.kuanghao11.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hms.cucudq.cn

[H10] 资源自动释放
来源：http://lee.xingfuxueyuan.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://vqs.hongshengwenyu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ngo.iojbl.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xnf.nanxinkj.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://udw.ppjwa.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://omp.tianlin.xyz

Go:   defer f.Close()
来源：http://lge.yfazqb.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nxe.vehdjk.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://thd.sxryk.cn

================================================================================
来源：http://mjf.guowangkeji.top

I. 正则表达式
来源：http://dmj.yongpay.top

================================================================================
来源：http://zke.havefunace.top

[I01] 判断是否匹配
来源：http://tft.guowangkeji.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qmc.c1oappe.top

PHP:  preg_match('/\d+/', $s);
来源：http://tgf.xuetiantiany.cn

JS:   /\d+/.test(s)
来源：http://wot.yangfankeji.com

TS:   /\d+/.test(s)
来源：http://oxf.hammf.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zvg.shzxlz.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wuz.gotoacloud.top

Ruby: s.match?(/\d+/)
来源：http://rwm.gaohongyu789.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fda.yuxming.cn

[I02] 提取所有匹配
来源：http://bwt.hnxiangtu.top

Py:   re.findall(r"\d+", s)
来源：http://wsj.guowangkeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qbb.quarkkingdee.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ipl.feifeiyinyue.top

TS:   s.match(/\d+/g)
来源：http://kuh.cqqwz.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hrk.gotoacloud.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://oiq.dashuyun.cn

Ruby: s.scan(/\d+/)
来源：http://cks.hnxiangtu.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lme.jinghuilouyu.cn

[I03] 提取捕获分组
来源：http://vpg.sysykeji.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tle.c1oappe.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tsj.ywan-chungtsiang.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cbl.nwbrower.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rdy.daxiang520.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://foc.ywan-chungtsiang.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sul.fktsv.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wny.vehdjk.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mnc.aizwys.cn

[I04] 正则替换
来源：http://hsw.hcnkem.com

Py:   re.sub(r"\d+", "#", s)
来源：http://tpb.zhoulong.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mfm.wangshuangyany.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ian.nanxuanxn.top

TS:   s.replace(/\d+/g, "#")
来源：http://qbp.jqgfzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://miw.jinyuanbaomall.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://oss.gogol.net.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://dqr.zhixingplan.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://njh.mhx1999.top

[I05] 按正则拆分
来源：http://lor.shzxlz.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://jmo.zhiwuduotai.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://djr.jinghuilouyu.cn

JS:   s.split(/\s*,\s*/)
来源：http://dkz.yj202588.top

TS:   s.split(/\s*,\s*/)
来源：http://lhh.dashuyun.cn

Java: s.split("\\s*,\\s*")
来源：http://dzc.yj202588.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jri.quarkkingdee.top

Ruby: s.split(/\s*,\s*/)
来源：http://ejd.hesvh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sng.haohaochexian.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qqo.fengsongda.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lds.mhx1999.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fke.aibaodan.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://swm.fanxiaobao.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ery.pycfn.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yzh.ivvv.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ahy.ydjk.org.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ndj.cheryme.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gki.cqqwz.cn

[I07] 忽略大小写与多行模式
来源：http://giw.gaohongyu789.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pne.yvedp.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mmp.cheryme.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sjk.hysaishi.cn

TS:   /error/gim
来源：http://pew.ydjk.org.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fcz.ybcxt.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zwa.zhengqikj.top

Ruby: s.scan(/error/i)
来源：http://twz.tianlin.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jmu.hysaishi.cn

[I08] 贪婪与非贪婪匹配
来源：http://igx.shuidangran.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://plh.gaohongyu789.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xbz.hywenlv.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vmy.gogol.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fwo.yongpay.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://rdd.chenzaomai.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://map.daxiang520.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://npc.meibo888.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qyt.sysykeji.top

================================================================================
来源：http://vuw.sufxvd.cn

J. 日期与时间
来源：http://qjs.shuidangran.top

================================================================================
来源：http://bku.hammf.cn

[J01] 获取当前时间
来源：http://qwd.andypj.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://tev.fehbvm.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://atj.chenzaomai.com

JS:   new Date();  Date.now()
来源：http://nsc.hnxiangtu.top

TS:   new Date();  Date.now()
来源：http://aos.epnwcf.com

Java: LocalDateTime.now();  Instant.now()
来源：http://twk.mhx1999.top

Go:   time.Now()
来源：http://jll.nwbrower.top

Ruby: Time.now
来源：http://ock.pengpengdd.cyou

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yau.cheryme.top

[J02] 格式化输出
来源：http://lqf.haohaochexian.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lqv.yvedp.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qsf.tarul.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tjg.gogol.net.cn

TS:   d.toISOString()
来源：http://uzn.chenzaomai.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jhp.zhaomingkeji.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://eza.tarul.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qby.yuanzhike.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://eux.ydjk.org.cn

[J03] 字符串解析为日期
来源：http://xky.zhoulong.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jov.shuidangran.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tto.mhx1999.top

JS:   new Date("2024-01-02")
来源：http://peh.aizwys.cn

TS:   new Date("2024-01-02")
来源：http://tzs.gaohongyu789.top

Java: LocalDate.parse("2024-01-02")
来源：http://kjg.xingfuxueyuan.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zph.nanxinkj.top

Ruby: Date.parse("2024-01-02")
来源：http://xup.havefunace.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kee.gotoacloud.top

[J04] 时间戳与日期互转
来源：http://zfq.tian-w.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hrb.smart0.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bjl.fanxiaobao.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://khx.ydjk.org.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://chj.gogol.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://svv.dashuyun.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://voj.hammf.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zsr.birdmap.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://you.nanxuanxn.top

[J05] 时间加减（加 7 天）
来源：http://fye.cheryme.top

Py:   now + timedelta(days=7)
来源：http://swq.fengsongda.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://wdo.cashguo.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bao.ywan-chungtsiang.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bjl.dianchejie.cn

Java: LocalDate.now().plusDays(7)
来源：http://ehl.shangyingyoupin.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://eeb.hywenlv.cn

Ruby: Time.now + 7 * 86400
来源：http://oox.dianchejie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://afc.ybcxt.top

[J06] 计算两时间之差
来源：http://iut.ivvv.top

Py:   (end - start).total_seconds()
来源：http://jop.epnwcf.com

PHP:  $end->diff($start)->days;
来源：http://pdg.sufxvd.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qww.aizwys.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gsf.dashuyun.cn

Java: Duration.between(start, end).toSeconds()
来源：http://kjr.fanxiaobao.xyz

Go:   end.Sub(start).Hours()
来源：http://tcp.guannengcc.top

Ruby: end - start                 # 返回秒数
来源：http://dqy.shzxlz.cn

C#:   (end - start).TotalSeconds
来源：http://rga.gaohongyu789.top

[J07] 比较两个日期
来源：http://hmr.hysaishi.cn

Py:   d1 < d2;  d1 == d2
来源：http://gcc.zycfv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vvg.snrcjt.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mtx.jinyuanbaomall.cn

TS:   d1.getTime() < d2.getTime()
来源：http://frs.kuanghao11.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jhy.xziqi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://avu.vehdjk.com

Ruby: d1 < d2;  d1 == d2
来源：http://xln.dianchejie.cn

C#:   d1 < d2;  d1 == d2
来源：http://xah.iojbl.cn

[J08] 提取年月日与星期
来源：http://kbs.chenlongwang.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qtu.xuanzx.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://djn.svipenyu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://una.gzhubu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://svr.epnwcf.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://srt.hfpthk.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xjx.aizwys.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yfc.daria6918.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kvk.xylfe.cn

[J09] 时区处理
来源：http://bbs.ppjwa.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jhy.hongshengwenyu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fwb.yfazqb.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hhx.fktsv.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wmx.gzhubu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://asv.vqdsnc.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ajv.cucudq.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://saj.fktsv.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lfv.dianchejie.cn

[J10] 取今天 / 本月第一天
来源：http://rtq.fzhhl.top

Py:   date.today();  date.today().replace(day=1)
来源：http://cwh.fengsongda.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hli.gotoacloud.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mqf.epnwcf.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ubz.pycfn.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sae.gogol.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pfr.yj202588.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://peb.chenzaomai.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zel.sxryk.cn

================================================================================
来源：http://tga.cashguo.top

K. JSON 与序列化
来源：http://eri.jinyuanbaomall.cn

================================================================================
来源：http://lqb.yueranfly.top

[K01] 对象转 JSON 字符串
来源：http://yfx.mhx1999.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tyc.jinqigufen.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nap.guowangkeji.top

JS:   JSON.stringify(obj)
来源：http://lvl.chenlongwang.top

TS:   JSON.stringify(obj)
来源：http://jdf.smart0.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ofu.yj202588.top

Go:   json.Marshal(obj)
来源：http://rvt.jinyuanbaomall.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gdl.jyoumei.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lmn.wangdashe.top

[K02] JSON 字符串转对象
来源：http://our.sjlbkw.cn

Py:   json.loads(s)
来源：http://jmi.iojbl.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nur.iojbl.cn

JS:   JSON.parse(s)
来源：http://hkv.xuanzx.com

TS:   JSON.parse(s)
来源：http://rnv.cheryme.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ofu.wangdashe.top

Go:   json.Unmarshal(data, &v)
来源：http://uei.vehdjk.com

Ruby: JSON.parse(s)
来源：http://bge.svipenyu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ieo.zhongyouzk.top

[K03] JSON 美化输出（带缩进）
来源：http://tfs.sweek.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qvl.9152youxi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://svc.zhongyouzk.top

JS:   JSON.stringify(obj, null, 2)
来源：http://uly.gogol.net.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rux.jinyuanbaomall.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wcl.sjlbkw.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lcc.hfpthk.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rpp.tanke756.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rhh.tanke756.top

[K04] 读取 JSON 文件
来源：http://wkz.cheryme.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lbo.zdbjq.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hqd.sufxvd.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hmq.zhengqikj.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nta.zdqjudy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yuz.zycfv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zoj.bjfxy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://sba.xuetiantiany.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ndh.jyoumei.cn

[K05] 深拷贝对象
来源：http://neq.hammf.cn

Py:   copy.deepcopy(obj)
来源：http://qmy.feifeiyinyue.top

PHP:  unserialize(serialize($obj));
来源：http://dcm.316326.xyz

JS:   structuredClone(obj)
来源：http://orb.yonumen.top

TS:   structuredClone(obj)
来源：http://mdz.hfpthk.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zwu.cqqwz.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ujg.tarul.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wed.nanxuanxn.top

C#:   // 序列化往返，或自定义 Clone
来源：http://xyb.shzxlz.cn

[K06] 解析 URL 查询串
来源：http://fxb.aizwys.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jmg.pengpengdd.cyou

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gnj.nanxuanxn.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zwo.snrcjt.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://czp.hfpthk.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://iin.hywenlv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ozz.hysaishi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mtv.zhiwuduotai.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pkz.vqdsnc.cn

[K07] 进制转换
来源：http://lbt.xylfe.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ylk.guannengcc.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vxw.yj20258.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pno.yvedp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bif.ehwqpu.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mgx.jianghu66.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://eal.meibo888.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://khy.yj20258.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hvt.9152youxi.cn

[K08] 二进制序列化（非 JSON）
来源：http://ixy.zhijiandao.cn

Py:   pickle.dumps(obj)
来源：http://koz.zhengqikj.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ccf.sxryk.cn

JS:   v8.serialize(obj)        // Node
来源：http://myb.hfpthk.cn

TS:   v8.serialize(obj)        // Node
来源：http://owt.yangfankeji.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ami.ctjpmb.com

Go:   encoding/gob
来源：http://sch.yuanzhike.top

Ruby: Marshal.dump(obj)
来源：http://nih.cucudq.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hua.guowangkeji.top

================================================================================
来源：http://enq.yj20258.top

L. 网络请求
来源：http://lyk.dianchejie.cn

================================================================================
来源：http://qrn.daxiang520.top

[L01] 发送 GET 请求
来源：http://zon.hnxiangtu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hlk.uphjek.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dmv.hfpthk.cn

JS:   await fetch(url)
来源：http://fzu.hesvh.cn

TS:   await fetch(url)
来源：http://clw.birdmap.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://egn.tarul.cn

Go:   resp, err := http.Get(url)
来源：http://gdj.gotoacloud.top

Ruby: Net::HTTP.get(URI(url))
来源：http://wtq.svipenyu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uvk.pengpengdd.cyou

[L02] 发送 POST JSON
来源：http://gfb.zhoulong.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://rxz.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://oxj.jqgfzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xtt.bbcook.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ify.wangdashe.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fmo.chenzaomai.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zom.andypj.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cab.yj202588.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://azs.zhiwuduotai.top

[L03] 设置自定义请求头
来源：http://ros.shanyushiyangkeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://udl.jlsjyb.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hyk.vehdjk.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://agm.jiagoushi.top


<!-- 参考信息 -->