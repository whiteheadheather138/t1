代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://vxv.hammf.cn

[H04] 自定义异常类型
来源：http://ifj.meibo888.top

Py:   class MyError(Exception): pass
来源：http://thr.zhixingplan.top

PHP:  class MyError extends RuntimeException {}
来源：http://yhm.pycfn.com

JS:   class MyError extends Error {}
来源：http://pze.xingfuxueyuan.xyz

TS:   class MyError extends Error {}
来源：http://gfw.hcnkem.com

Java: class MyException extends RuntimeException {}
来源：http://naw.iojbl.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dlq.c1oappe.top

Ruby: class MyError < StandardError; end
来源：http://efh.hnqzz.top

C#:   class MyException : Exception {}
来源：http://wpz.bjfxy.top

[H05] 捕获特定类型
来源：http://hgg.0kj1m.cn

Py:   except ValueError as e:
来源：http://wrn.daxiang520.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qjg.smart0.xyz

JS:   if (e instanceof TypeError) {}
来源：http://ots.zhaomingkeji.xyz

TS:   if (e instanceof TypeError) {}
来源：http://sby.wangshuangyany.cn

Java: catch (IOException | SQLException e) {}
来源：http://dix.yueranfly.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ael.jqgufenzy.top

Ruby: rescue ArgumentError => e
来源：http://pms.yuanzhike.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://iff.jyoumei.cn

[H06] 可选值 / 空值安全访问
来源：http://uys.yj20258888.top

Py:   value = d.get("k") or default
来源：http://erm.zdqjudy.top

PHP:  $v = $d["k"] ?? null;
来源：http://axc.zycfv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://jwj.sysykeji.top

TS:   obj?.a?.b;  d ?? default
来源：http://ndz.chenjidiqi.icu

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://waq.snrcjt.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fiv.meibo888.top

Ruby: d&.dig(:a, :b)
来源：http://xwq.tian-w.cn

C#:   obj?.A?.B ?? default
来源：http://dfi.316326.xyz

[H07] 断言
来源：http://rrg.xziqi.cn

Py:   assert x > 0, "必须为正"
来源：http://xnj.fengsongda.top

PHP:  assert($x > 0);
来源：http://uga.yj20258888.top

JS:   console.assert(x > 0);
来源：http://ych.daxiang520.top

TS:   console.assert(x > 0);
来源：http://bgo.xylfe.cn

Java: assert x > 0 : "必须为正";
来源：http://uad.gzhubu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qus.fanxiaobao.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://rdw.nanxinkj.top

C#:   Debug.Assert(x > 0);
来源：http://nzm.yuxming.cn

[H08] 获取错误信息与堆栈
来源：http://ygy.ctjpmb.com

Py:   str(e);  traceback.format_exc()
来源：http://rqp.havefunace.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xdf.yongpay.top

JS:   e.message;  e.stack
来源：http://dvz.aibaodan.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vli.tarul.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nvo.ybcxt.top

Go:   err.Error()
来源：http://heo.mhx1999.top

Ruby: e.message;  e.backtrace
来源：http://zwh.fanxiaobao.xyz

C#:   e.Message;  e.StackTrace
来源：http://clh.shanyushiyangkeji.top

[H09] 带错误码的异常
来源：http://gvo.hongshengwenyu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ljz.wangshuangyany.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://tak.tarul.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kvm.shanyushiyangtech.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://oup.feifeiyinyue.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lod.sysykeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uyp.snrcjt.cn

Ruby: raise MyError.new("fail", 500)
来源：http://sqw.yonumen.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xbk.svipenyu.cn

[H10] 资源自动释放
来源：http://zfw.aibaodan.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pmi.redwolf501.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ynm.hysaishi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://meg.52xcode.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jpg.zhengqikj.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lcr.svipenyu.cn

Go:   defer f.Close()
来源：http://cjc.ywan-chungtsiang.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dpa.gaohongyu789.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tbp.jinqigufen.top

================================================================================
来源：http://xxu.havefunace.top

I. 正则表达式
来源：http://hdd.jyoumei.cn

================================================================================
来源：http://fnd.shangyingyoupin.top

[I01] 判断是否匹配
来源：http://ctm.zdqjudy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://loc.bbcook.cn

PHP:  preg_match('/\d+/', $s);
来源：http://yex.jinqigufen.top

JS:   /\d+/.test(s)
来源：http://pbg.aibaodan.cn

TS:   /\d+/.test(s)
来源：http://fpj.wangdashe.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yrl.shanyushiyangkeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fed.snrcjt.cn

Ruby: s.match?(/\d+/)
来源：http://lbq.jinyuanbaomall.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://iuy.gaohongyu789.top

[I02] 提取所有匹配
来源：http://jjz.gotoacloud.top

Py:   re.findall(r"\d+", s)
来源：http://kjl.yj20258888.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ywa.dianchejie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hvt.tarul.cn

TS:   s.match(/\d+/g)
来源：http://bfr.xingfuxueyuan.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ddh.xuetiantiany.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tmj.yonumen.top

Ruby: s.scan(/\d+/)
来源：http://syc.shanyushiyangtech.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zeg.yfazqb.com

[I03] 提取捕获分组
来源：http://vlt.fengsongda.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dxx.xinyue.icu

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pcm.jqgfzy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://iag.xuetiantiany.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lrm.svipenyu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ewz.dianchejie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rgx.9152youxi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tga.yanxiufei.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://byr.shanyushiyangkeji.top

[I04] 正则替换
来源：http://jns.fengsongda.top

Py:   re.sub(r"\d+", "#", s)
来源：http://yos.jinghuilouyu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pck.hnqzz.top

JS:   s.replace(/\d+/g, "#")
来源：http://cxi.quarkkingdee.top

TS:   s.replace(/\d+/g, "#")
来源：http://gfh.daria6918.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ctq.hammf.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://cmb.xinyue.icu

Ruby: s.gsub(/\d+/, "#")
来源：http://krw.zhiwuduotai.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://eat.dianchejie.cn

[I05] 按正则拆分
来源：http://fuo.hongshengwenyu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://emh.ppjwa.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xlo.xingfuxueyuan.xyz

JS:   s.split(/\s*,\s*/)
来源：http://ivm.yanxiufei.cn

TS:   s.split(/\s*,\s*/)
来源：http://ubu.havefunace.top

Java: s.split("\\s*,\\s*")
来源：http://vpa.zhixingplan.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bbf.gotoacloud.top

Ruby: s.split(/\s*,\s*/)
来源：http://uvy.shangyingyoupin.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qim.yuanzhike.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ytu.ydzc1.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gmi.bbcook.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hkb.daria6918.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pym.yuxming.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lct.bjfxy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pxr.vqdsnc.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://apg.jyoumei.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hhu.kuanghao11.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nql.fengsongda.top

[I07] 忽略大小写与多行模式
来源：http://dfx.jyoumei.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wxf.gzhubu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ffz.zhengqikj.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pph.jiagoushi.top

TS:   /error/gim
来源：http://jfu.svipenyu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fsb.fengsongda.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://aqg.tanke756.top

Ruby: s.scan(/error/i)
来源：http://zfk.uphjek.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ogl.ctjpmb.com

[I08] 贪婪与非贪婪匹配
来源：http://edj.gotoacloud.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ofe.yvedp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vfp.kuanghao11.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uny.hesvh.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jko.chenzaomai.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://inh.hfpthk.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://aea.uphjek.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xvn.ehwqpu.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://coh.ivvv.top

================================================================================
来源：http://fqa.yj20258888.top

J. 日期与时间
来源：http://fqj.birdmap.top

================================================================================
来源：http://ysg.nwbrower.top

[J01] 获取当前时间
来源：http://gey.chenlongwang.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://isc.cucudq.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kyn.pycfn.com

JS:   new Date();  Date.now()
来源：http://ceu.yj20258.top

TS:   new Date();  Date.now()
来源：http://lsm.hywenlv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ojv.hnxiangtu.top

Go:   time.Now()
来源：http://wnt.yuanzhike.top

Ruby: Time.now
来源：http://mlv.gaohongyu789.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fun.zhongyouzk.top

[J02] 格式化输出
来源：http://god.epnwcf.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dva.shuidangran.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://css.zhaomingkeji.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ksc.iojbl.cn

TS:   d.toISOString()
来源：http://bqf.nanxinkj.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jrz.nanxuanxn.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cea.svipenyu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qrl.jqgufenzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jbj.yj20258888.top

[J03] 字符串解析为日期
来源：http://xxe.fktsv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tgp.zhijiandao.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zrb.shangyingyoupin.top

JS:   new Date("2024-01-02")
来源：http://yzy.hongshengwenyu.top

TS:   new Date("2024-01-02")
来源：http://njp.ppjwa.cn

Java: LocalDate.parse("2024-01-02")
来源：http://doy.0kj1m.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xvo.hnxiangtu.top

Ruby: Date.parse("2024-01-02")
来源：http://zlu.meibo888.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jty.yuxming.cn

[J04] 时间戳与日期互转
来源：http://oed.chenzaomai.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xbv.hysaishi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ktg.hnqzz.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://odn.yj20258888.top

TS:   Math.floor(Date.now() / 1000)
来源：http://stn.jqgfzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tsi.aizwys.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cky.yueranfly.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fch.yuanzhike.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://atv.xuanzx.com

[J05] 时间加减（加 7 天）
来源：http://nin.sufxvd.cn

Py:   now + timedelta(days=7)
来源：http://qcg.pengpengdd.cyou

PHP:  (new DateTime())->modify("+7 days");
来源：http://zrl.hywenlv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rej.ivvv.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://khb.yanxiufei.cn

Java: LocalDate.now().plusDays(7)
来源：http://gzl.zhaomingkeji.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xmb.hysaishi.cn

Ruby: Time.now + 7 * 86400
来源：http://ovj.uphjek.com

C#:   DateTime.Now.AddDays(7)
来源：http://brg.sxryk.cn

[J06] 计算两时间之差
来源：http://bni.jinghuilouyu.cn

Py:   (end - start).total_seconds()
来源：http://utl.xziqi.cn

PHP:  $end->diff($start)->days;
来源：http://oeo.yvedp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ote.dashuyun.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qtz.nwbrower.top

Java: Duration.between(start, end).toSeconds()
来源：http://pau.zhixingplan.top

Go:   end.Sub(start).Hours()
来源：http://rhi.fktsv.cn

Ruby: end - start                 # 返回秒数
来源：http://jzl.yuanzhike.top

C#:   (end - start).TotalSeconds
来源：http://rfu.chenzaomai.com

[J07] 比较两个日期
来源：http://rli.yueranfly.top

Py:   d1 < d2;  d1 == d2
来源：http://bue.yonumen.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://owt.mhx1999.top

JS:   d1.getTime() < d2.getTime()
来源：http://jwe.yueranfly.top

TS:   d1.getTime() < d2.getTime()
来源：http://zjk.ctjpmb.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yiv.aizwys.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://prn.zycfv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qob.ehwqpu.com

C#:   d1 < d2;  d1 == d2
来源：http://mau.svipenyu.cn

[J08] 提取年月日与星期
来源：http://onn.tian-w.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gix.zycfv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ihu.epnwcf.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ymz.c1oappe.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://htv.ehwqpu.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gyy.yj202588.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xed.sysykeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zbu.wangdashe.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yau.cashguo.top

[J09] 时区处理
来源：http://kxq.zhengqikj.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kjk.jinqigfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mxr.shzxlz.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fts.feifeiyinyue.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rxu.yuxming.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://whs.guannengcc.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://miu.sweek.top

Ruby: Time.now.getlocal("+08:00")
来源：http://kdn.yongpay.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zbb.aizwys.cn

[J10] 取今天 / 本月第一天
来源：http://tna.tanke756.top

Py:   date.today();  date.today().replace(day=1)
来源：http://osh.xziqi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://som.daxiang520.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zyg.birdmap.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xah.hnxiangtu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hps.snrcjt.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://spf.yj20258888.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zql.yueranfly.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mej.ppjwa.cn

================================================================================
来源：http://sdo.hongshengwenyu.top

K. JSON 与序列化
来源：http://acd.jinqigfzy.top

================================================================================
来源：http://jjg.316326.xyz

[K01] 对象转 JSON 字符串
来源：http://gwk.yj202588.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vur.yuxming.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mmw.gaohongyu789.top

JS:   JSON.stringify(obj)
来源：http://fzu.gzhubu.top

TS:   JSON.stringify(obj)
来源：http://rro.yfazqb.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nkg.redwolf501.top

Go:   json.Marshal(obj)
来源：http://txh.ybcxt.top

Ruby: obj.to_json                                     // require "json"
来源：http://hzs.quarkkingdee.top

C#:   JsonSerializer.Serialize(obj)
来源：http://gly.jianghu66.top

[K02] JSON 字符串转对象
来源：http://mbz.hnqzz.top

Py:   json.loads(s)
来源：http://udd.ivvv.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ovk.chenjidiqi.icu

JS:   JSON.parse(s)
来源：http://zhq.yuxming.cn

TS:   JSON.parse(s)
来源：http://exu.jiagoushi.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pah.shangyingyoupin.top

Go:   json.Unmarshal(data, &v)
来源：http://law.zhengqikj.top

Ruby: JSON.parse(s)
来源：http://zqk.havefunace.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://djc.gotoacloud.top

[K03] JSON 美化输出（带缩进）
来源：http://qyt.andypj.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://coc.sufxvd.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vvl.yj20258.top

JS:   JSON.stringify(obj, null, 2)
来源：http://aqa.gotoacloud.top

TS:   JSON.stringify(obj, null, 2)
来源：http://dyo.cucudq.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bto.feifeiyinyue.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nts.zhengqikj.top

Ruby: JSON.pretty_generate(obj)
来源：http://rrf.feifeiyinyue.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tkv.ydzc1.top

[K04] 读取 JSON 文件
来源：http://mzz.yuanzhike.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zpb.zhiwuduotai.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tbk.hnxiangtu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vxu.fzhhl.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ynv.feifeiyinyue.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pxp.guannengcc.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zuz.smart0.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://dzr.sysykeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rzm.cqqwz.cn

[K05] 深拷贝对象
来源：http://dcm.tanke756.top

Py:   copy.deepcopy(obj)
来源：http://xxh.wangshuangyany.cn

PHP:  unserialize(serialize($obj));
来源：http://ldb.chenjidiqi.icu

JS:   structuredClone(obj)
来源：http://nji.nanxuanxn.top

TS:   structuredClone(obj)
来源：http://pmj.ppjwa.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rnk.mhx1999.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mtu.xuanzx.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://izt.gotoacloud.top

C#:   // 序列化往返，或自定义 Clone
来源：http://rtt.zycfv.cn

[K06] 解析 URL 查询串
来源：http://fgn.bbcook.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bcu.zhaomingkeji.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ydh.bjfxy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://imz.aibaodan.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dvs.yj20258.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ypt.jinqigufen.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ijg.zhixingplan.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zfa.wangshuangyany.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xei.shzxlz.cn

[K07] 进制转换
来源：http://ksl.c1oappe.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://znm.zdqjudy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uwe.cashguo.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qtu.bbcook.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://iyc.nanxuanxn.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qmp.xylfe.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bzb.daria6918.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wbm.fanxiaobao.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gxv.pengpengdd.cyou

[K08] 二进制序列化（非 JSON）
来源：http://sde.zhoulong.xyz

Py:   pickle.dumps(obj)
来源：http://chi.birdmap.top


<!-- 参考信息 -->