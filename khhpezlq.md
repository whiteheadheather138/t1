代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ahy.tanke756.top

Go:   if v, ok := m["k"]; ok { }
来源：http://nso.fanxiaobao.xyz

Ruby: d&.dig(:a, :b)
来源：http://scb.wangshuangyany.cn

C#:   obj?.A?.B ?? default
来源：http://wdr.shanyushiyangtech.top

[H07] 断言
来源：http://vbg.yueranfly.top

Py:   assert x > 0, "必须为正"
来源：http://hof.chenzaomai.com

PHP:  assert($x > 0);
来源：http://lef.zhaomingkeji.xyz

JS:   console.assert(x > 0);
来源：http://kss.haohaochexian.top

TS:   console.assert(x > 0);
来源：http://gjr.pycfn.com

Java: assert x > 0 : "必须为正";
来源：http://fnx.vqdsnc.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xpn.0kj1m.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bkd.cdnleiting.top

C#:   Debug.Assert(x > 0);
来源：http://all.pycfn.com

[H08] 获取错误信息与堆栈
来源：http://xer.chenzaomai.com

Py:   str(e);  traceback.format_exc()
来源：http://tpj.wangdashe.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bsc.hfpthk.cn

JS:   e.message;  e.stack
来源：http://auo.shanyushiyangkeji.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ljv.yj202588.top

Java: e.getMessage();  e.printStackTrace()
来源：http://xgp.gaohongyu789.top

Go:   err.Error()
来源：http://sqh.cucudq.cn

Ruby: e.message;  e.backtrace
来源：http://ssa.gotoacloud.top

C#:   e.Message;  e.StackTrace
来源：http://myo.sysykeji.top

[H09] 带错误码的异常
来源：http://syf.shangyingyoupin.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zuj.vehdjk.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://ihg.xylfe.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yph.yuxming.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ymk.ybcxt.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sko.gotoacloud.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tqi.andypj.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://ruh.ybcxt.top

C#:   // 自定义异常类中加 Code 属性
来源：http://qgg.fktsv.cn

[H10] 资源自动释放
来源：http://vvc.bbcook.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xxy.hysaishi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sdf.52xcode.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kef.zhengqikj.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tag.yangfankeji.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fgs.fzhhl.top

Go:   defer f.Close()
来源：http://ioo.shuidangran.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fdl.shzxlz.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lfp.gzhubu.top

================================================================================
来源：http://zzg.shangyingyoupin.top

I. 正则表达式
来源：http://xcm.zdbjq.cn

================================================================================
来源：http://vvx.fanxiaobao.xyz

[I01] 判断是否匹配
来源：http://qgm.yueranfly.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dxk.zhaomingkeji.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://fne.cucudq.cn

JS:   /\d+/.test(s)
来源：http://sbw.9152youxi.cn

TS:   /\d+/.test(s)
来源：http://qko.tarul.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zin.meibo888.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tkv.yfazqb.com

Ruby: s.match?(/\d+/)
来源：http://lpq.aibaodan.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bzo.jiagoushi.top

[I02] 提取所有匹配
来源：http://qoy.hcnkem.com

Py:   re.findall(r"\d+", s)
来源：http://fiq.fehbvm.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uss.yj20258888.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pbt.xingfuxueyuan.xyz

TS:   s.match(/\d+/g)
来源：http://crt.xinyue.icu

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gpa.epnwcf.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fyl.xuetiantiany.cn

Ruby: s.scan(/\d+/)
来源：http://dfu.cheryme.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://osj.sweek.top

[I03] 提取捕获分组
来源：http://qyk.nanxinkj.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uvj.ctjpmb.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ngc.yanxiufei.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fzl.zhaomingkeji.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kps.zdqjudy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://byh.c1oappe.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pmw.fanxiaobao.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kbf.hongshengwenyu.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ogo.zhoulong.xyz

[I04] 正则替换
来源：http://jap.zycfv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://esg.dashuyun.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://krq.tarul.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ucu.bjfxy.top

TS:   s.replace(/\d+/g, "#")
来源：http://mhb.gogol.net.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bac.zhixingplan.top

Go:   re.ReplaceAllString(s, "#")
来源：http://wac.zdqjudy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://axs.yj202588.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cup.9152youxi.cn

[I05] 按正则拆分
来源：http://tsr.cqqwz.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ajo.hysaishi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://amk.hnxiangtu.top

JS:   s.split(/\s*,\s*/)
来源：http://zhd.hammf.cn

TS:   s.split(/\s*,\s*/)
来源：http://vum.xuanzx.com

Java: s.split("\\s*,\\s*")
来源：http://nms.sxryk.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dii.epnwcf.com

Ruby: s.split(/\s*,\s*/)
来源：http://uul.cqqwz.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jah.ehwqpu.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xvz.ehwqpu.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fyv.jqgufenzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cgq.jyoumei.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sjb.hammf.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xrj.xylfe.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gzp.sweek.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hlk.daria6918.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xic.fktsv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ick.wangdashe.top

[I07] 忽略大小写与多行模式
来源：http://prh.yvedp.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pdx.ydjk.org.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://als.quarkkingdee.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ggt.ybcxt.top

TS:   /error/gim
来源：http://ynh.mhx1999.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qby.zhixingplan.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://igo.shzxlz.cn

Ruby: s.scan(/error/i)
来源：http://iwu.hfpthk.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gjp.jinghuilouyu.cn

[I08] 贪婪与非贪婪匹配
来源：http://een.gzhubu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xop.sweek.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ndp.wangshuangyany.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fvi.hnxiangtu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ffn.316326.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://uef.iojbl.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yrt.hysaishi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://utr.dianchejie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://siu.ydzc1.top

================================================================================
来源：http://hxu.wangshuangyany.cn

J. 日期与时间
来源：http://xtn.jlsjyb.cn

================================================================================
来源：http://xnl.ywan-chungtsiang.top

[J01] 获取当前时间
来源：http://ogu.fzhhl.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://xah.birdmap.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://aet.hnqzz.top

JS:   new Date();  Date.now()
来源：http://oto.shzxlz.cn

TS:   new Date();  Date.now()
来源：http://vrr.gotoacloud.top

Java: LocalDateTime.now();  Instant.now()
来源：http://klm.daria6918.cn

Go:   time.Now()
来源：http://cyx.bbcook.cn

Ruby: Time.now
来源：http://pbf.feifeiyinyue.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vxa.jyoumei.cn

[J02] 格式化输出
来源：http://rzg.yangfankeji.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dfd.yonumen.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jsx.gogol.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hhs.ywan-chungtsiang.top

TS:   d.toISOString()
来源：http://fkc.guowangkeji.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jad.xylfe.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jjt.jinqigfzy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yhd.vehdjk.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://efl.vqdsnc.cn

[J03] 字符串解析为日期
来源：http://pws.vqdsnc.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uan.sjlbkw.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fnc.snrcjt.cn

JS:   new Date("2024-01-02")
来源：http://pah.hongshengwenyu.top

TS:   new Date("2024-01-02")
来源：http://idg.jinyuanbaomall.cn

Java: LocalDate.parse("2024-01-02")
来源：http://obr.tarul.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mbl.redwolf501.top

Ruby: Date.parse("2024-01-02")
来源：http://nyg.kuanghao11.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mqy.tanke756.top

[J04] 时间戳与日期互转
来源：http://rtk.nanxinkj.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://txw.hysaishi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gxn.havefunace.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gff.sxryk.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qkz.jianghu66.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xwc.nanxuanxn.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gqh.hysaishi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ekm.hongshengwenyu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cqv.shzxlz.cn

[J05] 时间加减（加 7 天）
来源：http://uti.jlsjyb.cn

Py:   now + timedelta(days=7)
来源：http://mbn.jlsjyb.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://twi.xuanzx.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zeh.yj20258888.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://prs.havefunace.top

Java: LocalDate.now().plusDays(7)
来源：http://wcq.bbcook.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lks.haohaochexian.top

Ruby: Time.now + 7 * 86400
来源：http://gbg.redwolf501.top

C#:   DateTime.Now.AddDays(7)
来源：http://ujf.daxiang520.top

[J06] 计算两时间之差
来源：http://hvp.jinyuanbaomall.cn

Py:   (end - start).total_seconds()
来源：http://qmz.sysykeji.top

PHP:  $end->diff($start)->days;
来源：http://cfw.sysykeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ryn.shanyushiyangkeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tnt.yuxming.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jhc.cashguo.top

Go:   end.Sub(start).Hours()
来源：http://alf.havefunace.top

Ruby: end - start                 # 返回秒数
来源：http://cpe.yfazqb.com

C#:   (end - start).TotalSeconds
来源：http://apl.hcnkem.com

[J07] 比较两个日期
来源：http://dqr.epnwcf.com

Py:   d1 < d2;  d1 == d2
来源：http://gaf.chenjidiqi.icu

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hbz.wangshuangyany.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mlw.hcnkem.com

TS:   d1.getTime() < d2.getTime()
来源：http://spr.ppjwa.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hsz.iojbl.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://odj.aibaodan.cn

Ruby: d1 < d2;  d1 == d2
来源：http://tgv.jqgufenzy.top

C#:   d1 < d2;  d1 == d2
来源：http://tzb.tanke756.top

[J08] 提取年月日与星期
来源：http://yzk.vehdjk.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://onk.wangdashe.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pvy.shanyushiyangkeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pie.feifeiyinyue.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jqc.zhixingplan.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tfo.epnwcf.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zdu.zhiwuduotai.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zgd.chenzaomai.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://heh.tarul.cn

[J09] 时区处理
来源：http://mmw.sjlbkw.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://avn.birdmap.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://amd.sysykeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fos.birdmap.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fbb.zhaomingkeji.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dum.sweek.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mbw.jinqigfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://mfn.c1oappe.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zll.guannengcc.top

[J10] 取今天 / 本月第一天
来源：http://uxc.nanxinkj.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ycz.fktsv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://atb.meibo888.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ylm.yanxiufei.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mef.jqgufenzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://egg.kuanghao11.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ogz.nanxuanxn.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ttt.zhaomingkeji.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://avc.xinyue.icu

================================================================================
来源：http://tfs.yueranfly.top

K. JSON 与序列化
来源：http://gai.jinqigfzy.top

================================================================================
来源：http://lhd.sysykeji.top

[K01] 对象转 JSON 字符串
来源：http://yja.sxryk.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nll.dashuyun.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ukp.meibo888.top

JS:   JSON.stringify(obj)
来源：http://ope.fanxiaobao.xyz

TS:   JSON.stringify(obj)
来源：http://lua.uphjek.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jxr.ydzc1.top

Go:   json.Marshal(obj)
来源：http://hlu.zdqjudy.top

Ruby: obj.to_json                                     // require "json"
来源：http://bxw.xuetiantiany.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vnn.svipenyu.cn

[K02] JSON 字符串转对象
来源：http://wwz.hnxiangtu.top

Py:   json.loads(s)
来源：http://ffx.yueranfly.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://axx.yj20258888.top

JS:   JSON.parse(s)
来源：http://jyj.xinyue.icu

TS:   JSON.parse(s)
来源：http://cod.jqgfzy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cwk.feifeiyinyue.top

Go:   json.Unmarshal(data, &v)
来源：http://dvw.jinqigufen.top

Ruby: JSON.parse(s)
来源：http://qwy.hnqzz.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kcn.shzxlz.cn

[K03] JSON 美化输出（带缩进）
来源：http://dlc.cucudq.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cjy.jinqigufen.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ava.zhiwuduotai.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ipe.aibaodan.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mbb.fanxiaobao.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bja.gogol.net.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ght.shangyingyoupin.top

Ruby: JSON.pretty_generate(obj)
来源：http://ulk.aibaodan.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nry.chenlongwang.top

[K04] 读取 JSON 文件
来源：http://cft.bjfxy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sfs.yuanzhike.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ela.yj20258888.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hlq.birdmap.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sud.wangdashe.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ugp.jianghu66.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dnh.hfpthk.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://eqc.ctjpmb.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://owm.sysykeji.top

[K05] 深拷贝对象
来源：http://kyb.yj20258.top

Py:   copy.deepcopy(obj)
来源：http://hot.hysaishi.cn

PHP:  unserialize(serialize($obj));
来源：http://kym.zhongyouzk.top

JS:   structuredClone(obj)
来源：http://auk.pengpengdd.cyou

TS:   structuredClone(obj)
来源：http://jfg.nanxuanxn.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ajx.zhongyouzk.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bbr.gzhubu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lks.sxryk.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lgh.kuanghao11.cn

[K06] 解析 URL 查询串
来源：http://akt.yueranfly.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nxz.ydzc1.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://npc.0kj1m.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ihx.yvedp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lvb.xuanzx.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jsj.sweek.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://kjf.yueranfly.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://clw.jiagoushi.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nwy.chenlongwang.top

[K07] 进制转换
来源：http://xyp.dianchejie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nqu.pycfn.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ifu.yuanzhike.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://csm.uphjek.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jer.ybcxt.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://eyp.dianchejie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gyh.jianghu66.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pxu.316326.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qlp.0kj1m.cn

[K08] 二进制序列化（非 JSON）
来源：http://nsg.ivvv.top

Py:   pickle.dumps(obj)
来源：http://ixp.cucudq.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dsi.zhiwuduotai.top

JS:   v8.serialize(obj)        // Node
来源：http://xur.zdqjudy.top

TS:   v8.serialize(obj)        // Node
来源：http://fem.cqqwz.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://anh.fehbvm.com

Go:   encoding/gob
来源：http://nwu.sjlbkw.cn

Ruby: Marshal.dump(obj)
来源：http://tby.hnxiangtu.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kbf.shzxlz.cn

================================================================================
来源：http://lsm.cqqwz.cn

L. 网络请求
来源：http://vwx.zhijiandao.cn

================================================================================
来源：http://dzg.sxryk.cn

[L01] 发送 GET 请求
来源：http://ero.snrcjt.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fff.wangshuangyany.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cti.shzxlz.cn

JS:   await fetch(url)
来源：http://tih.xingfuxueyuan.xyz

TS:   await fetch(url)
来源：http://gwj.aizwys.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://twb.daxiang520.top

Go:   resp, err := http.Get(url)
来源：http://grx.fzhhl.top

Ruby: Net::HTTP.get(URI(url))
来源：http://hpi.redwolf501.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://geo.zdbjq.cn

[L02] 发送 POST JSON
来源：http://qqx.hnxiangtu.top

Py:   requests.post(url, json={"a": 1})
来源：http://qsm.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bos.jinghuilouyu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wzf.zdbjq.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pcs.yongpay.top


<!-- 参考信息 -->