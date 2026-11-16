代发 wailian999

JS:   class MyError extends Error {}
来源：http://vdi.52xcode.cn

TS:   class MyError extends Error {}
来源：http://psa.iojbl.cn

Java: class MyException extends RuntimeException {}
来源：http://rgm.vqdsnc.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://oya.pengpengdd.cyou

Ruby: class MyError < StandardError; end
来源：http://kvh.shanyushiyangtech.top

C#:   class MyException : Exception {}
来源：http://lit.jianghu66.top

[H05] 捕获特定类型
来源：http://chs.ywan-chungtsiang.top

Py:   except ValueError as e:
来源：http://iuq.zhongyouzk.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qpj.yueranfly.top

JS:   if (e instanceof TypeError) {}
来源：http://ngu.fehbvm.com

TS:   if (e instanceof TypeError) {}
来源：http://uxl.hysaishi.cn

Java: catch (IOException | SQLException e) {}
来源：http://sij.tianlin.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xpt.guowangkeji.top

Ruby: rescue ArgumentError => e
来源：http://evb.cdnleiting.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dny.jinqigufen.top

[H06] 可选值 / 空值安全访问
来源：http://ltk.zhiwuduotai.top

Py:   value = d.get("k") or default
来源：http://fwa.xylfe.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cfj.jinghuilouyu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://kkg.ydzc1.top

TS:   obj?.a?.b;  d ?? default
来源：http://bmv.guowangkeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ssj.kuanghao11.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hou.hnxiangtu.top

Ruby: d&.dig(:a, :b)
来源：http://umz.quarkkingdee.top

C#:   obj?.A?.B ?? default
来源：http://tdu.chenlongwang.top

[H07] 断言
来源：http://ztk.haohaochexian.top

Py:   assert x > 0, "必须为正"
来源：http://xrg.ydjk.org.cn

PHP:  assert($x > 0);
来源：http://ooc.daxiang520.top

JS:   console.assert(x > 0);
来源：http://sud.fktsv.cn

TS:   console.assert(x > 0);
来源：http://nof.dianchejie.cn

Java: assert x > 0 : "必须为正";
来源：http://ozq.ydzc1.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dqi.bjfxy.top

Ruby: raise "必须为正" unless x > 0
来源：http://ypc.zdqjudy.top

C#:   Debug.Assert(x > 0);
来源：http://ywb.daria6918.cn

[H08] 获取错误信息与堆栈
来源：http://eqi.dashuyun.cn

Py:   str(e);  traceback.format_exc()
来源：http://ehj.hammf.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wpr.wangdashe.top

JS:   e.message;  e.stack
来源：http://biw.ydjk.org.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rxk.chenlongwang.top

Java: e.getMessage();  e.printStackTrace()
来源：http://wkk.andypj.xyz

Go:   err.Error()
来源：http://qbb.zdbjq.cn

Ruby: e.message;  e.backtrace
来源：http://ubx.zhijiandao.cn

C#:   e.Message;  e.StackTrace
来源：http://ydq.zhiwuduotai.top

[H09] 带错误码的异常
来源：http://rnx.zhixingplan.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://roe.shangyingyoupin.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://wjn.tianlin.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uxh.zdbjq.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yon.shuidangran.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://udi.hcnkem.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pix.smart0.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://sjd.bbcook.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://aid.kuanghao11.cn

[H10] 资源自动释放
来源：http://mxf.epnwcf.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://mqx.xuanzx.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zzx.shanyushiyangtech.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jbe.zhijiandao.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yrx.zhixingplan.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vkx.bbcook.cn

Go:   defer f.Close()
来源：http://bph.bbcook.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wtc.zdbjq.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tql.dianchejie.cn

================================================================================
来源：http://yld.vqdsnc.cn

I. 正则表达式
来源：http://omr.mhx1999.top

================================================================================
来源：http://vjq.ehwqpu.com

[I01] 判断是否匹配
来源：http://hys.iojbl.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rsd.9152youxi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vvd.yj20258888.top

JS:   /\d+/.test(s)
来源：http://cpz.ydzc1.top

TS:   /\d+/.test(s)
来源：http://smt.vqdsnc.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mqi.zhoulong.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kfx.zdqjudy.top

Ruby: s.match?(/\d+/)
来源：http://nac.xziqi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ood.shangyingyoupin.top

[I02] 提取所有匹配
来源：http://zeg.9152youxi.cn

Py:   re.findall(r"\d+", s)
来源：http://jmb.yonumen.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bnw.gogol.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jta.9152youxi.cn

TS:   s.match(/\d+/g)
来源：http://ovj.snrcjt.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tvp.daxiang520.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://heo.sweek.top

Ruby: s.scan(/\d+/)
来源：http://rqj.yfazqb.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ned.yj20258.top

[I03] 提取捕获分组
来源：http://znh.ydjk.org.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tii.redwolf501.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kzc.sjlbkw.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yym.fengsongda.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ijc.daria6918.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ioc.andypj.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://snj.jyoumei.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yzl.feifeiyinyue.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sbv.sjlbkw.cn

[I04] 正则替换
来源：http://fhb.hnxiangtu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://dtu.iojbl.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://woo.ctjpmb.com

JS:   s.replace(/\d+/g, "#")
来源：http://wzn.chenzaomai.com

TS:   s.replace(/\d+/g, "#")
来源：http://blx.hnxiangtu.top

Java: s.replaceAll("\\d+", "#")
来源：http://cpe.hongshengwenyu.top

Go:   re.ReplaceAllString(s, "#")
来源：http://uwi.uphjek.com

Ruby: s.gsub(/\d+/, "#")
来源：http://gaf.hammf.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qam.yj20258888.top

[I05] 按正则拆分
来源：http://amv.yuxming.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://olp.xylfe.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dsx.zdqjudy.top

JS:   s.split(/\s*,\s*/)
来源：http://ymn.yonumen.top

TS:   s.split(/\s*,\s*/)
来源：http://cdo.c1oappe.top

Java: s.split("\\s*,\\s*")
来源：http://gfy.cheryme.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ilr.xingfuxueyuan.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://tju.316326.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mwv.52xcode.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://llz.vqdsnc.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bhr.aizwys.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://anc.hnqzz.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tux.nanxuanxn.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://exx.hammf.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zbd.hongshengwenyu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ciu.nanxuanxn.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dws.yfazqb.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qwu.ivvv.top

[I07] 忽略大小写与多行模式
来源：http://stg.zycfv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fml.shzxlz.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qlz.meibo888.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hzf.yuxming.cn

TS:   /error/gim
来源：http://htf.316326.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wtm.daria6918.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ldu.daria6918.cn

Ruby: s.scan(/error/i)
来源：http://hdu.shanyushiyangkeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xxa.zdbjq.cn

[I08] 贪婪与非贪婪匹配
来源：http://gvy.yfazqb.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zux.sxryk.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dgt.snrcjt.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jbf.wangshuangyany.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pab.zhixingplan.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://yuh.sufxvd.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mwb.tian-w.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jya.c1oappe.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gxu.ctjpmb.com

================================================================================
来源：http://xda.52xcode.cn

J. 日期与时间
来源：http://ksd.cheryme.top

================================================================================
来源：http://ntm.yonumen.top

[J01] 获取当前时间
来源：http://mkb.xingfuxueyuan.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://wdm.yangfankeji.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://iks.shanyushiyangtech.top

JS:   new Date();  Date.now()
来源：http://bqu.feifeiyinyue.top

TS:   new Date();  Date.now()
来源：http://ety.svipenyu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fmr.fanxiaobao.xyz

Go:   time.Now()
来源：http://ldj.hcnkem.com

Ruby: Time.now
来源：http://knu.ctjpmb.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zsz.ybcxt.top

[J02] 格式化输出
来源：http://phf.tian-w.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bew.ivvv.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vpp.hnxiangtu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ore.ywan-chungtsiang.top

TS:   d.toISOString()
来源：http://bnv.yongpay.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://txf.52xcode.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hkd.yuanzhike.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zjw.chenzaomai.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ymt.bjfxy.top

[J03] 字符串解析为日期
来源：http://tgf.haohaochexian.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://szn.sufxvd.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dgc.wangdashe.top

JS:   new Date("2024-01-02")
来源：http://clt.xziqi.cn

TS:   new Date("2024-01-02")
来源：http://sca.iojbl.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gmh.shanyushiyangkeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cgx.yueranfly.top

Ruby: Date.parse("2024-01-02")
来源：http://hjl.yueranfly.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rio.316326.xyz

[J04] 时间戳与日期互转
来源：http://thj.316326.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pkm.jiagoushi.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zhi.kuanghao11.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cuj.vqdsnc.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jlj.zhiwuduotai.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mum.dashuyun.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mfy.zhixingplan.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lxr.xingfuxueyuan.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pws.cqqwz.cn

[J05] 时间加减（加 7 天）
来源：http://ucf.epnwcf.com

Py:   now + timedelta(days=7)
来源：http://xwi.snrcjt.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tvc.shangyingyoupin.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wlq.jinghuilouyu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vcw.cqqwz.cn

Java: LocalDate.now().plusDays(7)
来源：http://fzk.cqqwz.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wcf.yfazqb.com

Ruby: Time.now + 7 * 86400
来源：http://sod.yonumen.top

C#:   DateTime.Now.AddDays(7)
来源：http://qth.xuetiantiany.cn

[J06] 计算两时间之差
来源：http://upv.zhiwuduotai.top

Py:   (end - start).total_seconds()
来源：http://jzs.tarul.cn

PHP:  $end->diff($start)->days;
来源：http://jbc.hnxiangtu.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hil.hysaishi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gxf.hywenlv.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ech.zhijiandao.cn

Go:   end.Sub(start).Hours()
来源：http://haj.pycfn.com

Ruby: end - start                 # 返回秒数
来源：http://uif.birdmap.top

C#:   (end - start).TotalSeconds
来源：http://nxb.ivvv.top

[J07] 比较两个日期
来源：http://giy.sufxvd.cn

Py:   d1 < d2;  d1 == d2
来源：http://voa.c1oappe.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cbw.jinyuanbaomall.cn

JS:   d1.getTime() < d2.getTime()
来源：http://viz.jianghu66.top

TS:   d1.getTime() < d2.getTime()
来源：http://tge.snrcjt.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://spy.zhiwuduotai.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gna.jyoumei.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rnv.gzhubu.top

C#:   d1 < d2;  d1 == d2
来源：http://oee.shanyushiyangkeji.top

[J08] 提取年月日与星期
来源：http://hjv.ydzc1.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://izp.smart0.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ala.0kj1m.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sun.ctjpmb.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ycl.gotoacloud.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xaf.zhaomingkeji.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jju.zycfv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wsh.jqgufenzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ijw.gaohongyu789.top

[J09] 时区处理
来源：http://jyr.snrcjt.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ypp.mhx1999.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://opb.shzxlz.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pnr.hnqzz.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xet.nanxinkj.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kjn.yj202588.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tdm.kuanghao11.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://syv.gzhubu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jmt.shangyingyoupin.top

[J10] 取今天 / 本月第一天
来源：http://qxq.jqgfzy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://klf.ppjwa.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sco.jinqigufen.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qxd.yj20258.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://avs.hcnkem.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qjp.gaohongyu789.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ujy.redwolf501.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cbj.shzxlz.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nnx.xuanzx.com

================================================================================
来源：http://bae.xingfuxueyuan.xyz

K. JSON 与序列化
来源：http://cuj.zhengqikj.top

================================================================================
来源：http://ppq.iojbl.cn

[K01] 对象转 JSON 字符串
来源：http://ftm.pycfn.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tcy.ywan-chungtsiang.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mut.ydjk.org.cn

JS:   JSON.stringify(obj)
来源：http://aca.pengpengdd.cyou

TS:   JSON.stringify(obj)
来源：http://xmb.chenlongwang.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://swa.hcnkem.com

Go:   json.Marshal(obj)
来源：http://fwj.fanxiaobao.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://jvy.nwbrower.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ctl.zhongyouzk.top

[K02] JSON 字符串转对象
来源：http://dqf.redwolf501.top

Py:   json.loads(s)
来源：http://waw.gotoacloud.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://add.tian-w.cn

JS:   JSON.parse(s)
来源：http://cnd.hcnkem.com

TS:   JSON.parse(s)
来源：http://evz.ywan-chungtsiang.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tas.sysykeji.top

Go:   json.Unmarshal(data, &v)
来源：http://zdt.ybcxt.top

Ruby: JSON.parse(s)
来源：http://nej.dianchejie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://umg.chenjidiqi.icu

[K03] JSON 美化输出（带缩进）
来源：http://sys.daxiang520.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wxm.havefunace.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xcz.shzxlz.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xtz.uphjek.com

TS:   JSON.stringify(obj, null, 2)
来源：http://fdv.fktsv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lkn.ppjwa.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qde.dashuyun.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qnd.yangfankeji.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ppy.uphjek.com

[K04] 读取 JSON 文件
来源：http://dky.zhoulong.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uat.9152youxi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hrb.haohaochexian.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kty.iojbl.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oqb.vqdsnc.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xvp.gotoacloud.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kxv.sxryk.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://iks.jyoumei.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dpm.hesvh.cn

[K05] 深拷贝对象
来源：http://baw.ivvv.top

Py:   copy.deepcopy(obj)
来源：http://jtu.sweek.top

PHP:  unserialize(serialize($obj));
来源：http://ogh.xziqi.cn

JS:   structuredClone(obj)
来源：http://xrz.jyoumei.cn

TS:   structuredClone(obj)
来源：http://dnh.jqgufenzy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://dlx.vehdjk.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mzk.yuxming.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uwq.redwolf501.top

C#:   // 序列化往返，或自定义 Clone
来源：http://eqn.yuanzhike.top

[K06] 解析 URL 查询串
来源：http://tav.andypj.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mtr.sysykeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ufi.daria6918.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wdc.iojbl.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kgo.uphjek.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yby.hysaishi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://kvt.cucudq.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nyg.gogol.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://csd.ywan-chungtsiang.top

[K07] 进制转换
来源：http://eoc.nwbrower.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://das.fzhhl.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ptu.jyoumei.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://scy.daria6918.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zbr.hfpthk.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qvo.sufxvd.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hmu.xingfuxueyuan.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ufc.chenlongwang.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://brr.bbcook.cn

[K08] 二进制序列化（非 JSON）
来源：http://wie.ywan-chungtsiang.top

Py:   pickle.dumps(obj)
来源：http://rec.0kj1m.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fit.dianchejie.cn

JS:   v8.serialize(obj)        // Node
来源：http://bwx.zdbjq.cn

TS:   v8.serialize(obj)        // Node
来源：http://xjf.shangyingyoupin.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gso.tanke756.top


<!-- 参考信息 -->