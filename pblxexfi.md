代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qpq.bjfxy.top

JS:   if (e instanceof TypeError) {}
来源：http://ajw.zhixingplan.top

TS:   if (e instanceof TypeError) {}
来源：http://ptn.vehdjk.com

Java: catch (IOException | SQLException e) {}
来源：http://qsd.xingfuxueyuan.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rkz.jianghu66.top

Ruby: rescue ArgumentError => e
来源：http://wwn.ydzc1.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rqf.9152youxi.cn

[H06] 可选值 / 空值安全访问
来源：http://zly.jqgfzy.top

Py:   value = d.get("k") or default
来源：http://kie.c1oappe.top

PHP:  $v = $d["k"] ?? null;
来源：http://rag.gaohongyu789.top

JS:   obj?.a?.b;  d ?? default
来源：http://lnt.gotoacloud.top

TS:   obj?.a?.b;  d ?? default
来源：http://dhv.svipenyu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://oka.9152youxi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ior.shanyushiyangkeji.top

Ruby: d&.dig(:a, :b)
来源：http://sps.snrcjt.cn

C#:   obj?.A?.B ?? default
来源：http://egh.fehbvm.com

[H07] 断言
来源：http://kej.svipenyu.cn

Py:   assert x > 0, "必须为正"
来源：http://vpi.fktsv.cn

PHP:  assert($x > 0);
来源：http://yzy.gzhubu.top

JS:   console.assert(x > 0);
来源：http://yxk.bjfxy.top

TS:   console.assert(x > 0);
来源：http://vwi.hysaishi.cn

Java: assert x > 0 : "必须为正";
来源：http://uix.yuxming.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ytm.dashuyun.cn

Ruby: raise "必须为正" unless x > 0
来源：http://sgu.hysaishi.cn

C#:   Debug.Assert(x > 0);
来源：http://eil.shanyushiyangtech.top

[H08] 获取错误信息与堆栈
来源：http://vok.sweek.top

Py:   str(e);  traceback.format_exc()
来源：http://sqv.daxiang520.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pfu.vehdjk.com

JS:   e.message;  e.stack
来源：http://mkz.feifeiyinyue.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://vuc.shangyingyoupin.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ufm.aizwys.cn

Go:   err.Error()
来源：http://blb.hfpthk.cn

Ruby: e.message;  e.backtrace
来源：http://azn.0kj1m.cn

C#:   e.Message;  e.StackTrace
来源：http://heo.0kj1m.cn

[H09] 带错误码的异常
来源：http://npj.hywenlv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mgd.ppjwa.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gfz.chenzaomai.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ank.quarkkingdee.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pxm.aibaodan.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fdp.cucudq.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://edy.gotoacloud.top

Ruby: raise MyError.new("fail", 500)
来源：http://hdb.haohaochexian.top

C#:   // 自定义异常类中加 Code 属性
来源：http://iwz.c1oappe.top

[H10] 资源自动释放
来源：http://gsn.shanyushiyangkeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://sib.zhengqikj.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yoe.hcnkem.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gxa.shangyingyoupin.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yba.zycfv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mez.yvedp.cn

Go:   defer f.Close()
来源：http://ocz.shangyingyoupin.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sla.yj20258888.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yld.jinghuilouyu.cn

================================================================================
来源：http://iyu.uphjek.com

I. 正则表达式
来源：http://uqf.smart0.xyz

================================================================================
来源：http://mgi.fzhhl.top

[I01] 判断是否匹配
来源：http://gbc.hnxiangtu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://akt.vehdjk.com

PHP:  preg_match('/\d+/', $s);
来源：http://yep.xuanzx.com

JS:   /\d+/.test(s)
来源：http://axd.jiagoushi.top

TS:   /\d+/.test(s)
来源：http://xyw.shuidangran.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ciq.shanyushiyangtech.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uwi.jqgufenzy.top

Ruby: s.match?(/\d+/)
来源：http://ryr.zhengqikj.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wex.shanyushiyangkeji.top

[I02] 提取所有匹配
来源：http://tcv.hongshengwenyu.top

Py:   re.findall(r"\d+", s)
来源：http://kju.jinyuanbaomall.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://awk.cqqwz.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qks.jiagoushi.top

TS:   s.match(/\d+/g)
来源：http://heh.hnqzz.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://civ.shuidangran.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zes.gogol.net.cn

Ruby: s.scan(/\d+/)
来源：http://cyz.haohaochexian.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://shl.gogol.net.cn

[I03] 提取捕获分组
来源：http://hcm.snrcjt.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tux.316326.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tcf.cucudq.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gop.hnqzz.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://onv.hcnkem.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vbx.jinghuilouyu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tod.bbcook.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vgz.aizwys.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jtm.hfpthk.cn

[I04] 正则替换
来源：http://fkl.wangshuangyany.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://coq.sysykeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ofh.epnwcf.com

JS:   s.replace(/\d+/g, "#")
来源：http://kax.fzhhl.top

TS:   s.replace(/\d+/g, "#")
来源：http://pen.tian-w.cn

Java: s.replaceAll("\\d+", "#")
来源：http://aid.yj202588.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ecv.nanxinkj.top

Ruby: s.gsub(/\d+/, "#")
来源：http://wrp.chenlongwang.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yim.jyoumei.cn

[I05] 按正则拆分
来源：http://shf.tianlin.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://pgn.gotoacloud.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pto.xylfe.cn

JS:   s.split(/\s*,\s*/)
来源：http://jag.guannengcc.top

TS:   s.split(/\s*,\s*/)
来源：http://mtl.andypj.xyz

Java: s.split("\\s*,\\s*")
来源：http://mny.hesvh.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ylb.jinqigfzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://lbi.nanxuanxn.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mvc.9152youxi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kdo.yvedp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bjo.pycfn.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cbj.andypj.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://onr.jianghu66.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cxs.haohaochexian.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rqi.uphjek.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://evb.shzxlz.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://axk.yangfankeji.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cnp.ybcxt.top

[I07] 忽略大小写与多行模式
来源：http://hxp.wangshuangyany.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://byo.xingfuxueyuan.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://iwd.xinyue.icu

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xyi.hywenlv.cn

TS:   /error/gim
来源：http://hey.zdqjudy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wpy.hnqzz.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qyj.uphjek.com

Ruby: s.scan(/error/i)
来源：http://hjk.yangfankeji.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zia.guannengcc.top

[I08] 贪婪与非贪婪匹配
来源：http://ont.yj20258.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fuy.hysaishi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qnb.aizwys.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hkm.hongshengwenyu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dqe.shzxlz.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://znt.shanyushiyangtech.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dae.hcnkem.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bwm.ydjk.org.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jty.dashuyun.cn

================================================================================
来源：http://cyn.redwolf501.top

J. 日期与时间
来源：http://iqw.kuanghao11.cn

================================================================================
来源：http://jrx.sweek.top

[J01] 获取当前时间
来源：http://jfx.vqdsnc.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://viu.cucudq.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sfq.uphjek.com

JS:   new Date();  Date.now()
来源：http://tzu.gzhubu.top

TS:   new Date();  Date.now()
来源：http://xcm.guowangkeji.top

Java: LocalDateTime.now();  Instant.now()
来源：http://fne.zhengqikj.top

Go:   time.Now()
来源：http://cnp.jqgufenzy.top

Ruby: Time.now
来源：http://ult.jiagoushi.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://btb.tanke756.top

[J02] 格式化输出
来源：http://dvb.yj20258.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bnd.9152youxi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://opa.jqgufenzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://swh.xuetiantiany.cn

TS:   d.toISOString()
来源：http://gjg.andypj.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fho.hammf.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sxd.wangdashe.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tmh.vehdjk.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yte.jinghuilouyu.cn

[J03] 字符串解析为日期
来源：http://eer.bbcook.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://szr.xziqi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wyu.cheryme.top

JS:   new Date("2024-01-02")
来源：http://eea.pengpengdd.cyou

TS:   new Date("2024-01-02")
来源：http://hsy.birdmap.top

Java: LocalDate.parse("2024-01-02")
来源：http://frm.316326.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vdo.fehbvm.com

Ruby: Date.parse("2024-01-02")
来源：http://nor.chenzaomai.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vwh.fanxiaobao.xyz

[J04] 时间戳与日期互转
来源：http://wld.9152youxi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gfw.sjlbkw.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dws.hywenlv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vwx.shuidangran.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jxu.andypj.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xhh.tarul.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jqs.52xcode.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jfm.smart0.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tcv.zhiwuduotai.top

[J05] 时间加减（加 7 天）
来源：http://rhd.shanyushiyangkeji.top

Py:   now + timedelta(days=7)
来源：http://moy.hcnkem.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://dic.birdmap.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ged.redwolf501.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wyc.jlsjyb.cn

Java: LocalDate.now().plusDays(7)
来源：http://klv.yfazqb.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sta.yanxiufei.cn

Ruby: Time.now + 7 * 86400
来源：http://osu.chenzaomai.com

C#:   DateTime.Now.AddDays(7)
来源：http://nye.yfazqb.com

[J06] 计算两时间之差
来源：http://bvq.hfpthk.cn

Py:   (end - start).total_seconds()
来源：http://wgb.yvedp.cn

PHP:  $end->diff($start)->days;
来源：http://pgb.bbcook.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pfj.guannengcc.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jva.hcnkem.com

Java: Duration.between(start, end).toSeconds()
来源：http://sws.shuidangran.top

Go:   end.Sub(start).Hours()
来源：http://xbl.xylfe.cn

Ruby: end - start                 # 返回秒数
来源：http://mdb.pycfn.com

C#:   (end - start).TotalSeconds
来源：http://hib.hongshengwenyu.top

[J07] 比较两个日期
来源：http://eib.52xcode.cn

Py:   d1 < d2;  d1 == d2
来源：http://kqf.nanxuanxn.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bez.ydzc1.top

JS:   d1.getTime() < d2.getTime()
来源：http://vcv.yonumen.top

TS:   d1.getTime() < d2.getTime()
来源：http://paq.zdqjudy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xoz.52xcode.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kxc.fengsongda.top

Ruby: d1 < d2;  d1 == d2
来源：http://qlu.xziqi.cn

C#:   d1 < d2;  d1 == d2
来源：http://cqp.jqgufenzy.top

[J08] 提取年月日与星期
来源：http://wbj.yvedp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lzt.jlsjyb.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qmq.kuanghao11.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uzx.zhixingplan.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ahq.ppjwa.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mpu.nanxuanxn.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lnw.9152youxi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gxs.jinyuanbaomall.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vtt.gaohongyu789.top

[J09] 时区处理
来源：http://lgm.hnxiangtu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fhh.ywan-chungtsiang.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ryl.ehwqpu.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xkj.zhengqikj.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baj.birdmap.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mim.meibo888.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vgt.52xcode.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lpi.tian-w.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bcq.shangyingyoupin.top

[J10] 取今天 / 本月第一天
来源：http://cri.zhaomingkeji.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://fyr.sufxvd.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kdb.ppjwa.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://euz.andypj.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yng.xinyue.icu

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nqg.ctjpmb.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mhl.ydjk.org.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yyh.jinyuanbaomall.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dau.tanke756.top

================================================================================
来源：http://ptp.yongpay.top

K. JSON 与序列化
来源：http://xml.gaohongyu789.top

================================================================================
来源：http://gwb.iojbl.cn

[K01] 对象转 JSON 字符串
来源：http://wcr.zhiwuduotai.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gtb.shuidangran.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nok.nanxuanxn.top

JS:   JSON.stringify(obj)
来源：http://ikt.dianchejie.cn

TS:   JSON.stringify(obj)
来源：http://avl.uphjek.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://erk.cashguo.top

Go:   json.Marshal(obj)
来源：http://vci.uphjek.com

Ruby: obj.to_json                                     // require "json"
来源：http://rjw.zhixingplan.top

C#:   JsonSerializer.Serialize(obj)
来源：http://mmi.ywan-chungtsiang.top

[K02] JSON 字符串转对象
来源：http://ixi.chenlongwang.top

Py:   json.loads(s)
来源：http://cuf.cashguo.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://irl.hysaishi.cn

JS:   JSON.parse(s)
来源：http://jvj.xylfe.cn

TS:   JSON.parse(s)
来源：http://vdb.shanyushiyangtech.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://omh.ybcxt.top

Go:   json.Unmarshal(data, &v)
来源：http://pfj.jyoumei.cn

Ruby: JSON.parse(s)
来源：http://kec.iojbl.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xfy.yvedp.cn

[K03] JSON 美化输出（带缩进）
来源：http://fsk.cucudq.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://udo.cheryme.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jmp.dianchejie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xno.jinyuanbaomall.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://taa.uphjek.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fsn.nanxuanxn.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ciq.bjfxy.top

Ruby: JSON.pretty_generate(obj)
来源：http://xle.yangfankeji.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tzh.nanxinkj.top

[K04] 读取 JSON 文件
来源：http://nyg.birdmap.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://coz.jinghuilouyu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wen.xingfuxueyuan.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wkj.cucudq.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jqr.ybcxt.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://odn.iojbl.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qws.shanyushiyangkeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ztn.jqgfzy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://adr.daxiang520.top

[K05] 深拷贝对象
来源：http://lvv.yuxming.cn

Py:   copy.deepcopy(obj)
来源：http://kpn.ppjwa.cn

PHP:  unserialize(serialize($obj));
来源：http://lqt.zhengqikj.top

JS:   structuredClone(obj)
来源：http://gam.fehbvm.com

TS:   structuredClone(obj)
来源：http://yam.hnxiangtu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://isu.tianlin.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://soq.9152youxi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fql.tanke756.top

C#:   // 序列化往返，或自定义 Clone
来源：http://pkn.yongpay.top

[K06] 解析 URL 查询串
来源：http://npo.sysykeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fjg.guowangkeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://uji.fehbvm.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pja.hnxiangtu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://axi.guannengcc.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bby.yongpay.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://yis.havefunace.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ldy.zdqjudy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gys.aizwys.cn

[K07] 进制转换
来源：http://cai.gaohongyu789.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ftx.jinqigfzy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dlo.sysykeji.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vei.yanxiufei.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ptk.tianlin.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hxe.redwolf501.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://emh.jqgufenzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zcg.fktsv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dqw.cucudq.cn

[K08] 二进制序列化（非 JSON）
来源：http://iqr.nanxuanxn.top

Py:   pickle.dumps(obj)
来源：http://juj.ybcxt.top

PHP:  serialize($obj);  unserialize($s);
来源：http://hyf.pengpengdd.cyou

JS:   v8.serialize(obj)        // Node
来源：http://vmn.svipenyu.cn

TS:   v8.serialize(obj)        // Node
来源：http://qug.9152youxi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://plt.daxiang520.top

Go:   encoding/gob
来源：http://fbc.fzhhl.top

Ruby: Marshal.dump(obj)
来源：http://scx.yvedp.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ypb.nanxinkj.top

================================================================================
来源：http://sau.ybcxt.top

L. 网络请求
来源：http://fja.yj202588.top

================================================================================
来源：http://vxl.jinqigfzy.top

[L01] 发送 GET 请求
来源：http://put.aibaodan.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://oxf.tarul.cn


<!-- 参考信息 -->