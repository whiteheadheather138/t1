代发 wailian999

JS:   class MyError extends Error {}
来源：http://xyf.jinqigfzy.top

TS:   class MyError extends Error {}
来源：http://zpr.andypj.xyz

Java: class MyException extends RuntimeException {}
来源：http://uco.zhaomingkeji.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://iuk.yonumen.top

Ruby: class MyError < StandardError; end
来源：http://yrf.xylfe.cn

C#:   class MyException : Exception {}
来源：http://ftt.gotoacloud.top

[H05] 捕获特定类型
来源：http://ojg.xuanzx.com

Py:   except ValueError as e:
来源：http://vbz.yongpay.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://brt.yanxiufei.cn

JS:   if (e instanceof TypeError) {}
来源：http://zqz.svipenyu.cn

TS:   if (e instanceof TypeError) {}
来源：http://vyq.snrcjt.cn

Java: catch (IOException | SQLException e) {}
来源：http://dql.gzhubu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ust.zhongyouzk.top

Ruby: rescue ArgumentError => e
来源：http://uot.xylfe.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yrw.nwbrower.top

[H06] 可选值 / 空值安全访问
来源：http://hto.vqdsnc.cn

Py:   value = d.get("k") or default
来源：http://vup.zycfv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://slv.52xcode.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rfs.jiagoushi.top

TS:   obj?.a?.b;  d ?? default
来源：http://lup.epnwcf.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ctq.jqgfzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://qkp.ppjwa.cn

Ruby: d&.dig(:a, :b)
来源：http://bts.fengsongda.top

C#:   obj?.A?.B ?? default
来源：http://oth.nwbrower.top

[H07] 断言
来源：http://svu.wangdashe.top

Py:   assert x > 0, "必须为正"
来源：http://lht.zhongyouzk.top

PHP:  assert($x > 0);
来源：http://wrp.xingfuxueyuan.xyz

JS:   console.assert(x > 0);
来源：http://ztk.pycfn.com

TS:   console.assert(x > 0);
来源：http://dnx.cheryme.top

Java: assert x > 0 : "必须为正";
来源：http://lly.vehdjk.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uge.jyoumei.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cfy.shzxlz.cn

C#:   Debug.Assert(x > 0);
来源：http://xhd.9152youxi.cn

[H08] 获取错误信息与堆栈
来源：http://erd.uphjek.com

Py:   str(e);  traceback.format_exc()
来源：http://nlj.feifeiyinyue.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mxi.ydjk.org.cn

JS:   e.message;  e.stack
来源：http://xqv.cheryme.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://hzu.quarkkingdee.top

Java: e.getMessage();  e.printStackTrace()
来源：http://tcl.c1oappe.top

Go:   err.Error()
来源：http://azj.hysaishi.cn

Ruby: e.message;  e.backtrace
来源：http://smj.chenzaomai.com

C#:   e.Message;  e.StackTrace
来源：http://hug.bjfxy.top

[H09] 带错误码的异常
来源：http://mbq.fanxiaobao.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://frw.jinghuilouyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hbq.xuanzx.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zdu.hammf.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://orx.nanxuanxn.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mso.xylfe.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vng.316326.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://qqw.yanxiufei.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ned.pengpengdd.cyou

[H10] 资源自动释放
来源：http://fkn.yuanzhike.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://zar.tanke756.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lht.gzhubu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ysl.meibo888.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://raw.tarul.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kqq.hfpthk.cn

Go:   defer f.Close()
来源：http://qlh.yj202588.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uko.jinghuilouyu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tac.chenzaomai.com

================================================================================
来源：http://plj.yj20258.top

I. 正则表达式
来源：http://wlh.xylfe.cn

================================================================================
来源：http://cvj.fehbvm.com

[I01] 判断是否匹配
来源：http://jxh.gogol.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://osm.yuanzhike.top

PHP:  preg_match('/\d+/', $s);
来源：http://qck.gogol.net.cn

JS:   /\d+/.test(s)
来源：http://uaq.c1oappe.top

TS:   /\d+/.test(s)
来源：http://lfb.9152youxi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jtf.xziqi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kbi.cqqwz.cn

Ruby: s.match?(/\d+/)
来源：http://jvs.yvedp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wlj.bbcook.cn

[I02] 提取所有匹配
来源：http://tfb.zycfv.cn

Py:   re.findall(r"\d+", s)
来源：http://cnx.aibaodan.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rod.jqgfzy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qri.hesvh.cn

TS:   s.match(/\d+/g)
来源：http://bzh.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ftv.dashuyun.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mhs.cdnleiting.top

Ruby: s.scan(/\d+/)
来源：http://bnz.aizwys.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://utc.wangshuangyany.cn

[I03] 提取捕获分组
来源：http://uop.fktsv.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://noq.nanxinkj.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ith.havefunace.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mcd.yfazqb.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ucy.fehbvm.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://unq.shanyushiyangtech.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zof.yueranfly.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mcc.jinghuilouyu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zfm.cheryme.top

[I04] 正则替换
来源：http://kmf.smart0.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://tmp.yfazqb.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fsy.bjfxy.top

JS:   s.replace(/\d+/g, "#")
来源：http://aih.yanxiufei.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hni.haohaochexian.top

Java: s.replaceAll("\\d+", "#")
来源：http://fjy.yj202588.top

Go:   re.ReplaceAllString(s, "#")
来源：http://lke.bbcook.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://son.mhx1999.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fnz.yuxming.cn

[I05] 按正则拆分
来源：http://tuk.zhengqikj.top

Py:   re.split(r"\s*,\s*", s)
来源：http://gtq.hfpthk.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vhn.ctjpmb.com

JS:   s.split(/\s*,\s*/)
来源：http://vdr.yuanzhike.top

TS:   s.split(/\s*,\s*/)
来源：http://fxf.zhaomingkeji.xyz

Java: s.split("\\s*,\\s*")
来源：http://lkr.yonumen.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qbx.hywenlv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ebx.quarkkingdee.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://aai.yueranfly.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nsz.yj20258.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pvj.xziqi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vtt.uphjek.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jgu.xziqi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jef.tanke756.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pxy.jinqigufen.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fkv.dashuyun.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hfn.tianlin.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wid.zhengqikj.top

[I07] 忽略大小写与多行模式
来源：http://jwa.zhixingplan.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fwm.sjlbkw.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jlc.zhijiandao.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oec.jiagoushi.top

TS:   /error/gim
来源：http://xpe.ydjk.org.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zvg.havefunace.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://diz.zhijiandao.cn

Ruby: s.scan(/error/i)
来源：http://vlm.sweek.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fjz.xuanzx.com

[I08] 贪婪与非贪婪匹配
来源：http://pqk.tanke756.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xho.fengsongda.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xtf.ppjwa.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kah.feifeiyinyue.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://inv.fktsv.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vyp.shangyingyoupin.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cft.316326.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ikf.shangyingyoupin.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ocv.haohaochexian.top

================================================================================
来源：http://ihu.jiagoushi.top

J. 日期与时间
来源：http://uwy.pengpengdd.cyou

================================================================================
来源：http://bka.chenlongwang.top

[J01] 获取当前时间
来源：http://tfn.gzhubu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://krr.hesvh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dtj.cdnleiting.top

JS:   new Date();  Date.now()
来源：http://dhp.vehdjk.com

TS:   new Date();  Date.now()
来源：http://bhy.fengsongda.top

Java: LocalDateTime.now();  Instant.now()
来源：http://vyw.zycfv.cn

Go:   time.Now()
来源：http://spz.ctjpmb.com

Ruby: Time.now
来源：http://gat.yangfankeji.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wrv.fktsv.cn

[J02] 格式化输出
来源：http://ttm.shanyushiyangtech.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jch.zhixingplan.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vme.haohaochexian.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://arw.chenjidiqi.icu

TS:   d.toISOString()
来源：http://hdk.ybcxt.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ggn.nwbrower.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hno.tianlin.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hln.mhx1999.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nml.tian-w.cn

[J03] 字符串解析为日期
来源：http://hky.zhixingplan.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://otx.shangyingyoupin.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://txy.xuanzx.com

JS:   new Date("2024-01-02")
来源：http://zag.zhixingplan.top

TS:   new Date("2024-01-02")
来源：http://qhr.wangdashe.top

Java: LocalDate.parse("2024-01-02")
来源：http://nry.snrcjt.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uus.9152youxi.cn

Ruby: Date.parse("2024-01-02")
来源：http://ukk.vqdsnc.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xts.cdnleiting.top

[J04] 时间戳与日期互转
来源：http://gta.yueranfly.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zrh.52xcode.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yus.52xcode.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://psd.haohaochexian.top

TS:   Math.floor(Date.now() / 1000)
来源：http://pcm.zhongyouzk.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ugj.zhengqikj.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cqj.guannengcc.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qkm.shangyingyoupin.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tbi.shanyushiyangtech.top

[J05] 时间加减（加 7 天）
来源：http://siw.hongshengwenyu.top

Py:   now + timedelta(days=7)
来源：http://hpm.feifeiyinyue.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://kgv.fehbvm.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nkz.zhijiandao.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qld.52xcode.cn

Java: LocalDate.now().plusDays(7)
来源：http://ovx.havefunace.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pit.cashguo.top

Ruby: Time.now + 7 * 86400
来源：http://jnv.pengpengdd.cyou

C#:   DateTime.Now.AddDays(7)
来源：http://qey.gotoacloud.top

[J06] 计算两时间之差
来源：http://mwu.vehdjk.com

Py:   (end - start).total_seconds()
来源：http://fnp.hfpthk.cn

PHP:  $end->diff($start)->days;
来源：http://fvc.jinyuanbaomall.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vse.svipenyu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dkn.yongpay.top

Java: Duration.between(start, end).toSeconds()
来源：http://lqt.hfpthk.cn

Go:   end.Sub(start).Hours()
来源：http://kzv.iojbl.cn

Ruby: end - start                 # 返回秒数
来源：http://wms.aibaodan.cn

C#:   (end - start).TotalSeconds
来源：http://vcs.redwolf501.top

[J07] 比较两个日期
来源：http://xnx.sufxvd.cn

Py:   d1 < d2;  d1 == d2
来源：http://sai.epnwcf.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://plf.jinqigufen.top

JS:   d1.getTime() < d2.getTime()
来源：http://cve.redwolf501.top

TS:   d1.getTime() < d2.getTime()
来源：http://ena.zhiwuduotai.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://owl.xinyue.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://aju.havefunace.top

Ruby: d1 < d2;  d1 == d2
来源：http://sub.hnqzz.top

C#:   d1 < d2;  d1 == d2
来源：http://dce.zhijiandao.cn

[J08] 提取年月日与星期
来源：http://tbz.gzhubu.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mqb.tian-w.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tvn.zhengqikj.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yjh.xuetiantiany.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vrf.ydzc1.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fgr.jqgufenzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fez.hesvh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://inx.meibo888.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kms.fengsongda.top

[J09] 时区处理
来源：http://pbl.bjfxy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nkn.ybcxt.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zhw.aizwys.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://exc.wangshuangyany.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mgk.ybcxt.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lsp.tian-w.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cuu.vehdjk.com

Ruby: Time.now.getlocal("+08:00")
来源：http://vxr.jinqigufen.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zde.hnqzz.top

[J10] 取今天 / 本月第一天
来源：http://mzl.shzxlz.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://dtd.gzhubu.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pfn.0kj1m.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://phu.gogol.net.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tti.aizwys.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ceo.jyoumei.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ncj.cdnleiting.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dzw.tianlin.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tzx.yfazqb.com

================================================================================
来源：http://hdv.shanyushiyangtech.top

K. JSON 与序列化
来源：http://ytq.havefunace.top

================================================================================
来源：http://jgx.sxryk.cn

[K01] 对象转 JSON 字符串
来源：http://ovl.c1oappe.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://grc.hywenlv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://alt.zhaomingkeji.xyz

JS:   JSON.stringify(obj)
来源：http://iwg.dianchejie.cn

TS:   JSON.stringify(obj)
来源：http://atj.aibaodan.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kdz.snrcjt.cn

Go:   json.Marshal(obj)
来源：http://lzk.zycfv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://voh.xziqi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vuc.pengpengdd.cyou

[K02] JSON 字符串转对象
来源：http://ywi.shanyushiyangkeji.top

Py:   json.loads(s)
来源：http://tnb.jinghuilouyu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dht.gaohongyu789.top

JS:   JSON.parse(s)
来源：http://gez.pycfn.com

TS:   JSON.parse(s)
来源：http://snl.zhixingplan.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uva.yuanzhike.top

Go:   json.Unmarshal(data, &v)
来源：http://nea.redwolf501.top

Ruby: JSON.parse(s)
来源：http://fcw.xuetiantiany.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gih.bbcook.cn

[K03] JSON 美化输出（带缩进）
来源：http://acn.0kj1m.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hen.zdbjq.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://avr.fzhhl.top

JS:   JSON.stringify(obj, null, 2)
来源：http://wky.hongshengwenyu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://pzk.shuidangran.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://imm.sufxvd.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sst.zhongyouzk.top

Ruby: JSON.pretty_generate(obj)
来源：http://pth.jyoumei.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dvt.yongpay.top

[K04] 读取 JSON 文件
来源：http://lju.xuanzx.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rdj.svipenyu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gyr.aizwys.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://opg.havefunace.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://igo.smart0.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kbp.fktsv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jqq.xingfuxueyuan.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://ycg.sjlbkw.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rzr.guowangkeji.top

[K05] 深拷贝对象
来源：http://afc.yj202588.top

Py:   copy.deepcopy(obj)
来源：http://dml.yuxming.cn

PHP:  unserialize(serialize($obj));
来源：http://ikw.shzxlz.cn

JS:   structuredClone(obj)
来源：http://mjb.bjfxy.top

TS:   structuredClone(obj)
来源：http://fiv.fanxiaobao.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://fsx.cucudq.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ybc.bjfxy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xvi.bbcook.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vsj.c1oappe.top

[K06] 解析 URL 查询串
来源：http://zji.epnwcf.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kle.uphjek.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sit.meibo888.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dea.sufxvd.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zar.jlsjyb.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vut.bjfxy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://clt.havefunace.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nfw.9152youxi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ram.fanxiaobao.xyz

[K07] 进制转换
来源：http://hud.svipenyu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vjo.yanxiufei.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wux.yonumen.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sri.yuanzhike.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://szc.havefunace.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gzd.cdnleiting.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nxc.shuidangran.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ozp.quarkkingdee.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dbm.vehdjk.com

[K08] 二进制序列化（非 JSON）
来源：http://tuu.52xcode.cn

Py:   pickle.dumps(obj)
来源：http://mhv.nanxuanxn.top

PHP:  serialize($obj);  unserialize($s);
来源：http://vrz.hywenlv.cn

JS:   v8.serialize(obj)        // Node
来源：http://iwc.tian-w.cn

TS:   v8.serialize(obj)        // Node
来源：http://baz.meibo888.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://key.andypj.xyz


<!-- 参考信息 -->