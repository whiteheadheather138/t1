代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://zcs.ydjk.org.cn

C#:   class MyException : Exception {}
来源：http://qmo.0kj1m.cn

[H05] 捕获特定类型
来源：http://qgp.jinyuanbaomall.cn

Py:   except ValueError as e:
来源：http://ktf.hfpthk.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kxv.chenzaomai.com

JS:   if (e instanceof TypeError) {}
来源：http://qpy.nanxinkj.top

TS:   if (e instanceof TypeError) {}
来源：http://xah.redwolf501.top

Java: catch (IOException | SQLException e) {}
来源：http://xwu.gogol.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://abn.nwbrower.top

Ruby: rescue ArgumentError => e
来源：http://gki.birdmap.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tze.xziqi.cn

[H06] 可选值 / 空值安全访问
来源：http://ueg.ppjwa.cn

Py:   value = d.get("k") or default
来源：http://lif.iojbl.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gxr.zhiwuduotai.top

JS:   obj?.a?.b;  d ?? default
来源：http://nay.yfazqb.com

TS:   obj?.a?.b;  d ?? default
来源：http://dfn.andypj.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bcy.vqdsnc.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ujj.fanxiaobao.xyz

Ruby: d&.dig(:a, :b)
来源：http://hov.bbcook.cn

C#:   obj?.A?.B ?? default
来源：http://ifo.epnwcf.com

[H07] 断言
来源：http://lfo.shanyushiyangkeji.top

Py:   assert x > 0, "必须为正"
来源：http://htv.316326.xyz

PHP:  assert($x > 0);
来源：http://agw.cucudq.cn

JS:   console.assert(x > 0);
来源：http://ijj.vqdsnc.cn

TS:   console.assert(x > 0);
来源：http://fqh.aizwys.cn

Java: assert x > 0 : "必须为正";
来源：http://hck.vehdjk.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lna.gotoacloud.top

Ruby: raise "必须为正" unless x > 0
来源：http://zhk.snrcjt.cn

C#:   Debug.Assert(x > 0);
来源：http://vwk.tarul.cn

[H08] 获取错误信息与堆栈
来源：http://woy.chenzaomai.com

Py:   str(e);  traceback.format_exc()
来源：http://deo.hysaishi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zrl.pengpengdd.cyou

JS:   e.message;  e.stack
来源：http://kjd.hnxiangtu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://lsz.snrcjt.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zrz.nanxuanxn.top

Go:   err.Error()
来源：http://ust.guannengcc.top

Ruby: e.message;  e.backtrace
来源：http://zqg.pycfn.com

C#:   e.Message;  e.StackTrace
来源：http://zpa.hammf.cn

[H09] 带错误码的异常
来源：http://fjx.yj202588.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nky.hcnkem.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://tce.chenlongwang.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nyc.guannengcc.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kfw.yuxming.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ghl.ydzc1.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mmj.sysykeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://kem.hcnkem.com

C#:   // 自定义异常类中加 Code 属性
来源：http://yma.cucudq.cn

[H10] 资源自动释放
来源：http://aid.dianchejie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ffw.shanyushiyangkeji.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ppy.cqqwz.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ynm.zhiwuduotai.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yxu.daria6918.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pae.fengsongda.top

Go:   defer f.Close()
来源：http://aef.chenlongwang.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://min.cqqwz.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tuy.kuanghao11.cn

================================================================================
来源：http://ibz.fehbvm.com

I. 正则表达式
来源：http://sgw.quarkkingdee.top

================================================================================
来源：http://rrq.ybcxt.top

[I01] 判断是否匹配
来源：http://zrv.nwbrower.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ene.gogol.net.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fbd.bbcook.cn

JS:   /\d+/.test(s)
来源：http://wom.zhongyouzk.top

TS:   /\d+/.test(s)
来源：http://wdk.yonumen.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mkw.aibaodan.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xpp.52xcode.cn

Ruby: s.match?(/\d+/)
来源：http://dgi.ydjk.org.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://twl.fzhhl.top

[I02] 提取所有匹配
来源：http://ile.yvedp.cn

Py:   re.findall(r"\d+", s)
来源：http://gzl.redwolf501.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tcz.hfpthk.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lyg.meibo888.top

TS:   s.match(/\d+/g)
来源：http://tyj.yanxiufei.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fnu.shzxlz.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rsq.tian-w.cn

Ruby: s.scan(/\d+/)
来源：http://lev.0kj1m.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tsj.jlsjyb.cn

[I03] 提取捕获分组
来源：http://khk.ppjwa.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wjh.yfazqb.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fxq.iojbl.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zkp.zhiwuduotai.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bon.hnqzz.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wxm.andypj.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://afg.nwbrower.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wum.xingfuxueyuan.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://acy.pycfn.com

[I04] 正则替换
来源：http://avv.xuetiantiany.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qzi.yangfankeji.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zjf.vehdjk.com

JS:   s.replace(/\d+/g, "#")
来源：http://fom.tarul.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yrt.sysykeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://mik.zycfv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://weq.svipenyu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://dao.fengsongda.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pmc.hnxiangtu.top

[I05] 按正则拆分
来源：http://awd.xingfuxueyuan.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://dit.tanke756.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qmf.hysaishi.cn

JS:   s.split(/\s*,\s*/)
来源：http://aly.c1oappe.top

TS:   s.split(/\s*,\s*/)
来源：http://pgs.nanxuanxn.top

Java: s.split("\\s*,\\s*")
来源：http://kqx.yanxiufei.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yyp.cheryme.top

Ruby: s.split(/\s*,\s*/)
来源：http://fwf.xinyue.icu

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zfd.tian-w.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gus.fanxiaobao.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fch.xinyue.icu

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pyy.guowangkeji.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dek.shanyushiyangtech.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vjv.wangshuangyany.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bpf.ywan-chungtsiang.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zcl.jinyuanbaomall.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://joi.uphjek.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tct.tianlin.xyz

[I07] 忽略大小写与多行模式
来源：http://eik.chenjidiqi.icu

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://oeu.xuetiantiany.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://avi.xziqi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kye.uphjek.com

TS:   /error/gim
来源：http://sqz.jqgufenzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yhj.fktsv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fft.yj20258888.top

Ruby: s.scan(/error/i)
来源：http://nkn.0kj1m.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://woj.gzhubu.top

[I08] 贪婪与非贪婪匹配
来源：http://pbg.smart0.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://isl.jinghuilouyu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://csf.xingfuxueyuan.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://boa.gotoacloud.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://srj.snrcjt.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gja.haohaochexian.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ecf.shzxlz.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ilj.daria6918.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vyw.0kj1m.cn

================================================================================
来源：http://eob.zhixingplan.top

J. 日期与时间
来源：http://bep.dianchejie.cn

================================================================================
来源：http://kdr.chenjidiqi.icu

[J01] 获取当前时间
来源：http://vao.sysykeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://jxn.havefunace.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ypn.ydjk.org.cn

JS:   new Date();  Date.now()
来源：http://pwo.ehwqpu.com

TS:   new Date();  Date.now()
来源：http://pwt.c1oappe.top

Java: LocalDateTime.now();  Instant.now()
来源：http://acs.hammf.cn

Go:   time.Now()
来源：http://rpl.xylfe.cn

Ruby: Time.now
来源：http://dcc.aibaodan.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gak.redwolf501.top

[J02] 格式化输出
来源：http://ndg.hnxiangtu.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mrp.hysaishi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vls.iojbl.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://eci.birdmap.top

TS:   d.toISOString()
来源：http://zxl.xingfuxueyuan.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pjv.iojbl.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://owp.zhiwuduotai.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bzo.gogol.net.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zzo.snrcjt.cn

[J03] 字符串解析为日期
来源：http://itg.cashguo.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nqt.bjfxy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fop.cucudq.cn

JS:   new Date("2024-01-02")
来源：http://gzw.sxryk.cn

TS:   new Date("2024-01-02")
来源：http://jeq.xingfuxueyuan.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://zzn.fzhhl.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://eut.zhoulong.xyz

Ruby: Date.parse("2024-01-02")
来源：http://umq.yongpay.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wjo.shanyushiyangtech.top

[J04] 时间戳与日期互转
来源：http://fsr.haohaochexian.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xwa.zhijiandao.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fdz.ppjwa.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nxf.yj20258.top

TS:   Math.floor(Date.now() / 1000)
来源：http://lnf.zdqjudy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ftc.xuanzx.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fcz.hnxiangtu.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://phk.tanke756.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mug.iojbl.cn

[J05] 时间加减（加 7 天）
来源：http://rwh.jlsjyb.cn

Py:   now + timedelta(days=7)
来源：http://ojs.tanke756.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://jtp.hnqzz.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pom.jyoumei.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ddh.ctjpmb.com

Java: LocalDate.now().plusDays(7)
来源：http://nox.yongpay.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ajz.tanke756.top

Ruby: Time.now + 7 * 86400
来源：http://sfo.pengpengdd.cyou

C#:   DateTime.Now.AddDays(7)
来源：http://pyx.vehdjk.com

[J06] 计算两时间之差
来源：http://lzz.xuanzx.com

Py:   (end - start).total_seconds()
来源：http://dfo.shanyushiyangtech.top

PHP:  $end->diff($start)->days;
来源：http://twz.uphjek.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kay.meibo888.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nrg.daxiang520.top

Java: Duration.between(start, end).toSeconds()
来源：http://ixl.shanyushiyangtech.top

Go:   end.Sub(start).Hours()
来源：http://leo.guannengcc.top

Ruby: end - start                 # 返回秒数
来源：http://dpr.daxiang520.top

C#:   (end - start).TotalSeconds
来源：http://hls.yfazqb.com

[J07] 比较两个日期
来源：http://htj.andypj.xyz

Py:   d1 < d2;  d1 == d2
来源：http://tar.jinqigufen.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fvj.jlsjyb.cn

JS:   d1.getTime() < d2.getTime()
来源：http://crr.yj20258.top

TS:   d1.getTime() < d2.getTime()
来源：http://zun.ywan-chungtsiang.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://slq.jyoumei.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://inr.jinqigfzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://zww.meibo888.top

C#:   d1 < d2;  d1 == d2
来源：http://frp.pycfn.com

[J08] 提取年月日与星期
来源：http://zgj.shangyingyoupin.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rnn.ydzc1.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sjl.yanxiufei.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jxq.ybcxt.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tum.chenzaomai.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xih.yj202588.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mej.xuanzx.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ohn.jinqigfzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nud.tanke756.top

[J09] 时区处理
来源：http://vit.meibo888.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vaw.ivvv.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nrf.yueranfly.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zsm.chenlongwang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://end.xuetiantiany.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://plm.cashguo.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qce.wangdashe.top

Ruby: Time.now.getlocal("+08:00")
来源：http://sip.cashguo.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hdh.dashuyun.cn

[J10] 取今天 / 本月第一天
来源：http://qfd.chenzaomai.com

Py:   date.today();  date.today().replace(day=1)
来源：http://vkl.ywan-chungtsiang.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://efj.fengsongda.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dqt.hfpthk.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://szw.cheryme.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ney.yj202588.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://oxg.zhaomingkeji.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rrz.wangshuangyany.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gtg.jlsjyb.cn

================================================================================
来源：http://cdj.gogol.net.cn

K. JSON 与序列化
来源：http://edp.yvedp.cn

================================================================================
来源：http://ezs.yj20258.top

[K01] 对象转 JSON 字符串
来源：http://gwk.hysaishi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hmx.ywan-chungtsiang.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ipu.tarul.cn

JS:   JSON.stringify(obj)
来源：http://pxr.zhiwuduotai.top

TS:   JSON.stringify(obj)
来源：http://rzq.guannengcc.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wob.hesvh.cn

Go:   json.Marshal(obj)
来源：http://tdg.zhaomingkeji.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://jfe.guannengcc.top

C#:   JsonSerializer.Serialize(obj)
来源：http://nqc.fengsongda.top

[K02] JSON 字符串转对象
来源：http://cdu.daria6918.cn

Py:   json.loads(s)
来源：http://tbx.vehdjk.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xdo.guannengcc.top

JS:   JSON.parse(s)
来源：http://rta.chenlongwang.top

TS:   JSON.parse(s)
来源：http://urg.9152youxi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dmq.chenlongwang.top

Go:   json.Unmarshal(data, &v)
来源：http://msb.wangshuangyany.cn

Ruby: JSON.parse(s)
来源：http://zqr.sjlbkw.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://osl.52xcode.cn

[K03] JSON 美化输出（带缩进）
来源：http://cii.sweek.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bde.hnxiangtu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zyz.jinghuilouyu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hst.tanke756.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wre.chenzaomai.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wlz.nwbrower.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ipl.zhijiandao.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wym.zhixingplan.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ayn.hcnkem.com

[K04] 读取 JSON 文件
来源：http://hqn.sxryk.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://izp.jyoumei.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fzh.gaohongyu789.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wnp.gogol.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wdu.mhx1999.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nro.daxiang520.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mot.ybcxt.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ayk.xuanzx.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fga.xingfuxueyuan.xyz

[K05] 深拷贝对象
来源：http://xld.daria6918.cn

Py:   copy.deepcopy(obj)
来源：http://zou.ivvv.top

PHP:  unserialize(serialize($obj));
来源：http://blu.shangyingyoupin.top

JS:   structuredClone(obj)
来源：http://ysv.fzhhl.top

TS:   structuredClone(obj)
来源：http://fco.meibo888.top

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.redwolf501.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ack.meibo888.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ffb.havefunace.top

C#:   // 序列化往返，或自定义 Clone
来源：http://tih.shanyushiyangkeji.top

[K06] 解析 URL 查询串
来源：http://brg.wangshuangyany.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nvg.nanxinkj.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gne.hcnkem.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oxd.havefunace.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lux.zycfv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cqb.0kj1m.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://jdj.yanxiufei.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xrl.ybcxt.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ewf.uphjek.com

[K07] 进制转换
来源：http://awb.uphjek.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gbd.meibo888.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mtn.yueranfly.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lbn.sjlbkw.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://asf.hongshengwenyu.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ogt.shangyingyoupin.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wml.jiagoushi.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kzy.jinqigufen.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zsa.fehbvm.com

[K08] 二进制序列化（非 JSON）
来源：http://lql.xylfe.cn

Py:   pickle.dumps(obj)
来源：http://vio.hesvh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://jjg.nanxuanxn.top

JS:   v8.serialize(obj)        // Node
来源：http://ycw.yangfankeji.com

TS:   v8.serialize(obj)        // Node
来源：http://xmy.sweek.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wjp.sjlbkw.cn

Go:   encoding/gob
来源：http://ekm.kuanghao11.cn

Ruby: Marshal.dump(obj)
来源：http://lpy.9152youxi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zea.ehwqpu.com

================================================================================
来源：http://zxw.andypj.xyz


<!-- 参考信息 -->