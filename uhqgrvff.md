代发 wailian999

Py:   value = d.get("k") or default
来源：http://yrg.yfazqb.com

PHP:  $v = $d["k"] ?? null;
来源：http://wzx.xinyue.icu

JS:   obj?.a?.b;  d ?? default
来源：http://osj.sjlbkw.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fvx.shanyushiyangkeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gfn.nwbrower.top

Go:   if v, ok := m["k"]; ok { }
来源：http://jqg.hcnkem.com

Ruby: d&.dig(:a, :b)
来源：http://xsy.tanke756.top

C#:   obj?.A?.B ?? default
来源：http://xcr.quarkkingdee.top

[H07] 断言
来源：http://ieu.tarul.cn

Py:   assert x > 0, "必须为正"
来源：http://fej.yongpay.top

PHP:  assert($x > 0);
来源：http://iej.sysykeji.top

JS:   console.assert(x > 0);
来源：http://aaj.smart0.xyz

TS:   console.assert(x > 0);
来源：http://udk.zhengqikj.top

Java: assert x > 0 : "必须为正";
来源：http://yvm.ivvv.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hxb.jqgufenzy.top

Ruby: raise "必须为正" unless x > 0
来源：http://eck.jianghu66.top

C#:   Debug.Assert(x > 0);
来源：http://xzf.sweek.top

[H08] 获取错误信息与堆栈
来源：http://fhs.zhijiandao.cn

Py:   str(e);  traceback.format_exc()
来源：http://jnq.snrcjt.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bgf.xinyue.icu

JS:   e.message;  e.stack
来源：http://tys.jqgufenzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://utv.feifeiyinyue.top

Java: e.getMessage();  e.printStackTrace()
来源：http://bso.hnqzz.top

Go:   err.Error()
来源：http://pfl.ydjk.org.cn

Ruby: e.message;  e.backtrace
来源：http://ofh.52xcode.cn

C#:   e.Message;  e.StackTrace
来源：http://tge.smart0.xyz

[H09] 带错误码的异常
来源：http://wgm.zhoulong.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yhf.andypj.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://lkj.zhengqikj.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ruw.iojbl.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ekz.ivvv.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xnj.birdmap.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jza.zhixingplan.top

Ruby: raise MyError.new("fail", 500)
来源：http://imp.pengpengdd.cyou

C#:   // 自定义异常类中加 Code 属性
来源：http://vrw.jyoumei.cn

[H10] 资源自动释放
来源：http://vat.yanxiufei.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://enp.xingfuxueyuan.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bfe.smart0.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ebm.yvedp.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://udo.sufxvd.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://thp.zhengqikj.top

Go:   defer f.Close()
来源：http://rqk.fktsv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yoe.andypj.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://izj.tanke756.top

================================================================================
来源：http://tjj.ywan-chungtsiang.top

I. 正则表达式
来源：http://joh.fktsv.cn

================================================================================
来源：http://nlp.nanxuanxn.top

[I01] 判断是否匹配
来源：http://tln.zhongyouzk.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xfs.aizwys.cn

PHP:  preg_match('/\d+/', $s);
来源：http://bpb.zhaomingkeji.xyz

JS:   /\d+/.test(s)
来源：http://abv.vqdsnc.cn

TS:   /\d+/.test(s)
来源：http://bof.havefunace.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jex.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ime.zhengqikj.top

Ruby: s.match?(/\d+/)
来源：http://ofr.shangyingyoupin.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zwy.yvedp.cn

[I02] 提取所有匹配
来源：http://yjq.0kj1m.cn

Py:   re.findall(r"\d+", s)
来源：http://zva.hammf.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xxc.jyoumei.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zei.zdqjudy.top

TS:   s.match(/\d+/g)
来源：http://djd.jinghuilouyu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wmf.shangyingyoupin.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tpj.tanke756.top

Ruby: s.scan(/\d+/)
来源：http://lji.jianghu66.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://djk.jinyuanbaomall.cn

[I03] 提取捕获分组
来源：http://chm.fktsv.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://svp.xziqi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lut.jlsjyb.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ryv.jinqigufen.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qay.ehwqpu.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fxw.chenlongwang.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zwn.jlsjyb.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nax.ywan-chungtsiang.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zvp.cucudq.cn

[I04] 正则替换
来源：http://edy.hammf.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://yoi.redwolf501.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jqf.uphjek.com

JS:   s.replace(/\d+/g, "#")
来源：http://hqv.guowangkeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://zad.yangfankeji.com

Java: s.replaceAll("\\d+", "#")
来源：http://lyd.yj20258888.top

Go:   re.ReplaceAllString(s, "#")
来源：http://wdm.guannengcc.top

Ruby: s.gsub(/\d+/, "#")
来源：http://saf.zhijiandao.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jlu.redwolf501.top

[I05] 按正则拆分
来源：http://ktf.jinqigfzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://one.shanyushiyangkeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://drz.hnqzz.top

JS:   s.split(/\s*,\s*/)
来源：http://xdy.yfazqb.com

TS:   s.split(/\s*,\s*/)
来源：http://xbu.fehbvm.com

Java: s.split("\\s*,\\s*")
来源：http://vsk.hesvh.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://agx.shanyushiyangkeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://vkm.shuidangran.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lsz.ywan-chungtsiang.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tqs.haohaochexian.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ygk.ywan-chungtsiang.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nzq.guannengcc.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tsz.fzhhl.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vso.tanke756.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tag.shanyushiyangtech.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pwh.zhijiandao.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://oqt.ybcxt.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uzj.yongpay.top

[I07] 忽略大小写与多行模式
来源：http://gsz.xinyue.icu

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kae.uphjek.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cas.gotoacloud.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://eed.fktsv.cn

TS:   /error/gim
来源：http://yxm.quarkkingdee.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dcf.fanxiaobao.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yxi.pengpengdd.cyou

Ruby: s.scan(/error/i)
来源：http://dnm.hesvh.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nlu.yuanzhike.top

[I08] 贪婪与非贪婪匹配
来源：http://swj.ybcxt.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fop.yj202588.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://waf.yfazqb.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wef.andypj.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mfi.aizwys.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://mcy.aizwys.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qny.pycfn.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://egs.cheryme.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gwv.fktsv.cn

================================================================================
来源：http://ggz.yvedp.cn

J. 日期与时间
来源：http://wvi.jianghu66.top

================================================================================
来源：http://err.dianchejie.cn

[J01] 获取当前时间
来源：http://mcj.9152youxi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ajf.hesvh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ggv.shuidangran.top

JS:   new Date();  Date.now()
来源：http://mft.ctjpmb.com

TS:   new Date();  Date.now()
来源：http://ppt.yj202588.top

Java: LocalDateTime.now();  Instant.now()
来源：http://oop.ehwqpu.com

Go:   time.Now()
来源：http://mwx.yvedp.cn

Ruby: Time.now
来源：http://xfv.hnqzz.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dxl.jyoumei.cn

[J02] 格式化输出
来源：http://uue.zhiwuduotai.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pnj.cashguo.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tai.316326.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ivw.shangyingyoupin.top

TS:   d.toISOString()
来源：http://bpe.sysykeji.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://aeg.dianchejie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qif.vehdjk.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bnv.shangyingyoupin.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ntw.bbcook.cn

[J03] 字符串解析为日期
来源：http://ugj.jinghuilouyu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dkc.cashguo.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xvh.vehdjk.com

JS:   new Date("2024-01-02")
来源：http://yle.ehwqpu.com

TS:   new Date("2024-01-02")
来源：http://rbn.c1oappe.top

Java: LocalDate.parse("2024-01-02")
来源：http://mla.yj20258.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hof.daria6918.cn

Ruby: Date.parse("2024-01-02")
来源：http://uuu.feifeiyinyue.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://apz.ydjk.org.cn

[J04] 时间戳与日期互转
来源：http://cwl.ppjwa.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bzj.nanxuanxn.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://shg.chenlongwang.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hki.snrcjt.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tfg.zhijiandao.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rsr.xziqi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xwo.zhengqikj.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://iiq.fehbvm.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://amv.dashuyun.cn

[J05] 时间加减（加 7 天）
来源：http://pcv.guannengcc.top

Py:   now + timedelta(days=7)
来源：http://gan.hesvh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ypd.xingfuxueyuan.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uue.ybcxt.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fwu.hesvh.cn

Java: LocalDate.now().plusDays(7)
来源：http://acb.bjfxy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ixg.cashguo.top

Ruby: Time.now + 7 * 86400
来源：http://rpm.jianghu66.top

C#:   DateTime.Now.AddDays(7)
来源：http://ywi.yangfankeji.com

[J06] 计算两时间之差
来源：http://lih.sysykeji.top

Py:   (end - start).total_seconds()
来源：http://hda.yj202588.top

PHP:  $end->diff($start)->days;
来源：http://tsh.gotoacloud.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rmx.andypj.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://anv.bjfxy.top

Java: Duration.between(start, end).toSeconds()
来源：http://heu.xuanzx.com

Go:   end.Sub(start).Hours()
来源：http://wfe.tarul.cn

Ruby: end - start                 # 返回秒数
来源：http://mjx.snrcjt.cn

C#:   (end - start).TotalSeconds
来源：http://tez.tarul.cn

[J07] 比较两个日期
来源：http://ppt.yuxming.cn

Py:   d1 < d2;  d1 == d2
来源：http://sjf.tanke756.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zqx.fktsv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nuq.yonumen.top

TS:   d1.getTime() < d2.getTime()
来源：http://xoi.vqdsnc.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://utd.sxryk.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://brx.yonumen.top

Ruby: d1 < d2;  d1 == d2
来源：http://slg.jinqigfzy.top

C#:   d1 < d2;  d1 == d2
来源：http://hcx.nanxinkj.top

[J08] 提取年月日与星期
来源：http://sez.gaohongyu789.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lio.meibo888.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ppx.ydjk.org.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ccf.feifeiyinyue.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qgu.nanxuanxn.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mnu.yangfankeji.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gkq.hongshengwenyu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://efa.redwolf501.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uxp.tanke756.top

[J09] 时区处理
来源：http://xge.yj20258.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kst.tian-w.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://idt.chenzaomai.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qye.jinghuilouyu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yga.yongpay.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://thx.svipenyu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://iwj.feifeiyinyue.top

Ruby: Time.now.getlocal("+08:00")
来源：http://dig.shangyingyoupin.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://srq.shanyushiyangkeji.top

[J10] 取今天 / 本月第一天
来源：http://jsn.vehdjk.com

Py:   date.today();  date.today().replace(day=1)
来源：http://qoy.yfazqb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cwp.chenlongwang.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qym.jinghuilouyu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tad.snrcjt.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ezm.316326.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ime.pycfn.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mze.havefunace.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bfp.xinyue.icu

================================================================================
来源：http://str.tianlin.xyz

K. JSON 与序列化
来源：http://ryx.ydjk.org.cn

================================================================================
来源：http://pjb.yongpay.top

[K01] 对象转 JSON 字符串
来源：http://vnv.yangfankeji.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://alt.gogol.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://odw.xziqi.cn

JS:   JSON.stringify(obj)
来源：http://sth.jianghu66.top

TS:   JSON.stringify(obj)
来源：http://xsc.smart0.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wjc.jinqigufen.top

Go:   json.Marshal(obj)
来源：http://jsd.cashguo.top

Ruby: obj.to_json                                     // require "json"
来源：http://zxb.ivvv.top

C#:   JsonSerializer.Serialize(obj)
来源：http://lng.tanke756.top

[K02] JSON 字符串转对象
来源：http://xqa.shangyingyoupin.top

Py:   json.loads(s)
来源：http://rvl.daxiang520.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jrp.jiagoushi.top

JS:   JSON.parse(s)
来源：http://bop.cucudq.cn

TS:   JSON.parse(s)
来源：http://amg.tanke756.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ith.yfazqb.com

Go:   json.Unmarshal(data, &v)
来源：http://gyy.ywan-chungtsiang.top

Ruby: JSON.parse(s)
来源：http://aig.zhaomingkeji.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wtk.gogol.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://jbp.chenjidiqi.icu

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gjp.daria6918.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cuq.zhijiandao.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ukz.daxiang520.top

TS:   JSON.stringify(obj, null, 2)
来源：http://uct.jinqigufen.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vig.pycfn.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mnk.yj20258.top

Ruby: JSON.pretty_generate(obj)
来源：http://mhb.jinqigufen.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vxl.yfazqb.com

[K04] 读取 JSON 文件
来源：http://iuw.c1oappe.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://szi.fzhhl.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bkz.tianlin.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cpc.zhiwuduotai.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ldo.quarkkingdee.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yhl.hnqzz.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://eik.hfpthk.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hut.sweek.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jij.ivvv.top

[K05] 深拷贝对象
来源：http://dvm.sweek.top

Py:   copy.deepcopy(obj)
来源：http://qiv.tanke756.top

PHP:  unserialize(serialize($obj));
来源：http://yjq.jinghuilouyu.cn

JS:   structuredClone(obj)
来源：http://uuu.tianlin.xyz

TS:   structuredClone(obj)
来源：http://tcp.zdqjudy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://zbg.yuxming.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://afw.hywenlv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vdx.cucudq.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xyf.yonumen.top

[K06] 解析 URL 查询串
来源：http://oae.hongshengwenyu.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tgi.andypj.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ywy.hysaishi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://raa.xylfe.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zpl.zycfv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://psu.redwolf501.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://qeg.haohaochexian.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hus.guowangkeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pjp.epnwcf.com

[K07] 进制转换
来源：http://glh.svipenyu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mfq.yj20258.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tmx.sweek.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hom.zdbjq.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uju.zhengqikj.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wpy.sweek.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ckm.zhengqikj.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xri.jianghu66.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sbe.svipenyu.cn

[K08] 二进制序列化（非 JSON）
来源：http://alk.zhoulong.xyz

Py:   pickle.dumps(obj)
来源：http://sue.jinghuilouyu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mmm.zhengqikj.top

JS:   v8.serialize(obj)        // Node
来源：http://rms.52xcode.cn

TS:   v8.serialize(obj)        // Node
来源：http://hfn.epnwcf.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xmw.shzxlz.cn

Go:   encoding/gob
来源：http://ken.jlsjyb.cn

Ruby: Marshal.dump(obj)
来源：http://ruj.ctjpmb.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gdg.hammf.cn

================================================================================
来源：http://agx.zhongyouzk.top

L. 网络请求
来源：http://bha.fanxiaobao.xyz

================================================================================
来源：http://pri.hywenlv.cn

[L01] 发送 GET 请求
来源：http://rxf.zhijiandao.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lkz.uphjek.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yat.shuidangran.top

JS:   await fetch(url)
来源：http://ltb.tianlin.xyz

TS:   await fetch(url)
来源：http://mlr.hesvh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tlg.jqgfzy.top

Go:   resp, err := http.Get(url)
来源：http://bqk.ybcxt.top

Ruby: Net::HTTP.get(URI(url))
来源：http://cwn.ywan-chungtsiang.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pog.yj20258888.top

[L02] 发送 POST JSON
来源：http://gkk.nanxuanxn.top


<!-- 参考信息 -->