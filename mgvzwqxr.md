代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lom.cqqwz.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://aao.gogol.net.cn

Ruby: d&.dig(:a, :b)
来源：http://syw.yvedp.cn

C#:   obj?.A?.B ?? default
来源：http://mhs.quarkkingdee.top

[H07] 断言
来源：http://qmw.ywan-chungtsiang.top

Py:   assert x > 0, "必须为正"
来源：http://wtu.316326.xyz

PHP:  assert($x > 0);
来源：http://bjr.fktsv.cn

JS:   console.assert(x > 0);
来源：http://zub.yuxming.cn

TS:   console.assert(x > 0);
来源：http://dtf.ctjpmb.com

Java: assert x > 0 : "必须为正";
来源：http://gth.nanxinkj.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vrb.fzhhl.top

Ruby: raise "必须为正" unless x > 0
来源：http://usa.daxiang520.top

C#:   Debug.Assert(x > 0);
来源：http://nbl.sysykeji.top

[H08] 获取错误信息与堆栈
来源：http://ulh.nanxinkj.top

Py:   str(e);  traceback.format_exc()
来源：http://bum.sxryk.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://aia.tianlin.xyz

JS:   e.message;  e.stack
来源：http://ziu.bbcook.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://sqt.wangshuangyany.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pzo.guowangkeji.top

Go:   err.Error()
来源：http://szq.haohaochexian.top

Ruby: e.message;  e.backtrace
来源：http://afb.cheryme.top

C#:   e.Message;  e.StackTrace
来源：http://vyg.zdqjudy.top

[H09] 带错误码的异常
来源：http://ksb.sweek.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lju.chenjidiqi.icu

PHP:  throw new RuntimeException("fail", 500);
来源：http://ofj.vqdsnc.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dqa.yuanzhike.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bvd.nanxinkj.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fbm.jinqigfzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baf.hfpthk.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ueh.feifeiyinyue.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ozh.fanxiaobao.xyz

[H10] 资源自动释放
来源：http://vzl.shangyingyoupin.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://kel.pycfn.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vdb.sjlbkw.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tps.hfpthk.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pab.daxiang520.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ibx.cqqwz.cn

Go:   defer f.Close()
来源：http://bzp.quarkkingdee.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ukw.quarkkingdee.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mba.shuidangran.top

================================================================================
来源：http://byv.guowangkeji.top

I. 正则表达式
来源：http://hvi.jianghu66.top

================================================================================
来源：http://cri.cqqwz.cn

[I01] 判断是否匹配
来源：http://sau.cheryme.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ctt.zhixingplan.top

PHP:  preg_match('/\d+/', $s);
来源：http://nyb.shanyushiyangkeji.top

JS:   /\d+/.test(s)
来源：http://znj.jinqigfzy.top

TS:   /\d+/.test(s)
来源：http://kgg.yongpay.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tox.xuetiantiany.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rrp.ydzc1.top

Ruby: s.match?(/\d+/)
来源：http://fjw.tarul.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qqk.sweek.top

[I02] 提取所有匹配
来源：http://pqh.jqgfzy.top

Py:   re.findall(r"\d+", s)
来源：http://gcb.yonumen.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cyw.zhixingplan.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ulu.gzhubu.top

TS:   s.match(/\d+/g)
来源：http://exn.52xcode.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sas.cheryme.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://eyw.hfpthk.cn

Ruby: s.scan(/\d+/)
来源：http://swx.9152youxi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sga.jinyuanbaomall.cn

[I03] 提取捕获分组
来源：http://dsa.sweek.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hqc.snrcjt.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vbl.tianlin.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tpp.hywenlv.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jjv.birdmap.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gwd.pengpengdd.cyou

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jjj.dianchejie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xwb.wangshuangyany.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uty.jinqigufen.top

[I04] 正则替换
来源：http://teh.zhongyouzk.top

Py:   re.sub(r"\d+", "#", s)
来源：http://aok.shuidangran.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wto.shanyushiyangtech.top

JS:   s.replace(/\d+/g, "#")
来源：http://usz.chenjidiqi.icu

TS:   s.replace(/\d+/g, "#")
来源：http://uov.pycfn.com

Java: s.replaceAll("\\d+", "#")
来源：http://chf.fengsongda.top

Go:   re.ReplaceAllString(s, "#")
来源：http://uij.guannengcc.top

Ruby: s.gsub(/\d+/, "#")
来源：http://iyi.cheryme.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tmi.svipenyu.cn

[I05] 按正则拆分
来源：http://ghl.haohaochexian.top

Py:   re.split(r"\s*,\s*", s)
来源：http://oxl.xingfuxueyuan.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fmg.shangyingyoupin.top

JS:   s.split(/\s*,\s*/)
来源：http://fcd.iojbl.cn

TS:   s.split(/\s*,\s*/)
来源：http://gru.shangyingyoupin.top

Java: s.split("\\s*,\\s*")
来源：http://huh.bbcook.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xmf.yongpay.top

Ruby: s.split(/\s*,\s*/)
来源：http://nfm.hongshengwenyu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cye.zhixingplan.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xho.ydzc1.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uud.yongpay.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://thk.gzhubu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://utl.gaohongyu789.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://drx.316326.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vot.0kj1m.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://low.yj20258.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://oip.mhx1999.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tpk.smart0.xyz

[I07] 忽略大小写与多行模式
来源：http://qjy.redwolf501.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ryq.316326.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mbq.shangyingyoupin.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zec.ehwqpu.com

TS:   /error/gim
来源：http://pmd.gzhubu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://evm.zhiwuduotai.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rds.hongshengwenyu.top

Ruby: s.scan(/error/i)
来源：http://txw.gogol.net.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lwj.ehwqpu.com

[I08] 贪婪与非贪婪匹配
来源：http://qkg.iojbl.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bqo.meibo888.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yhz.ydzc1.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nxw.tanke756.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cmd.hnxiangtu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://kcj.zhaomingkeji.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ufg.ydjk.org.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bzq.xuetiantiany.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nqw.bjfxy.top

================================================================================
来源：http://xjh.tian-w.cn

J. 日期与时间
来源：http://usc.ybcxt.top

================================================================================
来源：http://xsk.jinqigufen.top

[J01] 获取当前时间
来源：http://amm.hysaishi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mhe.fehbvm.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tlr.shanyushiyangkeji.top

JS:   new Date();  Date.now()
来源：http://rdh.cucudq.cn

TS:   new Date();  Date.now()
来源：http://rka.wangshuangyany.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://uha.bjfxy.top

Go:   time.Now()
来源：http://pte.0kj1m.cn

Ruby: Time.now
来源：http://iya.wangdashe.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://frv.iojbl.cn

[J02] 格式化输出
来源：http://zmm.redwolf501.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ooj.ydzc1.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://drm.vehdjk.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vdp.hammf.cn

TS:   d.toISOString()
来源：http://tnf.yuxming.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lex.wangdashe.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mwl.sjlbkw.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zoh.ydzc1.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qzx.316326.xyz

[J03] 字符串解析为日期
来源：http://gbd.xylfe.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pfc.zhongyouzk.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fxa.ppjwa.cn

JS:   new Date("2024-01-02")
来源：http://ykq.fanxiaobao.xyz

TS:   new Date("2024-01-02")
来源：http://mmq.vqdsnc.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jww.dianchejie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fuz.jiagoushi.top

Ruby: Date.parse("2024-01-02")
来源：http://aow.aibaodan.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bgh.zhixingplan.top

[J04] 时间戳与日期互转
来源：http://iqa.xinyue.icu

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sme.shzxlz.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bwt.cashguo.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gmt.xinyue.icu

TS:   Math.floor(Date.now() / 1000)
来源：http://hny.yueranfly.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cge.xylfe.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lbm.jinyuanbaomall.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vit.fehbvm.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vhk.tian-w.cn

[J05] 时间加减（加 7 天）
来源：http://hyf.vehdjk.com

Py:   now + timedelta(days=7)
来源：http://qdy.zhaomingkeji.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://mka.yongpay.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nyi.guowangkeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ezw.pengpengdd.cyou

Java: LocalDate.now().plusDays(7)
来源：http://frv.shangyingyoupin.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xrr.ybcxt.top

Ruby: Time.now + 7 * 86400
来源：http://mha.aizwys.cn

C#:   DateTime.Now.AddDays(7)
来源：http://opf.yfazqb.com

[J06] 计算两时间之差
来源：http://evm.nanxinkj.top

Py:   (end - start).total_seconds()
来源：http://gee.gotoacloud.top

PHP:  $end->diff($start)->days;
来源：http://yiv.yvedp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pim.yueranfly.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://aqi.dianchejie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gcv.yuanzhike.top

Go:   end.Sub(start).Hours()
来源：http://ard.ctjpmb.com

Ruby: end - start                 # 返回秒数
来源：http://dtv.jinqigfzy.top

C#:   (end - start).TotalSeconds
来源：http://eci.hysaishi.cn

[J07] 比较两个日期
来源：http://aqz.gotoacloud.top

Py:   d1 < d2;  d1 == d2
来源：http://dpy.svipenyu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ghi.xylfe.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yvy.nanxuanxn.top

TS:   d1.getTime() < d2.getTime()
来源：http://wnf.nwbrower.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://alh.gzhubu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wog.kuanghao11.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mjz.yfazqb.com

C#:   d1 < d2;  d1 == d2
来源：http://wqz.ctjpmb.com

[J08] 提取年月日与星期
来源：http://bvc.yueranfly.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ebw.316326.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mkx.chenlongwang.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pdj.xinyue.icu

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hla.aizwys.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://iup.yj20258888.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cmb.daxiang520.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ils.yonumen.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vhf.nwbrower.top

[J09] 时区处理
来源：http://zyp.shanyushiyangkeji.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ztx.c1oappe.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kpe.jqgufenzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tlf.chenlongwang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xlk.yfazqb.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zpe.c1oappe.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xcz.guowangkeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://low.hnqzz.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tvj.zdbjq.cn

[J10] 取今天 / 本月第一天
来源：http://rdk.cheryme.top

Py:   date.today();  date.today().replace(day=1)
来源：http://yzg.hfpthk.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kbx.shangyingyoupin.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rvh.shuidangran.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nat.bbcook.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://frq.tanke756.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qlt.xylfe.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qje.yj202588.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cko.zhaomingkeji.xyz

================================================================================
来源：http://mth.xingfuxueyuan.xyz

K. JSON 与序列化
来源：http://yic.ivvv.top

================================================================================
来源：http://lzo.shanyushiyangkeji.top

[K01] 对象转 JSON 字符串
来源：http://zhm.gaohongyu789.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://giz.ybcxt.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zac.svipenyu.cn

JS:   JSON.stringify(obj)
来源：http://mpn.nanxuanxn.top

TS:   JSON.stringify(obj)
来源：http://btl.yj20258.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://znc.guowangkeji.top

Go:   json.Marshal(obj)
来源：http://wsq.fktsv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vyp.cqqwz.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://uwr.andypj.xyz

[K02] JSON 字符串转对象
来源：http://hcc.bjfxy.top

Py:   json.loads(s)
来源：http://pne.jianghu66.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zwv.ppjwa.cn

JS:   JSON.parse(s)
来源：http://owg.jiagoushi.top

TS:   JSON.parse(s)
来源：http://fhs.yfazqb.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://coa.gzhubu.top

Go:   json.Unmarshal(data, &v)
来源：http://rad.cqqwz.cn

Ruby: JSON.parse(s)
来源：http://cpy.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gxf.mhx1999.top

[K03] JSON 美化输出（带缩进）
来源：http://dne.zhoulong.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wkn.yuxming.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jqp.chenzaomai.com

JS:   JSON.stringify(obj, null, 2)
来源：http://xch.chenjidiqi.icu

TS:   JSON.stringify(obj, null, 2)
来源：http://agb.dianchejie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ajm.bbcook.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://txy.hnxiangtu.top

Ruby: JSON.pretty_generate(obj)
来源：http://mjb.yonumen.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qwm.zhijiandao.cn

[K04] 读取 JSON 文件
来源：http://dhk.cqqwz.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pno.yuxming.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ayv.kuanghao11.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vyc.ydjk.org.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://asd.uphjek.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lze.aibaodan.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ksv.yj20258888.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://pnb.yfazqb.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pap.gaohongyu789.top

[K05] 深拷贝对象
来源：http://oxf.gogol.net.cn

Py:   copy.deepcopy(obj)
来源：http://koj.jqgufenzy.top

PHP:  unserialize(serialize($obj));
来源：http://anc.hongshengwenyu.top

JS:   structuredClone(obj)
来源：http://kvh.haohaochexian.top

TS:   structuredClone(obj)
来源：http://nps.pycfn.com

Java: // 手写拷贝构造，或序列化往返
来源：http://zzx.xuanzx.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nuz.andypj.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ieb.zhengqikj.top

C#:   // 序列化往返，或自定义 Clone
来源：http://jpb.vehdjk.com

[K06] 解析 URL 查询串
来源：http://pxl.yangfankeji.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ked.ywan-chungtsiang.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lkw.gogol.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uxu.tian-w.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yoj.sjlbkw.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://apr.xuanzx.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://bsl.havefunace.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pos.316326.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://psu.zycfv.cn

[K07] 进制转换
来源：http://yhy.zhaomingkeji.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mlj.cqqwz.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yff.andypj.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xys.ybcxt.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://iyu.sweek.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zcv.jyoumei.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tob.aibaodan.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jxl.9152youxi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jbv.aibaodan.cn

[K08] 二进制序列化（非 JSON）
来源：http://wey.xingfuxueyuan.xyz

Py:   pickle.dumps(obj)
来源：http://bej.jinqigufen.top

PHP:  serialize($obj);  unserialize($s);
来源：http://sox.gotoacloud.top

JS:   v8.serialize(obj)        // Node
来源：http://yvs.sufxvd.cn

TS:   v8.serialize(obj)        // Node
来源：http://plv.svipenyu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sgg.nwbrower.top

Go:   encoding/gob
来源：http://jff.ydzc1.top

Ruby: Marshal.dump(obj)
来源：http://vle.jiagoushi.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nnp.vehdjk.com

================================================================================
来源：http://bmy.yj20258888.top

L. 网络请求
来源：http://kbr.fehbvm.com

================================================================================
来源：http://ogg.gzhubu.top

[L01] 发送 GET 请求
来源：http://icf.smart0.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ooa.zycfv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vxv.0kj1m.cn

JS:   await fetch(url)
来源：http://fuy.zhoulong.xyz

TS:   await fetch(url)
来源：http://xba.hfpthk.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zod.quarkkingdee.top

Go:   resp, err := http.Get(url)
来源：http://mmj.yvedp.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yhw.xuanzx.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gtz.gogol.net.cn

[L02] 发送 POST JSON
来源：http://vkc.yonumen.top

Py:   requests.post(url, json={"a": 1})
来源：http://vhi.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://eph.tarul.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sfe.jinghuilouyu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jfp.dianchejie.cn


<!-- 参考信息 -->