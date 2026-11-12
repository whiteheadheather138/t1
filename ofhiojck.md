代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://sbr.hnqzz.top

C#:   class MyException : Exception {}
来源：http://nec.zhengqikj.top

[H05] 捕获特定类型
来源：http://qei.shanyushiyangkeji.top

Py:   except ValueError as e:
来源：http://dkg.guannengcc.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dfz.jianghu66.top

JS:   if (e instanceof TypeError) {}
来源：http://edx.bbcook.cn

TS:   if (e instanceof TypeError) {}
来源：http://byv.aizwys.cn

Java: catch (IOException | SQLException e) {}
来源：http://amv.zhixingplan.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://saq.yanxiufei.cn

Ruby: rescue ArgumentError => e
来源：http://vjw.zhiwuduotai.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hpb.zhixingplan.top

[H06] 可选值 / 空值安全访问
来源：http://kso.yvedp.cn

Py:   value = d.get("k") or default
来源：http://ogp.daria6918.cn

PHP:  $v = $d["k"] ?? null;
来源：http://nrh.meibo888.top

JS:   obj?.a?.b;  d ?? default
来源：http://caf.iojbl.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rna.gotoacloud.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sdy.aizwys.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://rpq.jqgfzy.top

Ruby: d&.dig(:a, :b)
来源：http://jep.yj202588.top

C#:   obj?.A?.B ?? default
来源：http://npn.c1oappe.top

[H07] 断言
来源：http://wor.yj202588.top

Py:   assert x > 0, "必须为正"
来源：http://yxx.fzhhl.top

PHP:  assert($x > 0);
来源：http://gfd.cucudq.cn

JS:   console.assert(x > 0);
来源：http://gzn.fzhhl.top

TS:   console.assert(x > 0);
来源：http://bqg.xziqi.cn

Java: assert x > 0 : "必须为正";
来源：http://npu.zdqjudy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bqd.ppjwa.cn

Ruby: raise "必须为正" unless x > 0
来源：http://hos.tian-w.cn

C#:   Debug.Assert(x > 0);
来源：http://cyb.zhengqikj.top

[H08] 获取错误信息与堆栈
来源：http://cxy.zhixingplan.top

Py:   str(e);  traceback.format_exc()
来源：http://sry.nanxinkj.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jqa.ivvv.top

JS:   e.message;  e.stack
来源：http://hai.nanxuanxn.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://thj.xuetiantiany.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tzk.uphjek.com

Go:   err.Error()
来源：http://kpl.smart0.xyz

Ruby: e.message;  e.backtrace
来源：http://mpa.fengsongda.top

C#:   e.Message;  e.StackTrace
来源：http://zxk.nanxuanxn.top

[H09] 带错误码的异常
来源：http://rrd.ywan-chungtsiang.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hfa.xuanzx.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://mwx.316326.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bzb.jiagoushi.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wmr.jinqigufen.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ifa.gogol.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ppn.bjfxy.top

Ruby: raise MyError.new("fail", 500)
来源：http://mbt.zhixingplan.top

C#:   // 自定义异常类中加 Code 属性
来源：http://isf.daxiang520.top

[H10] 资源自动释放
来源：http://chc.ydzc1.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://dkc.kuanghao11.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xsa.redwolf501.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rdw.jlsjyb.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cst.9152youxi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kzt.quarkkingdee.top

Go:   defer f.Close()
来源：http://ycj.zdbjq.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qcc.snrcjt.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cji.snrcjt.cn

================================================================================
来源：http://qzj.meibo888.top

I. 正则表达式
来源：http://kbn.redwolf501.top

================================================================================
来源：http://iqg.nwbrower.top

[I01] 判断是否匹配
来源：http://wrn.pycfn.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sbc.ydjk.org.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gwz.fzhhl.top

JS:   /\d+/.test(s)
来源：http://zcz.sxryk.cn

TS:   /\d+/.test(s)
来源：http://jak.nanxuanxn.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nwo.gzhubu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://knc.quarkkingdee.top

Ruby: s.match?(/\d+/)
来源：http://cfb.jiagoushi.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lws.chenzaomai.com

[I02] 提取所有匹配
来源：http://blt.gotoacloud.top

Py:   re.findall(r"\d+", s)
来源：http://nuv.jqgufenzy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://shh.ivvv.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zmf.zycfv.cn

TS:   s.match(/\d+/g)
来源：http://dmz.zdqjudy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://alr.yvedp.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xxo.guowangkeji.top

Ruby: s.scan(/\d+/)
来源：http://ynb.yueranfly.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gxv.mhx1999.top

[I03] 提取捕获分组
来源：http://xsp.xziqi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kjk.iojbl.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vng.nanxuanxn.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vne.ivvv.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nub.zdqjudy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://htl.cdnleiting.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tui.shangyingyoupin.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kvk.daxiang520.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ufc.hongshengwenyu.top

[I04] 正则替换
来源：http://odn.fehbvm.com

Py:   re.sub(r"\d+", "#", s)
来源：http://pyb.gotoacloud.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xoy.hfpthk.cn

JS:   s.replace(/\d+/g, "#")
来源：http://eal.zdqjudy.top

TS:   s.replace(/\d+/g, "#")
来源：http://koq.pengpengdd.cyou

Java: s.replaceAll("\\d+", "#")
来源：http://woy.hongshengwenyu.top

Go:   re.ReplaceAllString(s, "#")
来源：http://mnq.zhijiandao.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nik.nwbrower.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://exc.xuanzx.com

[I05] 按正则拆分
来源：http://qmj.zhiwuduotai.top

Py:   re.split(r"\s*,\s*", s)
来源：http://vsb.yuxming.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ade.fanxiaobao.xyz

JS:   s.split(/\s*,\s*/)
来源：http://mfg.tarul.cn

TS:   s.split(/\s*,\s*/)
来源：http://cyn.shanyushiyangkeji.top

Java: s.split("\\s*,\\s*")
来源：http://cyq.xziqi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tqq.cucudq.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ywf.uphjek.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rhz.guannengcc.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xpw.tarul.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ezm.pycfn.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wfx.cashguo.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qwm.zhixingplan.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xzt.hfpthk.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://elm.tianlin.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zgi.jinqigfzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qod.sweek.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ini.9152youxi.cn

[I07] 忽略大小写与多行模式
来源：http://ggf.cucudq.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pde.yanxiufei.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://iyb.pycfn.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mxz.xingfuxueyuan.xyz

TS:   /error/gim
来源：http://jbg.havefunace.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ios.gaohongyu789.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://imr.pycfn.com

Ruby: s.scan(/error/i)
来源：http://atx.tanke756.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hog.cqqwz.cn

[I08] 贪婪与非贪婪匹配
来源：http://cso.shangyingyoupin.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nvi.haohaochexian.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://brg.wangdashe.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pqc.hnxiangtu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zlj.hcnkem.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://aed.gotoacloud.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ccn.ydzc1.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oie.dashuyun.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ovm.yuanzhike.top

================================================================================
来源：http://orr.tianlin.xyz

J. 日期与时间
来源：http://tka.hnxiangtu.top

================================================================================
来源：http://jqb.9152youxi.cn

[J01] 获取当前时间
来源：http://fng.guowangkeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://bmj.jinqigfzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kmh.nanxuanxn.top

JS:   new Date();  Date.now()
来源：http://zdh.jyoumei.cn

TS:   new Date();  Date.now()
来源：http://nin.shanyushiyangkeji.top

Java: LocalDateTime.now();  Instant.now()
来源：http://dks.haohaochexian.top

Go:   time.Now()
来源：http://tgr.vehdjk.com

Ruby: Time.now
来源：http://hgn.aizwys.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qfd.fktsv.cn

[J02] 格式化输出
来源：http://vgi.tanke756.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ene.vqdsnc.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://czc.epnwcf.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fnu.chenlongwang.top

TS:   d.toISOString()
来源：http://rsp.epnwcf.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bty.wangshuangyany.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rnq.chenjidiqi.icu

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://avs.hammf.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://iqy.yangfankeji.com

[J03] 字符串解析为日期
来源：http://qyg.ywan-chungtsiang.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sjr.jlsjyb.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jwx.zhijiandao.cn

JS:   new Date("2024-01-02")
来源：http://pws.yuanzhike.top

TS:   new Date("2024-01-02")
来源：http://myp.daria6918.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mor.sjlbkw.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ivm.ydjk.org.cn

Ruby: Date.parse("2024-01-02")
来源：http://kkz.gzhubu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://okl.jinqigfzy.top

[J04] 时间戳与日期互转
来源：http://gbl.yj20258888.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ofq.svipenyu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vkb.fanxiaobao.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://npc.dianchejie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://kzs.haohaochexian.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://whc.xylfe.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hap.fzhhl.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xvk.hongshengwenyu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://orm.shanyushiyangtech.top

[J05] 时间加减（加 7 天）
来源：http://oii.yueranfly.top

Py:   now + timedelta(days=7)
来源：http://nrz.zhijiandao.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ene.daria6918.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jvc.dashuyun.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ept.mhx1999.top

Java: LocalDate.now().plusDays(7)
来源：http://tfe.dianchejie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ibh.hywenlv.cn

Ruby: Time.now + 7 * 86400
来源：http://ghr.shzxlz.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dtp.52xcode.cn

[J06] 计算两时间之差
来源：http://kvo.fzhhl.top

Py:   (end - start).total_seconds()
来源：http://xxp.jlsjyb.cn

PHP:  $end->diff($start)->days;
来源：http://svh.zhiwuduotai.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ohu.yfazqb.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lmq.iojbl.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wtz.yuanzhike.top

Go:   end.Sub(start).Hours()
来源：http://ltn.andypj.xyz

Ruby: end - start                 # 返回秒数
来源：http://hcq.shzxlz.cn

C#:   (end - start).TotalSeconds
来源：http://qas.xuetiantiany.cn

[J07] 比较两个日期
来源：http://axp.daxiang520.top

Py:   d1 < d2;  d1 == d2
来源：http://gkh.ydzc1.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xnd.ppjwa.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qxw.nanxuanxn.top

TS:   d1.getTime() < d2.getTime()
来源：http://bbr.smart0.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pwu.yj202588.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://aoh.hysaishi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ldh.sjlbkw.cn

C#:   d1 < d2;  d1 == d2
来源：http://tbx.bjfxy.top

[J08] 提取年月日与星期
来源：http://vzd.gaohongyu789.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rrw.wangdashe.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://huc.bjfxy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mup.xingfuxueyuan.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xxq.cqqwz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xuh.cucudq.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mgs.snrcjt.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gin.mhx1999.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zuh.jyoumei.cn

[J09] 时区处理
来源：http://vws.iojbl.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lcf.52xcode.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ihp.yongpay.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yxg.xinyue.icu

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oia.jqgfzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rlv.hesvh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kpm.yj202588.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qca.yj20258888.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mkz.chenlongwang.top

[J10] 取今天 / 本月第一天
来源：http://poh.ybcxt.top

Py:   date.today();  date.today().replace(day=1)
来源：http://pwu.316326.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tzd.hfpthk.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bsu.jianghu66.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ksr.cucudq.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rzv.iojbl.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ola.chenlongwang.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lqj.dianchejie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wnh.cheryme.top

================================================================================
来源：http://cae.xinyue.icu

K. JSON 与序列化
来源：http://lew.wangdashe.top

================================================================================
来源：http://uro.hywenlv.cn

[K01] 对象转 JSON 字符串
来源：http://wnt.daxiang520.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xlc.tarul.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wht.tanke756.top

JS:   JSON.stringify(obj)
来源：http://gnd.zhixingplan.top

TS:   JSON.stringify(obj)
来源：http://otv.zhijiandao.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bfz.zhongyouzk.top

Go:   json.Marshal(obj)
来源：http://gdv.jinqigufen.top

Ruby: obj.to_json                                     // require "json"
来源：http://vgs.bjfxy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://pke.tarul.cn

[K02] JSON 字符串转对象
来源：http://xnp.zhongyouzk.top

Py:   json.loads(s)
来源：http://idp.sysykeji.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://psp.hammf.cn

JS:   JSON.parse(s)
来源：http://spd.jiagoushi.top

TS:   JSON.parse(s)
来源：http://mpd.ydjk.org.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://meu.yangfankeji.com

Go:   json.Unmarshal(data, &v)
来源：http://meg.gotoacloud.top

Ruby: JSON.parse(s)
来源：http://qod.yvedp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://aah.shangyingyoupin.top

[K03] JSON 美化输出（带缩进）
来源：http://mpb.gotoacloud.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vds.jinghuilouyu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://auv.hfpthk.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kot.yfazqb.com

TS:   JSON.stringify(obj, null, 2)
来源：http://ixh.redwolf501.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wbl.daria6918.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vhs.jyoumei.cn

Ruby: JSON.pretty_generate(obj)
来源：http://mdw.meibo888.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rtk.feifeiyinyue.top

[K04] 读取 JSON 文件
来源：http://hpj.sufxvd.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gsf.epnwcf.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qbr.zhongyouzk.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zoa.hnqzz.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ccb.aibaodan.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xpj.meibo888.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://inv.yuxming.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yzs.xylfe.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://aim.tian-w.cn

[K05] 深拷贝对象
来源：http://bdj.jinqigufen.top

Py:   copy.deepcopy(obj)
来源：http://ysj.hongshengwenyu.top

PHP:  unserialize(serialize($obj));
来源：http://abf.gaohongyu789.top

JS:   structuredClone(obj)
来源：http://kzi.hongshengwenyu.top

TS:   structuredClone(obj)
来源：http://udl.hfpthk.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fnt.yuanzhike.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fwy.ybcxt.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zhc.uphjek.com

C#:   // 序列化往返，或自定义 Clone
来源：http://pef.fengsongda.top

[K06] 解析 URL 查询串
来源：http://bxb.chenjidiqi.icu

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ycy.sufxvd.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wps.chenjidiqi.icu

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://aar.316326.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://puy.feifeiyinyue.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dhn.chenjidiqi.icu

Go:   url.ParseQuery("a=1&b=2")
来源：http://eiq.fzhhl.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cug.redwolf501.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xow.mhx1999.top

[K07] 进制转换
来源：http://qyq.aibaodan.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lxo.jinyuanbaomall.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ytq.svipenyu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dxj.wangdashe.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mel.dashuyun.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yse.cashguo.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nql.9152youxi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xnz.yj20258.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qqy.yuanzhike.top

[K08] 二进制序列化（非 JSON）
来源：http://nkw.zdqjudy.top

Py:   pickle.dumps(obj)
来源：http://cmm.tianlin.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://qvj.zhaomingkeji.xyz

JS:   v8.serialize(obj)        // Node
来源：http://jkd.ppjwa.cn

TS:   v8.serialize(obj)        // Node
来源：http://kpo.pycfn.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kvr.shanyushiyangkeji.top

Go:   encoding/gob
来源：http://rie.yj20258.top

Ruby: Marshal.dump(obj)
来源：http://fmn.pengpengdd.cyou

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fcr.pycfn.com

================================================================================
来源：http://rkg.nanxinkj.top


<!-- 参考信息 -->