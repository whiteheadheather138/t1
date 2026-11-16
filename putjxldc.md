代发 wailian999

JS:   class MyError extends Error {}
来源：http://unq.yj20258.top

TS:   class MyError extends Error {}
来源：http://zgl.zhaomingkeji.xyz

Java: class MyException extends RuntimeException {}
来源：http://yrx.hnxiangtu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://abr.yfazqb.com

Ruby: class MyError < StandardError; end
来源：http://ofi.zhaomingkeji.xyz

C#:   class MyException : Exception {}
来源：http://ngi.xuetiantiany.cn

[H05] 捕获特定类型
来源：http://lyp.feifeiyinyue.top

Py:   except ValueError as e:
来源：http://kom.cheryme.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://irb.yongpay.top

JS:   if (e instanceof TypeError) {}
来源：http://qlt.hammf.cn

TS:   if (e instanceof TypeError) {}
来源：http://rjj.mhx1999.top

Java: catch (IOException | SQLException e) {}
来源：http://ajh.jyoumei.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ppk.zdbjq.cn

Ruby: rescue ArgumentError => e
来源：http://sro.kuanghao11.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sff.yj20258888.top

[H06] 可选值 / 空值安全访问
来源：http://xit.tian-w.cn

Py:   value = d.get("k") or default
来源：http://wbb.zhoulong.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://xpi.dianchejie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://yim.yonumen.top

TS:   obj?.a?.b;  d ?? default
来源：http://auu.zhaomingkeji.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ils.yongpay.top

Go:   if v, ok := m["k"]; ok { }
来源：http://zwr.yonumen.top

Ruby: d&.dig(:a, :b)
来源：http://bed.c1oappe.top

C#:   obj?.A?.B ?? default
来源：http://gam.hysaishi.cn

[H07] 断言
来源：http://day.yongpay.top

Py:   assert x > 0, "必须为正"
来源：http://lbz.zdbjq.cn

PHP:  assert($x > 0);
来源：http://zbx.cucudq.cn

JS:   console.assert(x > 0);
来源：http://kex.xylfe.cn

TS:   console.assert(x > 0);
来源：http://yaq.sjlbkw.cn

Java: assert x > 0 : "必须为正";
来源：http://qau.c1oappe.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ykz.52xcode.cn

Ruby: raise "必须为正" unless x > 0
来源：http://azk.pycfn.com

C#:   Debug.Assert(x > 0);
来源：http://cvt.ivvv.top

[H08] 获取错误信息与堆栈
来源：http://srs.uphjek.com

Py:   str(e);  traceback.format_exc()
来源：http://dwk.shuidangran.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cbo.aibaodan.cn

JS:   e.message;  e.stack
来源：http://uic.52xcode.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jje.tarul.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://lfk.zhengqikj.top

Go:   err.Error()
来源：http://hav.dashuyun.cn

Ruby: e.message;  e.backtrace
来源：http://mef.c1oappe.top

C#:   e.Message;  e.StackTrace
来源：http://mik.yuanzhike.top

[H09] 带错误码的异常
来源：http://tji.zhoulong.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://imb.ctjpmb.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://nzw.cucudq.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xob.xylfe.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sii.hammf.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://opf.tarul.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ckp.xziqi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fnj.uphjek.com

C#:   // 自定义异常类中加 Code 属性
来源：http://psz.zhiwuduotai.top

[H10] 资源自动释放
来源：http://qkc.fanxiaobao.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://awh.vqdsnc.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oqe.jlsjyb.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bxt.nwbrower.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vln.shuidangran.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://har.xylfe.cn

Go:   defer f.Close()
来源：http://cug.gotoacloud.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wiy.jianghu66.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ywk.mhx1999.top

================================================================================
来源：http://bgv.havefunace.top

I. 正则表达式
来源：http://yyr.hcnkem.com

================================================================================
来源：http://kxy.guannengcc.top

[I01] 判断是否匹配
来源：http://blv.pycfn.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lwb.uphjek.com

PHP:  preg_match('/\d+/', $s);
来源：http://sek.vehdjk.com

JS:   /\d+/.test(s)
来源：http://mxa.cqqwz.cn

TS:   /\d+/.test(s)
来源：http://rrc.pycfn.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ncu.tianlin.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lql.iojbl.cn

Ruby: s.match?(/\d+/)
来源：http://hku.yonumen.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xfx.feifeiyinyue.top

[I02] 提取所有匹配
来源：http://ygj.andypj.xyz

Py:   re.findall(r"\d+", s)
来源：http://jls.svipenyu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nzq.svipenyu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hli.snrcjt.cn

TS:   s.match(/\d+/g)
来源：http://ozk.zhongyouzk.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gfx.shanyushiyangtech.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sza.hfpthk.cn

Ruby: s.scan(/\d+/)
来源：http://uwq.quarkkingdee.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gvi.meibo888.top

[I03] 提取捕获分组
来源：http://efd.ppjwa.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kan.yj20258888.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://npa.bbcook.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vqi.jinyuanbaomall.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kyh.smart0.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zfl.hesvh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zbl.hysaishi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xln.cashguo.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mut.daxiang520.top

[I04] 正则替换
来源：http://euc.gaohongyu789.top

Py:   re.sub(r"\d+", "#", s)
来源：http://gtq.zhijiandao.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mir.sysykeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://apa.bbcook.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zri.nanxinkj.top

Java: s.replaceAll("\\d+", "#")
来源：http://vbo.ppjwa.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://asj.xylfe.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cvg.yj202588.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://upc.aibaodan.cn

[I05] 按正则拆分
来源：http://tvv.zhongyouzk.top

Py:   re.split(r"\s*,\s*", s)
来源：http://jpr.guannengcc.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://quv.zhoulong.xyz

JS:   s.split(/\s*,\s*/)
来源：http://ryl.xuanzx.com

TS:   s.split(/\s*,\s*/)
来源：http://owl.meibo888.top

Java: s.split("\\s*,\\s*")
来源：http://gfw.cqqwz.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wvy.jyoumei.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fck.xingfuxueyuan.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dbr.smart0.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ybc.cucudq.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yjt.xinyue.icu

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uqg.tianlin.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uoz.c1oappe.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ydt.smart0.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hmq.yanxiufei.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mpv.yangfankeji.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://oqo.yvedp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hwc.jyoumei.cn

[I07] 忽略大小写与多行模式
来源：http://rzr.zhoulong.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://byr.shangyingyoupin.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dkk.sysykeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pka.bbcook.cn

TS:   /error/gim
来源：http://lqn.yangfankeji.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kvf.quarkkingdee.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xwr.9152youxi.cn

Ruby: s.scan(/error/i)
来源：http://erc.cashguo.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ywf.jiagoushi.top

[I08] 贪婪与非贪婪匹配
来源：http://tcv.cheryme.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ucx.zdqjudy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gug.dianchejie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://izu.hesvh.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ysl.dianchejie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hki.smart0.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vof.smart0.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zti.redwolf501.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://maq.yuxming.cn

================================================================================
来源：http://rse.jyoumei.cn

J. 日期与时间
来源：http://flb.haohaochexian.top

================================================================================
来源：http://ibb.zdbjq.cn

[J01] 获取当前时间
来源：http://xnd.dashuyun.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lxk.sxryk.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nal.feifeiyinyue.top

JS:   new Date();  Date.now()
来源：http://smg.iojbl.cn

TS:   new Date();  Date.now()
来源：http://kzj.hongshengwenyu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://aaj.chenzaomai.com

Go:   time.Now()
来源：http://nvu.kuanghao11.cn

Ruby: Time.now
来源：http://gtw.fzhhl.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sng.andypj.xyz

[J02] 格式化输出
来源：http://vbz.hcnkem.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wce.birdmap.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cft.smart0.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nwu.shuidangran.top

TS:   d.toISOString()
来源：http://sos.xuetiantiany.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dcr.nanxuanxn.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://chb.smart0.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rfj.hnxiangtu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://iex.dashuyun.cn

[J03] 字符串解析为日期
来源：http://qto.zdbjq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mjd.epnwcf.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yfl.haohaochexian.top

JS:   new Date("2024-01-02")
来源：http://juv.zhiwuduotai.top

TS:   new Date("2024-01-02")
来源：http://ein.vqdsnc.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vjl.dashuyun.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qnj.mhx1999.top

Ruby: Date.parse("2024-01-02")
来源：http://vfh.fzhhl.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nss.xingfuxueyuan.xyz

[J04] 时间戳与日期互转
来源：http://hpl.hcnkem.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pfx.nanxuanxn.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yyg.0kj1m.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dsz.sjlbkw.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://nkz.iojbl.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qbn.mhx1999.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fuj.xziqi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jmr.yj20258888.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://egh.pengpengdd.cyou

[J05] 时间加减（加 7 天）
来源：http://svu.hnqzz.top

Py:   now + timedelta(days=7)
来源：http://rfm.redwolf501.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://lkb.xingfuxueyuan.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://epz.yfazqb.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sok.snrcjt.cn

Java: LocalDate.now().plusDays(7)
来源：http://oum.meibo888.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ena.chenlongwang.top

Ruby: Time.now + 7 * 86400
来源：http://rln.gaohongyu789.top

C#:   DateTime.Now.AddDays(7)
来源：http://ygt.dianchejie.cn

[J06] 计算两时间之差
来源：http://bdo.sysykeji.top

Py:   (end - start).total_seconds()
来源：http://ivy.hnqzz.top

PHP:  $end->diff($start)->days;
来源：http://tqp.chenzaomai.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://flx.jinqigufen.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vrb.xylfe.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fvf.gotoacloud.top

Go:   end.Sub(start).Hours()
来源：http://qnf.fzhhl.top

Ruby: end - start                 # 返回秒数
来源：http://ccc.tian-w.cn

C#:   (end - start).TotalSeconds
来源：http://azy.fengsongda.top

[J07] 比较两个日期
来源：http://urz.ppjwa.cn

Py:   d1 < d2;  d1 == d2
来源：http://qqu.feifeiyinyue.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uhx.hongshengwenyu.top

JS:   d1.getTime() < d2.getTime()
来源：http://ldx.fengsongda.top

TS:   d1.getTime() < d2.getTime()
来源：http://qhs.yfazqb.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pis.zhoulong.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sfy.tanke756.top

Ruby: d1 < d2;  d1 == d2
来源：http://hqo.aizwys.cn

C#:   d1 < d2;  d1 == d2
来源：http://een.fehbvm.com

[J08] 提取年月日与星期
来源：http://wid.tian-w.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nbo.zycfv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ayd.ywan-chungtsiang.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vrh.yj20258888.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wst.feifeiyinyue.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://num.redwolf501.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sif.sxryk.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://evv.zhoulong.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://idv.sufxvd.cn

[J09] 时区处理
来源：http://oib.yj202588.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nmh.kuanghao11.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nlo.svipenyu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nit.wangshuangyany.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rtp.bjfxy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yky.jinyuanbaomall.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qzr.tarul.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://bls.cqqwz.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hfr.nanxinkj.top

[J10] 取今天 / 本月第一天
来源：http://bzt.chenzaomai.com

Py:   date.today();  date.today().replace(day=1)
来源：http://mgx.xuetiantiany.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://roj.pycfn.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://eve.cucudq.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qrk.gzhubu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mlk.jinqigufen.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pmb.shanyushiyangtech.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dhl.zhongyouzk.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dgk.ydjk.org.cn

================================================================================
来源：http://pzy.chenlongwang.top

K. JSON 与序列化
来源：http://ifm.aibaodan.cn

================================================================================
来源：http://pqc.ydjk.org.cn

[K01] 对象转 JSON 字符串
来源：http://nhi.yfazqb.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://neb.jinyuanbaomall.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://sbc.bbcook.cn

JS:   JSON.stringify(obj)
来源：http://riz.cheryme.top

TS:   JSON.stringify(obj)
来源：http://exn.zhengqikj.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zfz.snrcjt.cn

Go:   json.Marshal(obj)
来源：http://uzm.hfpthk.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yrl.mhx1999.top

C#:   JsonSerializer.Serialize(obj)
来源：http://jqv.svipenyu.cn

[K02] JSON 字符串转对象
来源：http://lyr.pengpengdd.cyou

Py:   json.loads(s)
来源：http://uja.zdbjq.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fsr.yj202588.top

JS:   JSON.parse(s)
来源：http://guu.yonumen.top

TS:   JSON.parse(s)
来源：http://dlw.fehbvm.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xpq.daria6918.cn

Go:   json.Unmarshal(data, &v)
来源：http://kty.ivvv.top

Ruby: JSON.parse(s)
来源：http://zxq.jinqigufen.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nsm.jyoumei.cn

[K03] JSON 美化输出（带缩进）
来源：http://nkv.ybcxt.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ant.aibaodan.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gvn.yongpay.top

JS:   JSON.stringify(obj, null, 2)
来源：http://akb.xylfe.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://dup.mhx1999.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://piz.hnqzz.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://key.yfazqb.com

Ruby: JSON.pretty_generate(obj)
来源：http://zpr.cdnleiting.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jyi.ydzc1.top

[K04] 读取 JSON 文件
来源：http://ykf.chenlongwang.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cml.52xcode.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nen.andypj.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://owg.hesvh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://njm.haohaochexian.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ifc.havefunace.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ywj.tianlin.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://bjb.yj20258.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://byi.xylfe.cn

[K05] 深拷贝对象
来源：http://pum.ctjpmb.com

Py:   copy.deepcopy(obj)
来源：http://noy.zhengqikj.top

PHP:  unserialize(serialize($obj));
来源：http://rqr.jinqigfzy.top

JS:   structuredClone(obj)
来源：http://yrx.vqdsnc.cn

TS:   structuredClone(obj)
来源：http://cnp.0kj1m.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://din.gaohongyu789.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kpi.fzhhl.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rsl.c1oappe.top

C#:   // 序列化往返，或自定义 Clone
来源：http://axd.zhengqikj.top

[K06] 解析 URL 查询串
来源：http://ose.ydjk.org.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xsw.zycfv.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cct.sufxvd.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jno.xinyue.icu

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cha.sjlbkw.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://say.ctjpmb.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://qpm.bjfxy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dxk.jyoumei.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dnm.fehbvm.com

[K07] 进制转换
来源：http://iib.hongshengwenyu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ghh.aibaodan.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tvq.pycfn.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ona.cdnleiting.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dty.9152youxi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sya.fktsv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://epr.zhiwuduotai.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://emv.52xcode.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://els.9152youxi.cn

[K08] 二进制序列化（非 JSON）
来源：http://xjs.ybcxt.top

Py:   pickle.dumps(obj)
来源：http://fdz.pengpengdd.cyou

PHP:  serialize($obj);  unserialize($s);
来源：http://ula.kuanghao11.cn

JS:   v8.serialize(obj)        // Node
来源：http://eho.kuanghao11.cn

TS:   v8.serialize(obj)        // Node
来源：http://ool.cashguo.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xus.chenlongwang.top


<!-- 参考信息 -->