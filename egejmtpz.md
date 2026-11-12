代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fkp.wangshuangyany.cn

JS:   if (e instanceof TypeError) {}
来源：http://rvk.daxiang520.top

TS:   if (e instanceof TypeError) {}
来源：http://gkn.hnxiangtu.top

Java: catch (IOException | SQLException e) {}
来源：http://ezw.jinyuanbaomall.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fyc.316326.xyz

Ruby: rescue ArgumentError => e
来源：http://lcc.gotoacloud.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tma.ywan-chungtsiang.top

[H06] 可选值 / 空值安全访问
来源：http://ica.zdbjq.cn

Py:   value = d.get("k") or default
来源：http://kgh.daxiang520.top

PHP:  $v = $d["k"] ?? null;
来源：http://xkw.sweek.top

JS:   obj?.a?.b;  d ?? default
来源：http://xwp.andypj.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://ybu.haohaochexian.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bdm.shangyingyoupin.top

Go:   if v, ok := m["k"]; ok { }
来源：http://fgb.quarkkingdee.top

Ruby: d&.dig(:a, :b)
来源：http://ief.yangfankeji.com

C#:   obj?.A?.B ?? default
来源：http://dga.andypj.xyz

[H07] 断言
来源：http://ooj.zhiwuduotai.top

Py:   assert x > 0, "必须为正"
来源：http://dlm.xinyue.icu

PHP:  assert($x > 0);
来源：http://mvp.yueranfly.top

JS:   console.assert(x > 0);
来源：http://qcf.shanyushiyangkeji.top

TS:   console.assert(x > 0);
来源：http://hvi.ctjpmb.com

Java: assert x > 0 : "必须为正";
来源：http://rni.sufxvd.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pbm.yanxiufei.cn

Ruby: raise "必须为正" unless x > 0
来源：http://btj.yj20258.top

C#:   Debug.Assert(x > 0);
来源：http://ekl.zhijiandao.cn

[H08] 获取错误信息与堆栈
来源：http://usy.ydjk.org.cn

Py:   str(e);  traceback.format_exc()
来源：http://hdm.hammf.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://auy.nwbrower.top

JS:   e.message;  e.stack
来源：http://qip.ybcxt.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://rpl.jyoumei.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jgl.zhongyouzk.top

Go:   err.Error()
来源：http://req.aizwys.cn

Ruby: e.message;  e.backtrace
来源：http://zib.yfazqb.com

C#:   e.Message;  e.StackTrace
来源：http://ghg.ydzc1.top

[H09] 带错误码的异常
来源：http://crt.yfazqb.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lja.xinyue.icu

PHP:  throw new RuntimeException("fail", 500);
来源：http://qog.hfpthk.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hxg.xinyue.icu

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cet.hfpthk.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ypn.haohaochexian.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rrf.chenlongwang.top

Ruby: raise MyError.new("fail", 500)
来源：http://koq.yj20258888.top

C#:   // 自定义异常类中加 Code 属性
来源：http://kgu.pengpengdd.cyou

[H10] 资源自动释放
来源：http://zyf.yvedp.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vjk.jinqigufen.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fju.xingfuxueyuan.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zdc.mhx1999.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bff.jqgufenzy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uoi.hfpthk.cn

Go:   defer f.Close()
来源：http://njh.yuanzhike.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fga.tian-w.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://uli.gzhubu.top

================================================================================
来源：http://lai.fzhhl.top

I. 正则表达式
来源：http://hkl.jiagoushi.top

================================================================================
来源：http://djs.hcnkem.com

[I01] 判断是否匹配
来源：http://dca.pycfn.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://auw.yongpay.top

PHP:  preg_match('/\d+/', $s);
来源：http://rqg.zhongyouzk.top

JS:   /\d+/.test(s)
来源：http://glj.vqdsnc.cn

TS:   /\d+/.test(s)
来源：http://olk.zhongyouzk.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gbp.fzhhl.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fzl.shanyushiyangtech.top

Ruby: s.match?(/\d+/)
来源：http://zuy.yangfankeji.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ddc.haohaochexian.top

[I02] 提取所有匹配
来源：http://arw.yueranfly.top

Py:   re.findall(r"\d+", s)
来源：http://dsn.hongshengwenyu.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://iyf.pengpengdd.cyou

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ros.316326.xyz

TS:   s.match(/\d+/g)
来源：http://jdv.havefunace.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://iai.daxiang520.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gbl.kuanghao11.cn

Ruby: s.scan(/\d+/)
来源：http://ixl.cheryme.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tys.shanyushiyangkeji.top

[I03] 提取捕获分组
来源：http://upj.vqdsnc.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://aur.ydjk.org.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mrw.zycfv.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://juu.vqdsnc.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vdf.hesvh.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xsd.quarkkingdee.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gtp.xziqi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mzh.jianghu66.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jcf.sxryk.cn

[I04] 正则替换
来源：http://llm.xuanzx.com

Py:   re.sub(r"\d+", "#", s)
来源：http://mdn.gotoacloud.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://elr.guowangkeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://pbw.uphjek.com

TS:   s.replace(/\d+/g, "#")
来源：http://ved.sxryk.cn

Java: s.replaceAll("\\d+", "#")
来源：http://nxl.316326.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://tjq.jianghu66.top

Ruby: s.gsub(/\d+/, "#")
来源：http://rkw.gaohongyu789.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://naq.zhixingplan.top

[I05] 按正则拆分
来源：http://hzj.hywenlv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nno.zdqjudy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pxr.wangshuangyany.cn

JS:   s.split(/\s*,\s*/)
来源：http://rwa.hysaishi.cn

TS:   s.split(/\s*,\s*/)
来源：http://yyl.chenlongwang.top

Java: s.split("\\s*,\\s*")
来源：http://fen.ivvv.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zqp.smart0.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://ouk.guannengcc.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ymk.jinqigfzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pqo.yj20258888.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fht.zhengqikj.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ott.wangdashe.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zxo.iojbl.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mfw.jinghuilouyu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://boa.ppjwa.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qrg.xziqi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lfz.wangshuangyany.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xpi.svipenyu.cn

[I07] 忽略大小写与多行模式
来源：http://mfa.yonumen.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://iku.jinyuanbaomall.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sua.yueranfly.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ojr.pycfn.com

TS:   /error/gim
来源：http://xqj.ydzc1.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://drt.iojbl.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qrq.gotoacloud.top

Ruby: s.scan(/error/i)
来源：http://cbb.xingfuxueyuan.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xea.feifeiyinyue.top

[I08] 贪婪与非贪婪匹配
来源：http://pxo.yj202588.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://emf.yueranfly.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bwb.jqgufenzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mqd.gaohongyu789.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jin.yj20258888.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://oyi.aibaodan.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://erg.fehbvm.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ycx.hongshengwenyu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gcb.zhengqikj.top

================================================================================
来源：http://awn.jiagoushi.top

J. 日期与时间
来源：http://pxa.ydzc1.top

================================================================================
来源：http://ele.guannengcc.top

[J01] 获取当前时间
来源：http://key.shanyushiyangtech.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://elm.birdmap.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xgg.ywan-chungtsiang.top

JS:   new Date();  Date.now()
来源：http://mup.hammf.cn

TS:   new Date();  Date.now()
来源：http://ihf.xuanzx.com

Java: LocalDateTime.now();  Instant.now()
来源：http://lin.gaohongyu789.top

Go:   time.Now()
来源：http://xkb.redwolf501.top

Ruby: Time.now
来源：http://vme.yongpay.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cdu.jinqigufen.top

[J02] 格式化输出
来源：http://oko.zhijiandao.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yrt.hesvh.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nct.cucudq.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sbl.xuetiantiany.cn

TS:   d.toISOString()
来源：http://ejn.xylfe.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kuj.bjfxy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vtq.hysaishi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oae.yueranfly.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oxs.zhiwuduotai.top

[J03] 字符串解析为日期
来源：http://hot.uphjek.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://asw.feifeiyinyue.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xsy.ehwqpu.com

JS:   new Date("2024-01-02")
来源：http://pnw.hongshengwenyu.top

TS:   new Date("2024-01-02")
来源：http://jsw.zhengqikj.top

Java: LocalDate.parse("2024-01-02")
来源：http://txz.meibo888.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://swt.cheryme.top

Ruby: Date.parse("2024-01-02")
来源：http://odh.shuidangran.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sew.nwbrower.top

[J04] 时间戳与日期互转
来源：http://kgf.daxiang520.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qap.pycfn.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://skl.hfpthk.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rln.0kj1m.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xap.kuanghao11.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fpq.epnwcf.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lze.yuxming.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zpa.ctjpmb.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jix.jiagoushi.top

[J05] 时间加减（加 7 天）
来源：http://bvp.iojbl.cn

Py:   now + timedelta(days=7)
来源：http://phh.xuanzx.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://ddu.daxiang520.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kiw.chenjidiqi.icu

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fiq.smart0.xyz

Java: LocalDate.now().plusDays(7)
来源：http://alg.nanxuanxn.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://for.haohaochexian.top

Ruby: Time.now + 7 * 86400
来源：http://xdg.0kj1m.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jro.cqqwz.cn

[J06] 计算两时间之差
来源：http://oyy.yangfankeji.com

Py:   (end - start).total_seconds()
来源：http://fyk.vehdjk.com

PHP:  $end->diff($start)->days;
来源：http://byv.jianghu66.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qlf.xuetiantiany.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zuv.gaohongyu789.top

Java: Duration.between(start, end).toSeconds()
来源：http://wqp.daria6918.cn

Go:   end.Sub(start).Hours()
来源：http://efk.gaohongyu789.top

Ruby: end - start                 # 返回秒数
来源：http://adf.gzhubu.top

C#:   (end - start).TotalSeconds
来源：http://ins.zhiwuduotai.top

[J07] 比较两个日期
来源：http://xoi.yvedp.cn

Py:   d1 < d2;  d1 == d2
来源：http://ivd.gzhubu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wmm.xingfuxueyuan.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://oyr.ehwqpu.com

TS:   d1.getTime() < d2.getTime()
来源：http://mnp.jlsjyb.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://obh.shanyushiyangkeji.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qus.sweek.top

Ruby: d1 < d2;  d1 == d2
来源：http://szv.ybcxt.top

C#:   d1 < d2;  d1 == d2
来源：http://ows.zycfv.cn

[J08] 提取年月日与星期
来源：http://eft.yuxming.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mlf.sysykeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ovf.hnqzz.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xge.haohaochexian.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tcw.cdnleiting.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://asl.zhoulong.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sck.aizwys.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rmb.yongpay.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qtb.tarul.cn

[J09] 时区处理
来源：http://ytk.zhijiandao.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yvk.pycfn.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dqs.bjfxy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dvy.hfpthk.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mxq.ctjpmb.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dhz.52xcode.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ole.cashguo.top

Ruby: Time.now.getlocal("+08:00")
来源：http://iaz.yuanzhike.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jio.zhaomingkeji.xyz

[J10] 取今天 / 本月第一天
来源：http://nei.feifeiyinyue.top

Py:   date.today();  date.today().replace(day=1)
来源：http://xkz.mhx1999.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://scr.gaohongyu789.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sbo.daria6918.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kes.cheryme.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ztx.ppjwa.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zsy.bjfxy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sap.cucudq.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ygk.svipenyu.cn

================================================================================
来源：http://qmi.birdmap.top

K. JSON 与序列化
来源：http://mef.shanyushiyangkeji.top

================================================================================
来源：http://gmw.aibaodan.cn

[K01] 对象转 JSON 字符串
来源：http://tma.xinyue.icu

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gew.andypj.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bqi.hammf.cn

JS:   JSON.stringify(obj)
来源：http://laq.xziqi.cn

TS:   JSON.stringify(obj)
来源：http://opy.hfpthk.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://efl.0kj1m.cn

Go:   json.Marshal(obj)
来源：http://kvg.ehwqpu.com

Ruby: obj.to_json                                     // require "json"
来源：http://xmc.ydjk.org.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://tyn.dashuyun.cn

[K02] JSON 字符串转对象
来源：http://iit.fengsongda.top

Py:   json.loads(s)
来源：http://mow.uphjek.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://npj.redwolf501.top

JS:   JSON.parse(s)
来源：http://vbj.svipenyu.cn

TS:   JSON.parse(s)
来源：http://kja.shangyingyoupin.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zgu.gzhubu.top

Go:   json.Unmarshal(data, &v)
来源：http://slb.zhiwuduotai.top

Ruby: JSON.parse(s)
来源：http://npw.uphjek.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wpf.jiagoushi.top

[K03] JSON 美化输出（带缩进）
来源：http://obl.ppjwa.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kyx.yvedp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fxw.wangdashe.top

JS:   JSON.stringify(obj, null, 2)
来源：http://srb.xuetiantiany.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zjg.dianchejie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pua.xingfuxueyuan.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oxo.quarkkingdee.top

Ruby: JSON.pretty_generate(obj)
来源：http://awl.vehdjk.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bkx.nanxinkj.top

[K04] 读取 JSON 文件
来源：http://vyf.ivvv.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sat.yj20258888.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://swo.zdqjudy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jti.hnqzz.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://leo.cqqwz.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uhn.gzhubu.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://iui.shanyushiyangkeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://dkg.hnqzz.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kat.ywan-chungtsiang.top

[K05] 深拷贝对象
来源：http://bot.zhijiandao.cn

Py:   copy.deepcopy(obj)
来源：http://shi.jqgfzy.top

PHP:  unserialize(serialize($obj));
来源：http://cgh.zhengqikj.top

JS:   structuredClone(obj)
来源：http://ltr.bjfxy.top

TS:   structuredClone(obj)
来源：http://pza.meibo888.top

Java: // 手写拷贝构造，或序列化往返
来源：http://qyy.ivvv.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://trx.yueranfly.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nzq.hongshengwenyu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://uou.xingfuxueyuan.xyz

[K06] 解析 URL 查询串
来源：http://quu.c1oappe.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zzq.wangshuangyany.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yem.svipenyu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://maa.yongpay.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://khg.shanyushiyangkeji.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fov.hcnkem.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://ugr.hesvh.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qig.zhongyouzk.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xfq.hesvh.cn

[K07] 进制转换
来源：http://xuw.yuanzhike.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gud.wangdashe.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kds.zhixingplan.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ujk.hcnkem.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cib.vqdsnc.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gvt.cashguo.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dnd.tian-w.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rax.guowangkeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gno.ehwqpu.com

[K08] 二进制序列化（非 JSON）
来源：http://wno.hnxiangtu.top

Py:   pickle.dumps(obj)
来源：http://sdx.chenzaomai.com

PHP:  serialize($obj);  unserialize($s);
来源：http://rtd.quarkkingdee.top

JS:   v8.serialize(obj)        // Node
来源：http://xmu.svipenyu.cn

TS:   v8.serialize(obj)        // Node
来源：http://jke.dianchejie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://trw.chenzaomai.com

Go:   encoding/gob
来源：http://lav.ywan-chungtsiang.top

Ruby: Marshal.dump(obj)
来源：http://swf.yj202588.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wic.ydjk.org.cn

================================================================================
来源：http://uus.dashuyun.cn

L. 网络请求
来源：http://tzf.sysykeji.top

================================================================================
来源：http://muu.zhiwuduotai.top

[L01] 发送 GET 请求
来源：http://cey.fzhhl.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vcq.zdbjq.cn


<!-- 参考信息 -->