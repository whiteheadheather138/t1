代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bmc.hcnkem.com

JS:   if (e instanceof TypeError) {}
来源：http://ybh.ydjk.org.cn

TS:   if (e instanceof TypeError) {}
来源：http://caf.iojbl.cn

Java: catch (IOException | SQLException e) {}
来源：http://ubc.sufxvd.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fug.jinghuilouyu.cn

Ruby: rescue ArgumentError => e
来源：http://dpb.ybcxt.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sod.yfazqb.com

[H06] 可选值 / 空值安全访问
来源：http://pft.yj20258888.top

Py:   value = d.get("k") or default
来源：http://hum.yuanzhike.top

PHP:  $v = $d["k"] ?? null;
来源：http://lty.chenlongwang.top

JS:   obj?.a?.b;  d ?? default
来源：http://exc.xylfe.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cyg.hcnkem.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hsr.feifeiyinyue.top

Go:   if v, ok := m["k"]; ok { }
来源：http://rlp.yonumen.top

Ruby: d&.dig(:a, :b)
来源：http://uix.aizwys.cn

C#:   obj?.A?.B ?? default
来源：http://jxx.pengpengdd.cyou

[H07] 断言
来源：http://fse.shzxlz.cn

Py:   assert x > 0, "必须为正"
来源：http://uij.yongpay.top

PHP:  assert($x > 0);
来源：http://azr.ybcxt.top

JS:   console.assert(x > 0);
来源：http://bry.ivvv.top

TS:   console.assert(x > 0);
来源：http://wop.nanxuanxn.top

Java: assert x > 0 : "必须为正";
来源：http://mam.hywenlv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yxk.jinqigfzy.top

Ruby: raise "必须为正" unless x > 0
来源：http://uxn.jinghuilouyu.cn

C#:   Debug.Assert(x > 0);
来源：http://mrn.ctjpmb.com

[H08] 获取错误信息与堆栈
来源：http://nvg.yueranfly.top

Py:   str(e);  traceback.format_exc()
来源：http://qbz.fehbvm.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ewu.jqgufenzy.top

JS:   e.message;  e.stack
来源：http://ycn.sysykeji.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://nta.bjfxy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://reo.9152youxi.cn

Go:   err.Error()
来源：http://qsy.sjlbkw.cn

Ruby: e.message;  e.backtrace
来源：http://eov.fktsv.cn

C#:   e.Message;  e.StackTrace
来源：http://hcp.hammf.cn

[H09] 带错误码的异常
来源：http://qvf.yonumen.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dkr.zhiwuduotai.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ske.guannengcc.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mho.sjlbkw.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wug.zycfv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ikk.mhx1999.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ozx.xziqi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://udt.shangyingyoupin.top

C#:   // 自定义异常类中加 Code 属性
来源：http://yid.zdqjudy.top

[H10] 资源自动释放
来源：http://lcc.hammf.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://dxm.yanxiufei.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dti.cashguo.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mus.chenjidiqi.icu

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fex.aibaodan.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nwj.52xcode.cn

Go:   defer f.Close()
来源：http://edp.vehdjk.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vos.andypj.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mim.cheryme.top

================================================================================
来源：http://qqx.dianchejie.cn

I. 正则表达式
来源：http://wmg.bbcook.cn

================================================================================
来源：http://nwn.0kj1m.cn

[I01] 判断是否匹配
来源：http://fgq.cashguo.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dxm.hammf.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wyn.jianghu66.top

JS:   /\d+/.test(s)
来源：http://hak.xingfuxueyuan.xyz

TS:   /\d+/.test(s)
来源：http://qhg.cheryme.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cir.daria6918.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qyk.hnqzz.top

Ruby: s.match?(/\d+/)
来源：http://nnu.ybcxt.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cjl.cheryme.top

[I02] 提取所有匹配
来源：http://ntq.haohaochexian.top

Py:   re.findall(r"\d+", s)
来源：http://rik.jinghuilouyu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://toz.dashuyun.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lyq.bbcook.cn

TS:   s.match(/\d+/g)
来源：http://jfe.cashguo.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fcz.xziqi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fow.shangyingyoupin.top

Ruby: s.scan(/\d+/)
来源：http://bkf.tarul.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gca.hnqzz.top

[I03] 提取捕获分组
来源：http://sls.shanyushiyangtech.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wuz.pycfn.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lht.jianghu66.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hbz.sufxvd.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sbl.feifeiyinyue.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fho.ydzc1.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mxv.hnxiangtu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://utq.jinqigfzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ypm.jianghu66.top

[I04] 正则替换
来源：http://mcz.shanyushiyangkeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ggy.feifeiyinyue.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pqf.guowangkeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://fqp.ydzc1.top

TS:   s.replace(/\d+/g, "#")
来源：http://cxm.jyoumei.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ayo.fzhhl.top

Go:   re.ReplaceAllString(s, "#")
来源：http://wye.9152youxi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://rnf.yj20258888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dta.dianchejie.cn

[I05] 按正则拆分
来源：http://lpa.sjlbkw.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wte.yonumen.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://syk.epnwcf.com

JS:   s.split(/\s*,\s*/)
来源：http://jlt.ydjk.org.cn

TS:   s.split(/\s*,\s*/)
来源：http://yjf.feifeiyinyue.top

Java: s.split("\\s*,\\s*")
来源：http://vkb.jinghuilouyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://izf.yangfankeji.com

Ruby: s.split(/\s*,\s*/)
来源：http://xac.gzhubu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ird.tianlin.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://snh.sysykeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fte.9152youxi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rra.fanxiaobao.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cov.chenzaomai.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://afo.xylfe.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nha.wangdashe.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://deu.jinyuanbaomall.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bqz.sysykeji.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vvx.aibaodan.cn

[I07] 忽略大小写与多行模式
来源：http://uqv.shanyushiyangtech.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tzc.yfazqb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jem.yuanzhike.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://asv.cashguo.top

TS:   /error/gim
来源：http://for.jlsjyb.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cyq.sjlbkw.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qtn.0kj1m.cn

Ruby: s.scan(/error/i)
来源：http://mhg.zhijiandao.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kjd.vehdjk.com

[I08] 贪婪与非贪婪匹配
来源：http://zfe.ivvv.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sja.cashguo.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lkx.gzhubu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wvo.iojbl.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ydr.chenzaomai.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://ozt.yanxiufei.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wqn.sysykeji.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rys.9152youxi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zab.yuxming.cn

================================================================================
来源：http://xsg.andypj.xyz

J. 日期与时间
来源：http://klm.nwbrower.top

================================================================================
来源：http://vaj.xingfuxueyuan.xyz

[J01] 获取当前时间
来源：http://ofa.xylfe.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://jzt.ctjpmb.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wkm.redwolf501.top

JS:   new Date();  Date.now()
来源：http://daq.ctjpmb.com

TS:   new Date();  Date.now()
来源：http://kse.chenlongwang.top

Java: LocalDateTime.now();  Instant.now()
来源：http://rfk.meibo888.top

Go:   time.Now()
来源：http://beu.quarkkingdee.top

Ruby: Time.now
来源：http://ttp.nanxuanxn.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://grj.gaohongyu789.top

[J02] 格式化输出
来源：http://kxe.xinyue.icu

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://myo.ppjwa.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ral.yanxiufei.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ggp.hongshengwenyu.top

TS:   d.toISOString()
来源：http://vgg.hfpthk.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hqk.chenjidiqi.icu

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vpy.xuetiantiany.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bxz.jinqigfzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pcx.shzxlz.cn

[J03] 字符串解析为日期
来源：http://nhs.svipenyu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://iei.sufxvd.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bzh.hysaishi.cn

JS:   new Date("2024-01-02")
来源：http://yho.gogol.net.cn

TS:   new Date("2024-01-02")
来源：http://wyf.chenlongwang.top

Java: LocalDate.parse("2024-01-02")
来源：http://yxv.wangdashe.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gwj.hesvh.cn

Ruby: Date.parse("2024-01-02")
来源：http://btv.zhixingplan.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://way.ehwqpu.com

[J04] 时间戳与日期互转
来源：http://yve.bjfxy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dgm.gzhubu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ces.pengpengdd.cyou

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jew.c1oappe.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ixr.guannengcc.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hxt.zhixingplan.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://znl.jqgfzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://suo.shanyushiyangtech.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zbe.haohaochexian.top

[J05] 时间加减（加 7 天）
来源：http://xnz.bjfxy.top

Py:   now + timedelta(days=7)
来源：http://rnu.xziqi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://fef.yj202588.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kfz.xuetiantiany.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jhk.aizwys.cn

Java: LocalDate.now().plusDays(7)
来源：http://age.pycfn.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kzo.yanxiufei.cn

Ruby: Time.now + 7 * 86400
来源：http://aib.zhixingplan.top

C#:   DateTime.Now.AddDays(7)
来源：http://wvv.daria6918.cn

[J06] 计算两时间之差
来源：http://ayr.nanxinkj.top

Py:   (end - start).total_seconds()
来源：http://qyk.zhaomingkeji.xyz

PHP:  $end->diff($start)->days;
来源：http://hct.zdqjudy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gcc.hysaishi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pdf.pengpengdd.cyou

Java: Duration.between(start, end).toSeconds()
来源：http://ulf.xuanzx.com

Go:   end.Sub(start).Hours()
来源：http://ykl.xinyue.icu

Ruby: end - start                 # 返回秒数
来源：http://rby.fktsv.cn

C#:   (end - start).TotalSeconds
来源：http://fwt.daxiang520.top

[J07] 比较两个日期
来源：http://cdm.hysaishi.cn

Py:   d1 < d2;  d1 == d2
来源：http://pkx.yongpay.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bla.tian-w.cn

JS:   d1.getTime() < d2.getTime()
来源：http://guy.jlsjyb.cn

TS:   d1.getTime() < d2.getTime()
来源：http://iuk.zhiwuduotai.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hif.ydzc1.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://luo.yvedp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://src.yueranfly.top

C#:   d1 < d2;  d1 == d2
来源：http://ynm.xinyue.icu

[J08] 提取年月日与星期
来源：http://eza.sxryk.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zra.yj20258888.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bmd.hammf.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cfm.fzhhl.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uus.ppjwa.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pgt.jqgufenzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cyz.jinghuilouyu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://agq.fzhhl.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mpt.316326.xyz

[J09] 时区处理
来源：http://vgx.yuxming.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jea.cdnleiting.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wnz.yuxming.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xvc.jinghuilouyu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rov.yanxiufei.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ans.kuanghao11.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zay.ybcxt.top

Ruby: Time.now.getlocal("+08:00")
来源：http://agk.zhaomingkeji.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://trv.gogol.net.cn

[J10] 取今天 / 本月第一天
来源：http://pql.pengpengdd.cyou

Py:   date.today();  date.today().replace(day=1)
来源：http://zan.yuxming.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yzq.zycfv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kgo.hcnkem.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uqy.zhijiandao.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vwy.yuxming.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xuk.mhx1999.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ttb.pycfn.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qqx.shanyushiyangtech.top

================================================================================
来源：http://wyp.cashguo.top

K. JSON 与序列化
来源：http://mhd.hfpthk.cn

================================================================================
来源：http://qij.52xcode.cn

[K01] 对象转 JSON 字符串
来源：http://lac.zdqjudy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wkw.aibaodan.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kgi.jinyuanbaomall.cn

JS:   JSON.stringify(obj)
来源：http://ytg.wangshuangyany.cn

TS:   JSON.stringify(obj)
来源：http://vqk.jlsjyb.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zon.kuanghao11.cn

Go:   json.Marshal(obj)
来源：http://flm.yongpay.top

Ruby: obj.to_json                                     // require "json"
来源：http://mkz.shanyushiyangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://dsp.jinyuanbaomall.cn

[K02] JSON 字符串转对象
来源：http://fqg.ywan-chungtsiang.top

Py:   json.loads(s)
来源：http://syv.hfpthk.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fsc.aizwys.cn

JS:   JSON.parse(s)
来源：http://wnk.ppjwa.cn

TS:   JSON.parse(s)
来源：http://xpe.zhaomingkeji.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qkg.yj20258.top

Go:   json.Unmarshal(data, &v)
来源：http://fce.zdqjudy.top

Ruby: JSON.parse(s)
来源：http://oom.havefunace.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://guf.nwbrower.top

[K03] JSON 美化输出（带缩进）
来源：http://eas.ydjk.org.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gqc.hfpthk.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vda.quarkkingdee.top

JS:   JSON.stringify(obj, null, 2)
来源：http://fjc.dashuyun.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fmn.fanxiaobao.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xko.iojbl.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uxp.fanxiaobao.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://jle.gaohongyu789.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vza.zycfv.cn

[K04] 读取 JSON 文件
来源：http://tfr.zycfv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cbx.aizwys.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kdm.jinqigfzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cuw.c1oappe.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tzi.tanke756.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vws.zhoulong.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yat.xuetiantiany.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xrn.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oxl.bbcook.cn

[K05] 深拷贝对象
来源：http://yby.xinyue.icu

Py:   copy.deepcopy(obj)
来源：http://kom.iojbl.cn

PHP:  unserialize(serialize($obj));
来源：http://ltd.yuxming.cn

JS:   structuredClone(obj)
来源：http://tvr.xinyue.icu

TS:   structuredClone(obj)
来源：http://htx.ctjpmb.com

Java: // 手写拷贝构造，或序列化往返
来源：http://qhe.tanke756.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yto.chenzaomai.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nar.xziqi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://net.0kj1m.cn

[K06] 解析 URL 查询串
来源：http://zba.jiagoushi.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mtx.zhengqikj.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jql.ywan-chungtsiang.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nis.yanxiufei.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yjt.kuanghao11.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ycb.jinyuanbaomall.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://feg.zhengqikj.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ijj.316326.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hkc.xziqi.cn

[K07] 进制转换
来源：http://ykr.0kj1m.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pri.hysaishi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kvq.jqgufenzy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vwp.chenjidiqi.icu

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://loy.hywenlv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zel.jqgufenzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://exe.iojbl.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hcs.fengsongda.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kdu.smart0.xyz

[K08] 二进制序列化（非 JSON）
来源：http://ijm.jinyuanbaomall.cn

Py:   pickle.dumps(obj)
来源：http://evv.fengsongda.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ira.fzhhl.top

JS:   v8.serialize(obj)        // Node
来源：http://ugg.smart0.xyz

TS:   v8.serialize(obj)        // Node
来源：http://ydb.chenzaomai.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nlb.daxiang520.top

Go:   encoding/gob
来源：http://bhi.kuanghao11.cn

Ruby: Marshal.dump(obj)
来源：http://hna.uphjek.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lmy.zhiwuduotai.top

================================================================================
来源：http://jqc.shzxlz.cn

L. 网络请求
来源：http://gnz.ydjk.org.cn

================================================================================
来源：http://dvh.fanxiaobao.xyz

[L01] 发送 GET 请求
来源：http://vkh.fengsongda.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://aue.ivvv.top


<!-- 参考信息 -->