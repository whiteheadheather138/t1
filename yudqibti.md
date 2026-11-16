代发 wailian999

JS:   class MyError extends Error {}
来源：http://wge.quarkkingdee.top

TS:   class MyError extends Error {}
来源：http://nca.9152youxi.cn

Java: class MyException extends RuntimeException {}
来源：http://sot.zhengqikj.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ndt.epnwcf.com

Ruby: class MyError < StandardError; end
来源：http://ixt.jiagoushi.top

C#:   class MyException : Exception {}
来源：http://fps.dashuyun.cn

[H05] 捕获特定类型
来源：http://dyx.redwolf501.top

Py:   except ValueError as e:
来源：http://uno.c1oappe.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pze.bjfxy.top

JS:   if (e instanceof TypeError) {}
来源：http://ujc.nwbrower.top

TS:   if (e instanceof TypeError) {}
来源：http://ied.nanxuanxn.top

Java: catch (IOException | SQLException e) {}
来源：http://ncp.nanxinkj.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yda.xziqi.cn

Ruby: rescue ArgumentError => e
来源：http://joy.gzhubu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tds.xziqi.cn

[H06] 可选值 / 空值安全访问
来源：http://hug.zhixingplan.top

Py:   value = d.get("k") or default
来源：http://qwb.daria6918.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gmy.hammf.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wgc.hnqzz.top

TS:   obj?.a?.b;  d ?? default
来源：http://evd.iojbl.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gpt.wangshuangyany.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jok.xingfuxueyuan.xyz

Ruby: d&.dig(:a, :b)
来源：http://rxp.yuanzhike.top

C#:   obj?.A?.B ?? default
来源：http://wfm.316326.xyz

[H07] 断言
来源：http://utg.uphjek.com

Py:   assert x > 0, "必须为正"
来源：http://crr.aizwys.cn

PHP:  assert($x > 0);
来源：http://jam.sjlbkw.cn

JS:   console.assert(x > 0);
来源：http://rve.shangyingyoupin.top

TS:   console.assert(x > 0);
来源：http://ngp.9152youxi.cn

Java: assert x > 0 : "必须为正";
来源：http://qdf.yongpay.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dte.ctjpmb.com

Ruby: raise "必须为正" unless x > 0
来源：http://ifw.xuanzx.com

C#:   Debug.Assert(x > 0);
来源：http://olf.sxryk.cn

[H08] 获取错误信息与堆栈
来源：http://mpd.mhx1999.top

Py:   str(e);  traceback.format_exc()
来源：http://vbn.sweek.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pkz.daria6918.cn

JS:   e.message;  e.stack
来源：http://iio.vqdsnc.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://laf.yuxming.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hyf.cqqwz.cn

Go:   err.Error()
来源：http://taz.yueranfly.top

Ruby: e.message;  e.backtrace
来源：http://kfc.guannengcc.top

C#:   e.Message;  e.StackTrace
来源：http://rcu.smart0.xyz

[H09] 带错误码的异常
来源：http://cfq.tian-w.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ywh.hnqzz.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://eyf.tarul.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tpu.sjlbkw.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xgr.xinyue.icu

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://knv.jyoumei.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://csl.jinyuanbaomall.cn

Ruby: raise MyError.new("fail", 500)
来源：http://eys.hfpthk.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wbb.aizwys.cn

[H10] 资源自动释放
来源：http://kss.hnxiangtu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ygj.jqgufenzy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://iqh.nanxuanxn.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ahs.hfpthk.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://eoq.epnwcf.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mkf.zhongyouzk.top

Go:   defer f.Close()
来源：http://ned.ppjwa.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uvc.cashguo.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mgx.hywenlv.cn

================================================================================
来源：http://rsn.zhoulong.xyz

I. 正则表达式
来源：http://ukp.zhixingplan.top

================================================================================
来源：http://nna.52xcode.cn

[I01] 判断是否匹配
来源：http://qkz.fengsongda.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nxu.yj20258.top

PHP:  preg_match('/\d+/', $s);
来源：http://mwi.guannengcc.top

JS:   /\d+/.test(s)
来源：http://vyl.jiagoushi.top

TS:   /\d+/.test(s)
来源：http://qga.zdbjq.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pdk.sufxvd.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xkw.sweek.top

Ruby: s.match?(/\d+/)
来源：http://rzo.jlsjyb.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://haj.9152youxi.cn

[I02] 提取所有匹配
来源：http://qtn.guowangkeji.top

Py:   re.findall(r"\d+", s)
来源：http://sxo.pycfn.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dny.316326.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://adf.bbcook.cn

TS:   s.match(/\d+/g)
来源：http://opl.52xcode.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qmp.sjlbkw.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kys.ydzc1.top

Ruby: s.scan(/\d+/)
来源：http://clx.hnqzz.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ioh.cucudq.cn

[I03] 提取捕获分组
来源：http://fev.zhaomingkeji.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dqb.aibaodan.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mzq.9152youxi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bzq.andypj.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xkj.c1oappe.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lsr.birdmap.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://anf.zhijiandao.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://epb.kuanghao11.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ftq.shanyushiyangtech.top

[I04] 正则替换
来源：http://ssq.jyoumei.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vuc.andypj.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bmw.jinyuanbaomall.cn

JS:   s.replace(/\d+/g, "#")
来源：http://oeg.pycfn.com

TS:   s.replace(/\d+/g, "#")
来源：http://aca.andypj.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://ezl.ivvv.top

Go:   re.ReplaceAllString(s, "#")
来源：http://etw.hongshengwenyu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://mqy.andypj.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dzx.pycfn.com

[I05] 按正则拆分
来源：http://ngm.chenzaomai.com

Py:   re.split(r"\s*,\s*", s)
来源：http://xuf.yuanzhike.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zzl.havefunace.top

JS:   s.split(/\s*,\s*/)
来源：http://hfp.jinqigfzy.top

TS:   s.split(/\s*,\s*/)
来源：http://eqn.9152youxi.cn

Java: s.split("\\s*,\\s*")
来源：http://zbm.ehwqpu.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rtp.chenlongwang.top

Ruby: s.split(/\s*,\s*/)
来源：http://bul.smart0.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pid.daxiang520.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xfd.sysykeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://arn.gotoacloud.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tzn.jinghuilouyu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mwb.zhoulong.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ybg.jiagoushi.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dzb.ehwqpu.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bvp.zdbjq.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hud.tianlin.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://eaw.fengsongda.top

[I07] 忽略大小写与多行模式
来源：http://ohq.guannengcc.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fjl.wangshuangyany.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ksn.jyoumei.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kpm.gotoacloud.top

TS:   /error/gim
来源：http://lqb.jlsjyb.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jhw.ybcxt.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qcd.vehdjk.com

Ruby: s.scan(/error/i)
来源：http://otz.jinghuilouyu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jgm.jyoumei.cn

[I08] 贪婪与非贪婪匹配
来源：http://efd.tanke756.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://iay.cashguo.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://iuw.sxryk.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mct.ydzc1.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zgb.bjfxy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://nnl.dashuyun.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qzp.pycfn.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uqx.hnxiangtu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xgz.nwbrower.top

================================================================================
来源：http://hpy.xylfe.cn

J. 日期与时间
来源：http://ulk.hysaishi.cn

================================================================================
来源：http://koh.hysaishi.cn

[J01] 获取当前时间
来源：http://osc.mhx1999.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ynx.yueranfly.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://woo.xuetiantiany.cn

JS:   new Date();  Date.now()
来源：http://fos.hongshengwenyu.top

TS:   new Date();  Date.now()
来源：http://twp.mhx1999.top

Java: LocalDateTime.now();  Instant.now()
来源：http://apc.nwbrower.top

Go:   time.Now()
来源：http://isv.smart0.xyz

Ruby: Time.now
来源：http://hie.guannengcc.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ckh.gotoacloud.top

[J02] 格式化输出
来源：http://vho.zhongyouzk.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kxy.zhaomingkeji.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://obw.yfazqb.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bsd.bbcook.cn

TS:   d.toISOString()
来源：http://sua.yuanzhike.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xrk.havefunace.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://oin.ivvv.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bcu.jianghu66.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tbq.hnqzz.top

[J03] 字符串解析为日期
来源：http://aal.daxiang520.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zkf.sjlbkw.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dlz.9152youxi.cn

JS:   new Date("2024-01-02")
来源：http://ebg.tarul.cn

TS:   new Date("2024-01-02")
来源：http://avj.gogol.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hhv.vqdsnc.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bse.yueranfly.top

Ruby: Date.parse("2024-01-02")
来源：http://vpe.xinyue.icu

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://imx.nwbrower.top

[J04] 时间戳与日期互转
来源：http://tjq.daria6918.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wul.jinghuilouyu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qsh.shangyingyoupin.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nqq.ybcxt.top

TS:   Math.floor(Date.now() / 1000)
来源：http://nmr.mhx1999.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vhw.cqqwz.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rzw.jiagoushi.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ond.jinqigfzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://aok.epnwcf.com

[J05] 时间加减（加 7 天）
来源：http://tue.vqdsnc.cn

Py:   now + timedelta(days=7)
来源：http://qpc.jyoumei.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wju.dianchejie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rav.svipenyu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tsh.9152youxi.cn

Java: LocalDate.now().plusDays(7)
来源：http://zyq.yuxming.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hsx.guowangkeji.top

Ruby: Time.now + 7 * 86400
来源：http://tzs.jiagoushi.top

C#:   DateTime.Now.AddDays(7)
来源：http://noa.jlsjyb.cn

[J06] 计算两时间之差
来源：http://tch.havefunace.top

Py:   (end - start).total_seconds()
来源：http://reo.hnxiangtu.top

PHP:  $end->diff($start)->days;
来源：http://ppe.havefunace.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bvu.snrcjt.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hex.yfazqb.com

Java: Duration.between(start, end).toSeconds()
来源：http://und.52xcode.cn

Go:   end.Sub(start).Hours()
来源：http://qho.meibo888.top

Ruby: end - start                 # 返回秒数
来源：http://ctq.ppjwa.cn

C#:   (end - start).TotalSeconds
来源：http://qjf.hcnkem.com

[J07] 比较两个日期
来源：http://vil.birdmap.top

Py:   d1 < d2;  d1 == d2
来源：http://fan.birdmap.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rdm.bjfxy.top

JS:   d1.getTime() < d2.getTime()
来源：http://jij.ehwqpu.com

TS:   d1.getTime() < d2.getTime()
来源：http://pkj.yuxming.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rvp.andypj.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cfe.yvedp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://uib.hcnkem.com

C#:   d1 < d2;  d1 == d2
来源：http://ctq.quarkkingdee.top

[J08] 提取年月日与星期
来源：http://ist.hcnkem.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bbn.shzxlz.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lic.meibo888.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vod.ywan-chungtsiang.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://top.guannengcc.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://azq.cashguo.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xft.yj20258.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xsz.zdqjudy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jjo.nanxinkj.top

[J09] 时区处理
来源：http://caq.52xcode.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vrt.aizwys.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lwo.zhoulong.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fqk.9152youxi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fub.yongpay.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gqr.fanxiaobao.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ayd.zhongyouzk.top

Ruby: Time.now.getlocal("+08:00")
来源：http://vcs.yj202588.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cme.smart0.xyz

[J10] 取今天 / 本月第一天
来源：http://iog.yuanzhike.top

Py:   date.today();  date.today().replace(day=1)
来源：http://gof.bjfxy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://evv.tanke756.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://puz.aibaodan.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nva.tarul.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cck.yj20258888.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hep.hysaishi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://erx.cashguo.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zze.xuetiantiany.cn

================================================================================
来源：http://tft.gaohongyu789.top

K. JSON 与序列化
来源：http://qgz.nanxuanxn.top

================================================================================
来源：http://spv.haohaochexian.top

[K01] 对象转 JSON 字符串
来源：http://wdm.jinqigufen.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gtm.316326.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fyx.jianghu66.top

JS:   JSON.stringify(obj)
来源：http://yyf.zhaomingkeji.xyz

TS:   JSON.stringify(obj)
来源：http://bvj.sxryk.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tfh.chenlongwang.top

Go:   json.Marshal(obj)
来源：http://rcq.yonumen.top

Ruby: obj.to_json                                     // require "json"
来源：http://zzi.zycfv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://mbo.fktsv.cn

[K02] JSON 字符串转对象
来源：http://adc.chenzaomai.com

Py:   json.loads(s)
来源：http://kwy.wangdashe.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ivu.daria6918.cn

JS:   JSON.parse(s)
来源：http://rpu.mhx1999.top

TS:   JSON.parse(s)
来源：http://cqi.sufxvd.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mkq.0kj1m.cn

Go:   json.Unmarshal(data, &v)
来源：http://sef.guannengcc.top

Ruby: JSON.parse(s)
来源：http://bzu.chenlongwang.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zyv.c1oappe.top

[K03] JSON 美化输出（带缩进）
来源：http://gzm.andypj.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://utz.yongpay.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tos.jiagoushi.top

JS:   JSON.stringify(obj, null, 2)
来源：http://gan.tian-w.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://meu.xingfuxueyuan.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lfc.ehwqpu.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://egl.pycfn.com

Ruby: JSON.pretty_generate(obj)
来源：http://kgu.hfpthk.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ypv.xziqi.cn

[K04] 读取 JSON 文件
来源：http://pkc.andypj.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zcg.guannengcc.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gjg.yongpay.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gwh.yj20258.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bbb.hcnkem.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qxv.jqgfzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hsp.pycfn.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://dem.ybcxt.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ofp.nwbrower.top

[K05] 深拷贝对象
来源：http://yhw.wangdashe.top

Py:   copy.deepcopy(obj)
来源：http://zad.hcnkem.com

PHP:  unserialize(serialize($obj));
来源：http://ibn.chenlongwang.top

JS:   structuredClone(obj)
来源：http://tnn.jinghuilouyu.cn

TS:   structuredClone(obj)
来源：http://iuv.hywenlv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://uay.aibaodan.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://apx.yj20258888.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zum.xylfe.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dss.ctjpmb.com

[K06] 解析 URL 查询串
来源：http://wqe.nwbrower.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gwp.dianchejie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vwd.yfazqb.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lll.ehwqpu.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rbm.0kj1m.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sxo.epnwcf.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://yiw.vqdsnc.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ytn.guowangkeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ccd.fengsongda.top

[K07] 进制转换
来源：http://ywp.xuanzx.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://snj.9152youxi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://arj.pengpengdd.cyou

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bht.jianghu66.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mhl.guowangkeji.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gwl.quarkkingdee.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://stt.zdbjq.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ell.tanke756.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jrg.wangshuangyany.cn

[K08] 二进制序列化（非 JSON）
来源：http://hlu.fanxiaobao.xyz

Py:   pickle.dumps(obj)
来源：http://gum.sxryk.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vwv.c1oappe.top

JS:   v8.serialize(obj)        // Node
来源：http://imw.gzhubu.top

TS:   v8.serialize(obj)        // Node
来源：http://lfc.epnwcf.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cya.ydjk.org.cn


<!-- 参考信息 -->