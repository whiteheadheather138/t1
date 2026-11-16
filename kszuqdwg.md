代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qrc.ehwqpu.com

Go:   if v, ok := m["k"]; ok { }
来源：http://qyu.redwolf501.top

Ruby: d&.dig(:a, :b)
来源：http://buo.zhiwuduotai.top

C#:   obj?.A?.B ?? default
来源：http://orv.sysykeji.top

[H07] 断言
来源：http://lns.shangyingyoupin.top

Py:   assert x > 0, "必须为正"
来源：http://ldf.hysaishi.cn

PHP:  assert($x > 0);
来源：http://caw.pengpengdd.cyou

JS:   console.assert(x > 0);
来源：http://yit.aibaodan.cn

TS:   console.assert(x > 0);
来源：http://yoj.xylfe.cn

Java: assert x > 0 : "必须为正";
来源：http://mnh.316326.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://poe.zhoulong.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://lka.kuanghao11.cn

C#:   Debug.Assert(x > 0);
来源：http://wcz.xylfe.cn

[H08] 获取错误信息与堆栈
来源：http://brq.redwolf501.top

Py:   str(e);  traceback.format_exc()
来源：http://prn.wangshuangyany.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oey.jinghuilouyu.cn

JS:   e.message;  e.stack
来源：http://zne.chenjidiqi.icu

TS:   e instanceof Error ? e.message : String(e)
来源：http://avf.shuidangran.top

Java: e.getMessage();  e.printStackTrace()
来源：http://zxd.haohaochexian.top

Go:   err.Error()
来源：http://cju.sysykeji.top

Ruby: e.message;  e.backtrace
来源：http://caa.pengpengdd.cyou

C#:   e.Message;  e.StackTrace
来源：http://kjb.zhengqikj.top

[H09] 带错误码的异常
来源：http://sps.yueranfly.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xtb.meibo888.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://pwb.vqdsnc.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sjn.pycfn.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://smb.yj20258888.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xxa.ivvv.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://psx.chenlongwang.top

Ruby: raise MyError.new("fail", 500)
来源：http://rcs.sufxvd.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://kio.yangfankeji.com

[H10] 资源自动释放
来源：http://afy.tian-w.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ufp.hammf.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://erb.pengpengdd.cyou

JS:   // 无 with：在 finally 里关闭句柄
来源：http://joz.zhaomingkeji.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cmm.iojbl.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://erc.zhaomingkeji.xyz

Go:   defer f.Close()
来源：http://aww.pycfn.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jhw.ywan-chungtsiang.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nuc.jqgufenzy.top

================================================================================
来源：http://seb.iojbl.cn

I. 正则表达式
来源：http://zae.yanxiufei.cn

================================================================================
来源：http://hjp.hcnkem.com

[I01] 判断是否匹配
来源：http://iqy.yfazqb.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hsd.tian-w.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jab.aizwys.cn

JS:   /\d+/.test(s)
来源：http://ijt.shanyushiyangtech.top

TS:   /\d+/.test(s)
来源：http://bie.xingfuxueyuan.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zsh.cucudq.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pct.ywan-chungtsiang.top

Ruby: s.match?(/\d+/)
来源：http://ruk.shzxlz.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zrn.ydzc1.top

[I02] 提取所有匹配
来源：http://qmq.jinqigfzy.top

Py:   re.findall(r"\d+", s)
来源：http://ppa.jiagoushi.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gye.sufxvd.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rvo.zycfv.cn

TS:   s.match(/\d+/g)
来源：http://ihx.uphjek.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mea.jinqigfzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://iga.chenzaomai.com

Ruby: s.scan(/\d+/)
来源：http://ain.zhixingplan.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kng.epnwcf.com

[I03] 提取捕获分组
来源：http://lqk.haohaochexian.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hbf.zhongyouzk.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mlo.kuanghao11.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xai.ydjk.org.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ciu.hfpthk.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://stb.cashguo.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hym.yueranfly.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://eey.xinyue.icu

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jqb.wangdashe.top

[I04] 正则替换
来源：http://uqz.chenzaomai.com

Py:   re.sub(r"\d+", "#", s)
来源：http://lct.ivvv.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rmw.zhiwuduotai.top

JS:   s.replace(/\d+/g, "#")
来源：http://qdk.fanxiaobao.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://nob.cucudq.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ufs.gogol.net.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xrt.haohaochexian.top

Ruby: s.gsub(/\d+/, "#")
来源：http://azv.ybcxt.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pnh.vehdjk.com

[I05] 按正则拆分
来源：http://cca.jyoumei.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xsi.jlsjyb.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ugc.yuanzhike.top

JS:   s.split(/\s*,\s*/)
来源：http://pqa.daxiang520.top

TS:   s.split(/\s*,\s*/)
来源：http://wkl.haohaochexian.top

Java: s.split("\\s*,\\s*")
来源：http://dya.gogol.net.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ojm.wangshuangyany.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pim.nanxuanxn.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dkr.jlsjyb.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uxj.yvedp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://raa.gotoacloud.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fnk.gaohongyu789.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sew.zdbjq.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ovg.9152youxi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ofu.fehbvm.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vpx.sweek.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wlp.ydjk.org.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vlf.dashuyun.cn

[I07] 忽略大小写与多行模式
来源：http://rno.fzhhl.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gng.pycfn.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jry.ctjpmb.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lls.epnwcf.com

TS:   /error/gim
来源：http://bph.yonumen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lot.yanxiufei.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://etk.nanxinkj.top

Ruby: s.scan(/error/i)
来源：http://toi.havefunace.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xfw.yangfankeji.com

[I08] 贪婪与非贪婪匹配
来源：http://cbk.gotoacloud.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kmu.aibaodan.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rbz.haohaochexian.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ndz.xuanzx.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://boe.havefunace.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://wip.hcnkem.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hqi.fzhhl.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vhj.sjlbkw.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://umm.jlsjyb.cn

================================================================================
来源：http://uwy.jinyuanbaomall.cn

J. 日期与时间
来源：http://bis.zhijiandao.cn

================================================================================
来源：http://ytx.fehbvm.com

[J01] 获取当前时间
来源：http://fvu.jlsjyb.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://oah.jinyuanbaomall.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lpu.cucudq.cn

JS:   new Date();  Date.now()
来源：http://qba.yuxming.cn

TS:   new Date();  Date.now()
来源：http://mss.yuanzhike.top

Java: LocalDateTime.now();  Instant.now()
来源：http://alf.pycfn.com

Go:   time.Now()
来源：http://kqr.xziqi.cn

Ruby: Time.now
来源：http://hwj.ctjpmb.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zww.zhengqikj.top

[J02] 格式化输出
来源：http://wdh.fzhhl.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://spa.gaohongyu789.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tvw.haohaochexian.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vqy.hongshengwenyu.top

TS:   d.toISOString()
来源：http://ctp.xuanzx.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://abx.chenjidiqi.icu

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hmr.shzxlz.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ylc.0kj1m.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cmg.jyoumei.cn

[J03] 字符串解析为日期
来源：http://rcr.fengsongda.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lwz.cdnleiting.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qpd.shanyushiyangkeji.top

JS:   new Date("2024-01-02")
来源：http://plg.cucudq.cn

TS:   new Date("2024-01-02")
来源：http://bvs.gzhubu.top

Java: LocalDate.parse("2024-01-02")
来源：http://yla.ctjpmb.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qsz.9152youxi.cn

Ruby: Date.parse("2024-01-02")
来源：http://lgh.daxiang520.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zfu.0kj1m.cn

[J04] 时间戳与日期互转
来源：http://lve.yj20258888.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tqs.jinqigfzy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sxa.tanke756.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://iew.yongpay.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jza.yj20258888.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gek.haohaochexian.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xbu.sxryk.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mpj.jyoumei.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wpb.gzhubu.top

[J05] 时间加减（加 7 天）
来源：http://idq.wangshuangyany.cn

Py:   now + timedelta(days=7)
来源：http://hch.uphjek.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://fdi.xuetiantiany.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kxm.yj202588.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mxx.meibo888.top

Java: LocalDate.now().plusDays(7)
来源：http://sgc.chenlongwang.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nms.dashuyun.cn

Ruby: Time.now + 7 * 86400
来源：http://ozt.ydjk.org.cn

C#:   DateTime.Now.AddDays(7)
来源：http://czi.jinqigufen.top

[J06] 计算两时间之差
来源：http://npw.hysaishi.cn

Py:   (end - start).total_seconds()
来源：http://fdl.yvedp.cn

PHP:  $end->diff($start)->days;
来源：http://jxm.ctjpmb.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xof.yonumen.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ivj.vqdsnc.cn

Java: Duration.between(start, end).toSeconds()
来源：http://aod.yfazqb.com

Go:   end.Sub(start).Hours()
来源：http://pgl.xylfe.cn

Ruby: end - start                 # 返回秒数
来源：http://max.mhx1999.top

C#:   (end - start).TotalSeconds
来源：http://mmo.wangdashe.top

[J07] 比较两个日期
来源：http://lqm.wangdashe.top

Py:   d1 < d2;  d1 == d2
来源：http://yqg.sufxvd.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hse.fzhhl.top

JS:   d1.getTime() < d2.getTime()
来源：http://fre.hongshengwenyu.top

TS:   d1.getTime() < d2.getTime()
来源：http://bht.daxiang520.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bjf.yueranfly.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nfl.shanyushiyangkeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://ibk.yonumen.top

C#:   d1 < d2;  d1 == d2
来源：http://stz.pycfn.com

[J08] 提取年月日与星期
来源：http://rcz.pengpengdd.cyou

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ayo.xziqi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fdx.tarul.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fmb.yj202588.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uay.jinyuanbaomall.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cgo.gotoacloud.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lwa.daxiang520.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kof.xylfe.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://esk.hfpthk.cn

[J09] 时区处理
来源：http://sca.quarkkingdee.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wbg.dashuyun.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rpw.jqgufenzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aml.sysykeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vse.nwbrower.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nkk.yvedp.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://and.gzhubu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://mky.uphjek.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hql.sufxvd.cn

[J10] 取今天 / 本月第一天
来源：http://yhc.meibo888.top

Py:   date.today();  date.today().replace(day=1)
来源：http://lyr.guowangkeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zac.jqgufenzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dgh.yfazqb.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kdl.havefunace.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lfb.wangshuangyany.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bsc.yj20258888.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uet.bjfxy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fou.sysykeji.top

================================================================================
来源：http://qna.jyoumei.cn

K. JSON 与序列化
来源：http://feg.shuidangran.top

================================================================================
来源：http://xkr.haohaochexian.top

[K01] 对象转 JSON 字符串
来源：http://tlu.yuanzhike.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ykx.andypj.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qsp.yj20258888.top

JS:   JSON.stringify(obj)
来源：http://njm.chenlongwang.top

TS:   JSON.stringify(obj)
来源：http://aba.chenzaomai.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://aqi.jianghu66.top

Go:   json.Marshal(obj)
来源：http://dtw.cdnleiting.top

Ruby: obj.to_json                                     // require "json"
来源：http://moa.zdqjudy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://drt.jlsjyb.cn

[K02] JSON 字符串转对象
来源：http://nha.yanxiufei.cn

Py:   json.loads(s)
来源：http://xcr.tian-w.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nig.hysaishi.cn

JS:   JSON.parse(s)
来源：http://hak.pycfn.com

TS:   JSON.parse(s)
来源：http://cku.gogol.net.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qnd.yanxiufei.cn

Go:   json.Unmarshal(data, &v)
来源：http://ejl.bbcook.cn

Ruby: JSON.parse(s)
来源：http://zhj.ehwqpu.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://opj.daxiang520.top

[K03] JSON 美化输出（带缩进）
来源：http://rjn.9152youxi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kro.shuidangran.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://aoo.epnwcf.com

JS:   JSON.stringify(obj, null, 2)
来源：http://plb.zhengqikj.top

TS:   JSON.stringify(obj, null, 2)
来源：http://iup.zhaomingkeji.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mov.havefunace.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wqa.yj202588.top

Ruby: JSON.pretty_generate(obj)
来源：http://odb.aibaodan.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hcw.fzhhl.top

[K04] 读取 JSON 文件
来源：http://wad.vehdjk.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zei.feifeiyinyue.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rzg.pengpengdd.cyou

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kvd.yangfankeji.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://htz.ctjpmb.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://eat.shangyingyoupin.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fub.ydzc1.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://buj.ydzc1.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ddi.9152youxi.cn

[K05] 深拷贝对象
来源：http://rdb.ydzc1.top

Py:   copy.deepcopy(obj)
来源：http://amq.dianchejie.cn

PHP:  unserialize(serialize($obj));
来源：http://pdi.yuanzhike.top

JS:   structuredClone(obj)
来源：http://oqv.hnqzz.top

TS:   structuredClone(obj)
来源：http://dbu.cashguo.top

Java: // 手写拷贝构造，或序列化往返
来源：http://exy.tarul.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gqz.kuanghao11.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sjy.mhx1999.top

C#:   // 序列化往返，或自定义 Clone
来源：http://kap.snrcjt.cn

[K06] 解析 URL 查询串
来源：http://ytu.xuetiantiany.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xsl.ydzc1.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://opi.cashguo.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ram.yfazqb.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yry.ywan-chungtsiang.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fbh.gotoacloud.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://xug.zdbjq.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://crk.tian-w.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://prf.yfazqb.com

[K07] 进制转换
来源：http://fmr.shzxlz.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mnb.cdnleiting.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dae.cdnleiting.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fkp.kuanghao11.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vtx.jqgfzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rwh.wangshuangyany.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wtb.aibaodan.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zbg.bbcook.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bvv.sjlbkw.cn

[K08] 二进制序列化（非 JSON）
来源：http://khi.jinqigfzy.top

Py:   pickle.dumps(obj)
来源：http://mgc.bjfxy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://rnt.shuidangran.top

JS:   v8.serialize(obj)        // Node
来源：http://ffx.jqgfzy.top

TS:   v8.serialize(obj)        // Node
来源：http://cqm.ydzc1.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yqo.cheryme.top

Go:   encoding/gob
来源：http://mrf.fehbvm.com

Ruby: Marshal.dump(obj)
来源：http://ivi.ywan-chungtsiang.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bcn.9152youxi.cn

================================================================================
来源：http://jzl.pycfn.com

L. 网络请求
来源：http://uts.bbcook.cn

================================================================================
来源：http://asd.xylfe.cn

[L01] 发送 GET 请求
来源：http://ecd.ydzc1.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nay.tian-w.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jxw.jinghuilouyu.cn

JS:   await fetch(url)
来源：http://brj.fehbvm.com

TS:   await fetch(url)
来源：http://zfs.gotoacloud.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qnx.ehwqpu.com

Go:   resp, err := http.Get(url)
来源：http://vav.c1oappe.top

Ruby: Net::HTTP.get(URI(url))
来源：http://qmp.cdnleiting.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yjx.hesvh.cn

[L02] 发送 POST JSON
来源：http://jtw.xziqi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mgf.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wvm.hnxiangtu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jty.yuanzhike.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ljh.sxryk.cn


<!-- 参考信息 -->