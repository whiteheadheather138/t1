代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://bdc.316326.xyz

[H04] 自定义异常类型
来源：http://ctu.haohaochexian.top

Py:   class MyError(Exception): pass
来源：http://uwr.ybcxt.top

PHP:  class MyError extends RuntimeException {}
来源：http://mpa.fzhhl.top

JS:   class MyError extends Error {}
来源：http://lws.xingfuxueyuan.xyz

TS:   class MyError extends Error {}
来源：http://rzy.iojbl.cn

Java: class MyException extends RuntimeException {}
来源：http://qng.zhaomingkeji.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yhb.hongshengwenyu.top

Ruby: class MyError < StandardError; end
来源：http://vua.jlsjyb.cn

C#:   class MyException : Exception {}
来源：http://qma.shanyushiyangkeji.top

[H05] 捕获特定类型
来源：http://dfo.yj20258.top

Py:   except ValueError as e:
来源：http://zgj.jianghu66.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xsk.yonumen.top

JS:   if (e instanceof TypeError) {}
来源：http://mnt.yj20258888.top

TS:   if (e instanceof TypeError) {}
来源：http://rfk.yangfankeji.com

Java: catch (IOException | SQLException e) {}
来源：http://nbn.dianchejie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blw.cucudq.cn

Ruby: rescue ArgumentError => e
来源：http://vlf.shzxlz.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cbq.hywenlv.cn

[H06] 可选值 / 空值安全访问
来源：http://djh.snrcjt.cn

Py:   value = d.get("k") or default
来源：http://sjg.hesvh.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pwv.snrcjt.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bto.ctjpmb.com

TS:   obj?.a?.b;  d ?? default
来源：http://zai.wangdashe.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://clm.pycfn.com

Go:   if v, ok := m["k"]; ok { }
来源：http://xtx.ydzc1.top

Ruby: d&.dig(:a, :b)
来源：http://msu.uphjek.com

C#:   obj?.A?.B ?? default
来源：http://sym.meibo888.top

[H07] 断言
来源：http://obt.yj20258888.top

Py:   assert x > 0, "必须为正"
来源：http://mjh.jinyuanbaomall.cn

PHP:  assert($x > 0);
来源：http://eid.daria6918.cn

JS:   console.assert(x > 0);
来源：http://akw.hnxiangtu.top

TS:   console.assert(x > 0);
来源：http://dbo.fengsongda.top

Java: assert x > 0 : "必须为正";
来源：http://qbd.yj20258888.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://utw.tarul.cn

Ruby: raise "必须为正" unless x > 0
来源：http://slc.cdnleiting.top

C#:   Debug.Assert(x > 0);
来源：http://tfj.ctjpmb.com

[H08] 获取错误信息与堆栈
来源：http://kxw.yj20258.top

Py:   str(e);  traceback.format_exc()
来源：http://mcm.yangfankeji.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ydk.xziqi.cn

JS:   e.message;  e.stack
来源：http://zjj.ppjwa.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://nwo.tanke756.top

Java: e.getMessage();  e.printStackTrace()
来源：http://llq.hfpthk.cn

Go:   err.Error()
来源：http://dpr.ppjwa.cn

Ruby: e.message;  e.backtrace
来源：http://mqy.nwbrower.top

C#:   e.Message;  e.StackTrace
来源：http://zdv.dashuyun.cn

[H09] 带错误码的异常
来源：http://uuq.ppjwa.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://faf.yanxiufei.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://afm.gogol.net.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://acx.xuetiantiany.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yvr.sxryk.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wfc.vqdsnc.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sym.316326.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://nmu.hnxiangtu.top

C#:   // 自定义异常类中加 Code 属性
来源：http://tcc.zhiwuduotai.top

[H10] 资源自动释放
来源：http://tik.ppjwa.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qjg.cdnleiting.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wjp.zycfv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://evq.iojbl.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lra.zhiwuduotai.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nbz.sufxvd.cn

Go:   defer f.Close()
来源：http://uew.0kj1m.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qus.zhijiandao.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fpd.zhengqikj.top

================================================================================
来源：http://ckd.yangfankeji.com

I. 正则表达式
来源：http://xmi.fengsongda.top

================================================================================
来源：http://hja.pycfn.com

[I01] 判断是否匹配
来源：http://lah.ctjpmb.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fax.uphjek.com

PHP:  preg_match('/\d+/', $s);
来源：http://ygc.tanke756.top

JS:   /\d+/.test(s)
来源：http://vbv.cqqwz.cn

TS:   /\d+/.test(s)
来源：http://lum.yj202588.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://exw.hnqzz.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://owu.jqgfzy.top

Ruby: s.match?(/\d+/)
来源：http://swe.vqdsnc.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yza.shzxlz.cn

[I02] 提取所有匹配
来源：http://wez.xuanzx.com

Py:   re.findall(r"\d+", s)
来源：http://vtz.hfpthk.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rey.xinyue.icu

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://prm.gotoacloud.top

TS:   s.match(/\d+/g)
来源：http://bhg.jinghuilouyu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uxw.smart0.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sco.bjfxy.top

Ruby: s.scan(/\d+/)
来源：http://hdl.dianchejie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ieh.ctjpmb.com

[I03] 提取捕获分组
来源：http://wcn.yuanzhike.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qmr.quarkkingdee.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ins.havefunace.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ilw.zdqjudy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wvq.pengpengdd.cyou

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ckw.jlsjyb.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zbn.jianghu66.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://oku.shanyushiyangkeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bpb.chenjidiqi.icu

[I04] 正则替换
来源：http://wkp.quarkkingdee.top

Py:   re.sub(r"\d+", "#", s)
来源：http://nmm.shuidangran.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pnq.zhoulong.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://iie.yuanzhike.top

TS:   s.replace(/\d+/g, "#")
来源：http://szc.c1oappe.top

Java: s.replaceAll("\\d+", "#")
来源：http://eue.fengsongda.top

Go:   re.ReplaceAllString(s, "#")
来源：http://eff.hammf.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ncg.hnqzz.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fou.zhengqikj.top

[I05] 按正则拆分
来源：http://wcr.tian-w.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ptb.ybcxt.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pmd.dianchejie.cn

JS:   s.split(/\s*,\s*/)
来源：http://hoq.nanxinkj.top

TS:   s.split(/\s*,\s*/)
来源：http://xgd.redwolf501.top

Java: s.split("\\s*,\\s*")
来源：http://smz.havefunace.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kvn.sysykeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://vya.bjfxy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ngf.guannengcc.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qzc.cashguo.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cez.guannengcc.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nsq.jinyuanbaomall.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rwb.guannengcc.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bha.wangshuangyany.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mqv.sweek.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://akg.yangfankeji.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gdk.bbcook.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cub.shanyushiyangtech.top

[I07] 忽略大小写与多行模式
来源：http://gfd.ehwqpu.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gok.ctjpmb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fbq.mhx1999.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xce.pengpengdd.cyou

TS:   /error/gim
来源：http://ikr.uphjek.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xyr.mhx1999.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://atq.fengsongda.top

Ruby: s.scan(/error/i)
来源：http://hew.hongshengwenyu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://snj.birdmap.top

[I08] 贪婪与非贪婪匹配
来源：http://aif.nwbrower.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qnz.bbcook.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rwd.daxiang520.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vke.shanyushiyangkeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mag.hesvh.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://esh.xylfe.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://phz.guannengcc.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vkr.fehbvm.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://saz.haohaochexian.top

================================================================================
来源：http://mji.yueranfly.top

J. 日期与时间
来源：http://ahz.jinyuanbaomall.cn

================================================================================
来源：http://ihs.jinghuilouyu.cn

[J01] 获取当前时间
来源：http://hea.zhoulong.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://jbi.316326.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ztv.yueranfly.top

JS:   new Date();  Date.now()
来源：http://zrt.bjfxy.top

TS:   new Date();  Date.now()
来源：http://hnb.ydjk.org.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://umq.shangyingyoupin.top

Go:   time.Now()
来源：http://qsc.vehdjk.com

Ruby: Time.now
来源：http://qyu.yonumen.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kfq.shzxlz.cn

[J02] 格式化输出
来源：http://sef.sxryk.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://swp.wangdashe.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qgo.fzhhl.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://krh.fzhhl.top

TS:   d.toISOString()
来源：http://waz.52xcode.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://epc.bbcook.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zak.pengpengdd.cyou

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tzq.ywan-chungtsiang.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yov.c1oappe.top

[J03] 字符串解析为日期
来源：http://vkb.zhongyouzk.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://her.iojbl.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bzi.xuetiantiany.cn

JS:   new Date("2024-01-02")
来源：http://kmx.hcnkem.com

TS:   new Date("2024-01-02")
来源：http://ane.sysykeji.top

Java: LocalDate.parse("2024-01-02")
来源：http://xva.zhengqikj.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lgf.pycfn.com

Ruby: Date.parse("2024-01-02")
来源：http://tln.shanyushiyangtech.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ypq.xingfuxueyuan.xyz

[J04] 时间戳与日期互转
来源：http://wza.wangshuangyany.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lwu.feifeiyinyue.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tzf.gzhubu.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nlh.yanxiufei.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wbj.zhengqikj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://feq.tanke756.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dia.52xcode.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ufv.yueranfly.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pmd.birdmap.top

[J05] 时间加减（加 7 天）
来源：http://oqc.yuanzhike.top

Py:   now + timedelta(days=7)
来源：http://fko.wangshuangyany.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jiq.tian-w.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://txu.zhaomingkeji.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uyb.cqqwz.cn

Java: LocalDate.now().plusDays(7)
来源：http://fre.yuxming.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://eoz.uphjek.com

Ruby: Time.now + 7 * 86400
来源：http://oqi.yuxming.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ngs.jinqigfzy.top

[J06] 计算两时间之差
来源：http://nvv.jqgfzy.top

Py:   (end - start).total_seconds()
来源：http://bvs.yueranfly.top

PHP:  $end->diff($start)->days;
来源：http://phr.jianghu66.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hdw.iojbl.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rne.shzxlz.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ngf.yfazqb.com

Go:   end.Sub(start).Hours()
来源：http://hkz.yanxiufei.cn

Ruby: end - start                 # 返回秒数
来源：http://neo.sjlbkw.cn

C#:   (end - start).TotalSeconds
来源：http://bdr.yj20258.top

[J07] 比较两个日期
来源：http://vcl.hfpthk.cn

Py:   d1 < d2;  d1 == d2
来源：http://ria.guannengcc.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mvo.zhaomingkeji.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://rim.yuxming.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ozg.ehwqpu.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uzn.wangdashe.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mws.cdnleiting.top

Ruby: d1 < d2;  d1 == d2
来源：http://mze.hesvh.cn

C#:   d1 < d2;  d1 == d2
来源：http://gqn.gotoacloud.top

[J08] 提取年月日与星期
来源：http://uli.jqgufenzy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://keq.sufxvd.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jac.yj202588.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kce.zhijiandao.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pli.fanxiaobao.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://leb.sxryk.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fuw.shanyushiyangkeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://iyv.sjlbkw.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nvu.gzhubu.top

[J09] 时区处理
来源：http://xyt.haohaochexian.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://eeg.zhaomingkeji.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lus.zdbjq.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lct.jyoumei.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kgt.ehwqpu.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zrx.ybcxt.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cnn.hesvh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://iwo.tarul.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vgu.bbcook.cn

[J10] 取今天 / 本月第一天
来源：http://xql.mhx1999.top

Py:   date.today();  date.today().replace(day=1)
来源：http://wnx.havefunace.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lud.andypj.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xqf.sxryk.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xwj.xuanzx.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vsm.c1oappe.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xza.xziqi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wwz.uphjek.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vwe.daxiang520.top

================================================================================
来源：http://ypj.xuanzx.com

K. JSON 与序列化
来源：http://sbt.guannengcc.top

================================================================================
来源：http://ghf.yangfankeji.com

[K01] 对象转 JSON 字符串
来源：http://vnl.zhixingplan.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ekb.hcnkem.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kna.jinyuanbaomall.cn

JS:   JSON.stringify(obj)
来源：http://bwb.sweek.top

TS:   JSON.stringify(obj)
来源：http://vcu.smart0.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lzj.xziqi.cn

Go:   json.Marshal(obj)
来源：http://rlz.xylfe.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zug.sweek.top

C#:   JsonSerializer.Serialize(obj)
来源：http://cnk.dianchejie.cn

[K02] JSON 字符串转对象
来源：http://qpf.iojbl.cn

Py:   json.loads(s)
来源：http://trw.sweek.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qic.gotoacloud.top

JS:   JSON.parse(s)
来源：http://eyv.snrcjt.cn

TS:   JSON.parse(s)
来源：http://wpj.sufxvd.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gwe.vehdjk.com

Go:   json.Unmarshal(data, &v)
来源：http://qtx.xylfe.cn

Ruby: JSON.parse(s)
来源：http://hkw.nanxinkj.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ida.sxryk.cn

[K03] JSON 美化输出（带缩进）
来源：http://wim.yuxming.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sbb.havefunace.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://acd.sysykeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://fpl.yfazqb.com

TS:   JSON.stringify(obj, null, 2)
来源：http://nnk.yanxiufei.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rlz.ctjpmb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://glt.sysykeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://iha.vehdjk.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nkg.uphjek.com

[K04] 读取 JSON 文件
来源：http://xai.svipenyu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tok.sjlbkw.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dwj.ivvv.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tpg.vehdjk.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gow.yvedp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wtv.jyoumei.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xwh.vqdsnc.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zsi.feifeiyinyue.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rcd.jinyuanbaomall.cn

[K05] 深拷贝对象
来源：http://lph.xziqi.cn

Py:   copy.deepcopy(obj)
来源：http://wak.ydzc1.top

PHP:  unserialize(serialize($obj));
来源：http://nnu.yj202588.top

JS:   structuredClone(obj)
来源：http://jwx.epnwcf.com

TS:   structuredClone(obj)
来源：http://jmu.zhongyouzk.top

Java: // 手写拷贝构造，或序列化往返
来源：http://bzj.yj20258888.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qce.gaohongyu789.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ljp.hesvh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cbo.smart0.xyz

[K06] 解析 URL 查询串
来源：http://phs.mhx1999.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sap.shangyingyoupin.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fcz.vqdsnc.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://emo.epnwcf.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zlj.hcnkem.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rdk.fktsv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vqs.cdnleiting.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://eak.yvedp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cyf.dianchejie.cn

[K07] 进制转换
来源：http://ntp.jinqigfzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hvt.yj20258.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://luj.hysaishi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uad.yueranfly.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dvf.pengpengdd.cyou

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gzq.havefunace.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://aou.redwolf501.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://myp.52xcode.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ztx.feifeiyinyue.top

[K08] 二进制序列化（非 JSON）
来源：http://fqx.hnxiangtu.top

Py:   pickle.dumps(obj)
来源：http://zbg.yvedp.cn


<!-- 参考信息 -->