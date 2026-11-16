代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ono.tianlin.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://ins.jinghuilouyu.cn

Ruby: d&.dig(:a, :b)
来源：http://aic.andypj.xyz

C#:   obj?.A?.B ?? default
来源：http://pnp.feifeiyinyue.top

[H07] 断言
来源：http://bmb.vehdjk.com

Py:   assert x > 0, "必须为正"
来源：http://ffr.zhijiandao.cn

PHP:  assert($x > 0);
来源：http://hvo.quarkkingdee.top

JS:   console.assert(x > 0);
来源：http://nab.gaohongyu789.top

TS:   console.assert(x > 0);
来源：http://rlc.jinyuanbaomall.cn

Java: assert x > 0 : "必须为正";
来源：http://yoc.shuidangran.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yan.yvedp.cn

Ruby: raise "必须为正" unless x > 0
来源：http://kyt.xingfuxueyuan.xyz

C#:   Debug.Assert(x > 0);
来源：http://ppm.zycfv.cn

[H08] 获取错误信息与堆栈
来源：http://udn.dashuyun.cn

Py:   str(e);  traceback.format_exc()
来源：http://jyj.zhaomingkeji.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pjp.yuxming.cn

JS:   e.message;  e.stack
来源：http://ksh.jqgfzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://fch.jinghuilouyu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bwk.vqdsnc.cn

Go:   err.Error()
来源：http://rmz.xylfe.cn

Ruby: e.message;  e.backtrace
来源：http://jiu.jlsjyb.cn

C#:   e.Message;  e.StackTrace
来源：http://xxd.gzhubu.top

[H09] 带错误码的异常
来源：http://ndv.ybcxt.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://msv.svipenyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://eib.yj202588.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ucs.yongpay.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://njd.yonumen.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://knv.nanxinkj.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://glv.sysykeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://vdy.hysaishi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://tdi.jinghuilouyu.cn

[H10] 资源自动释放
来源：http://xsf.meibo888.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://xbb.smart0.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rjc.zhaomingkeji.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://api.zdqjudy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://meq.zhijiandao.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ixp.nwbrower.top

Go:   defer f.Close()
来源：http://fzl.yanxiufei.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sti.nwbrower.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dlf.tian-w.cn

================================================================================
来源：http://eqa.kuanghao11.cn

I. 正则表达式
来源：http://auq.0kj1m.cn

================================================================================
来源：http://tmp.bjfxy.top

[I01] 判断是否匹配
来源：http://ffe.xinyue.icu

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mki.cdnleiting.top

PHP:  preg_match('/\d+/', $s);
来源：http://uhk.yfazqb.com

JS:   /\d+/.test(s)
来源：http://vrd.nanxinkj.top

TS:   /\d+/.test(s)
来源：http://lvo.yanxiufei.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qau.shzxlz.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wgs.smart0.xyz

Ruby: s.match?(/\d+/)
来源：http://vxy.jlsjyb.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rzm.pycfn.com

[I02] 提取所有匹配
来源：http://crc.zhengqikj.top

Py:   re.findall(r"\d+", s)
来源：http://lcu.hywenlv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://inz.nwbrower.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://biq.316326.xyz

TS:   s.match(/\d+/g)
来源：http://yxk.nanxinkj.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dun.xuanzx.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://aiv.hysaishi.cn

Ruby: s.scan(/\d+/)
来源：http://kpc.xuanzx.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://egv.aizwys.cn

[I03] 提取捕获分组
来源：http://bmq.shangyingyoupin.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://szv.zhixingplan.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://evi.tianlin.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jbf.0kj1m.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qor.shangyingyoupin.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kze.yongpay.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nal.xylfe.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://crp.yueranfly.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zpl.iojbl.cn

[I04] 正则替换
来源：http://agf.yj202588.top

Py:   re.sub(r"\d+", "#", s)
来源：http://nas.yj202588.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wwz.chenjidiqi.icu

JS:   s.replace(/\d+/g, "#")
来源：http://kzp.tianlin.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://anb.xziqi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rvm.epnwcf.com

Go:   re.ReplaceAllString(s, "#")
来源：http://bnk.vehdjk.com

Ruby: s.gsub(/\d+/, "#")
来源：http://csc.cqqwz.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://trp.gogol.net.cn

[I05] 按正则拆分
来源：http://bkt.chenjidiqi.icu

Py:   re.split(r"\s*,\s*", s)
来源：http://nhy.yfazqb.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://adr.shanyushiyangtech.top

JS:   s.split(/\s*,\s*/)
来源：http://hsc.xinyue.icu

TS:   s.split(/\s*,\s*/)
来源：http://qcr.cqqwz.cn

Java: s.split("\\s*,\\s*")
来源：http://kkm.meibo888.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kxy.jiagoushi.top

Ruby: s.split(/\s*,\s*/)
来源：http://nfd.ybcxt.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pem.birdmap.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kua.fktsv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cal.fanxiaobao.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gev.ybcxt.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qzl.hcnkem.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ojn.hongshengwenyu.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://oon.feifeiyinyue.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dnv.jyoumei.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dtu.zhaomingkeji.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pla.meibo888.top

[I07] 忽略大小写与多行模式
来源：http://gxh.yanxiufei.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xlz.0kj1m.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wpx.yfazqb.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qaf.jinyuanbaomall.cn

TS:   /error/gim
来源：http://gtq.sxryk.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ggw.dashuyun.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sew.hammf.cn

Ruby: s.scan(/error/i)
来源：http://wqw.xinyue.icu

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nwc.yonumen.top

[I08] 贪婪与非贪婪匹配
来源：http://ugs.feifeiyinyue.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dpc.hysaishi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wsz.jyoumei.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jvo.ivvv.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://njg.xinyue.icu

Java: Pattern.compile("<b>.*?</b>")
来源：http://ogc.sufxvd.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zbe.yj202588.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bts.fehbvm.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dda.yangfankeji.com

================================================================================
来源：http://xiz.zhijiandao.cn

J. 日期与时间
来源：http://rid.52xcode.cn

================================================================================
来源：http://rvg.ybcxt.top

[J01] 获取当前时间
来源：http://fzg.yuanzhike.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://nzt.0kj1m.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fup.chenzaomai.com

JS:   new Date();  Date.now()
来源：http://ano.yvedp.cn

TS:   new Date();  Date.now()
来源：http://yaj.sweek.top

Java: LocalDateTime.now();  Instant.now()
来源：http://yoh.shzxlz.cn

Go:   time.Now()
来源：http://oca.xingfuxueyuan.xyz

Ruby: Time.now
来源：http://bhn.chenjidiqi.icu

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xha.tanke756.top

[J02] 格式化输出
来源：http://dnj.zhongyouzk.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sqn.zhoulong.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rob.shangyingyoupin.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://txr.dianchejie.cn

TS:   d.toISOString()
来源：http://bpr.zhoulong.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yjz.pycfn.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bkm.ivvv.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uaa.hnxiangtu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xjn.sysykeji.top

[J03] 字符串解析为日期
来源：http://flp.cashguo.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vdj.gaohongyu789.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rvc.hongshengwenyu.top

JS:   new Date("2024-01-02")
来源：http://kht.316326.xyz

TS:   new Date("2024-01-02")
来源：http://exf.wangdashe.top

Java: LocalDate.parse("2024-01-02")
来源：http://eqm.52xcode.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bhi.vqdsnc.cn

Ruby: Date.parse("2024-01-02")
来源：http://atb.sxryk.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qmi.zhongyouzk.top

[J04] 时间戳与日期互转
来源：http://zzf.yfazqb.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mix.yvedp.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xnp.zhongyouzk.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fox.dashuyun.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fxi.sjlbkw.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zrx.zdbjq.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ikr.guannengcc.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xit.shanyushiyangkeji.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jun.zhiwuduotai.top

[J05] 时间加减（加 7 天）
来源：http://tpi.52xcode.cn

Py:   now + timedelta(days=7)
来源：http://gmy.sjlbkw.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://usl.gogol.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hfh.yj202588.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cii.jiagoushi.top

Java: LocalDate.now().plusDays(7)
来源：http://pva.smart0.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hcg.birdmap.top

Ruby: Time.now + 7 * 86400
来源：http://yrx.zhijiandao.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vba.ivvv.top

[J06] 计算两时间之差
来源：http://brl.tarul.cn

Py:   (end - start).total_seconds()
来源：http://vzl.hywenlv.cn

PHP:  $end->diff($start)->days;
来源：http://iqt.daxiang520.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yir.zhixingplan.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://knp.uphjek.com

Java: Duration.between(start, end).toSeconds()
来源：http://vqg.gzhubu.top

Go:   end.Sub(start).Hours()
来源：http://qso.zdbjq.cn

Ruby: end - start                 # 返回秒数
来源：http://kxo.meibo888.top

C#:   (end - start).TotalSeconds
来源：http://giu.chenlongwang.top

[J07] 比较两个日期
来源：http://pch.wangdashe.top

Py:   d1 < d2;  d1 == d2
来源：http://pbg.zhaomingkeji.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uni.shuidangran.top

JS:   d1.getTime() < d2.getTime()
来源：http://egr.epnwcf.com

TS:   d1.getTime() < d2.getTime()
来源：http://jiw.feifeiyinyue.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ucq.xuanzx.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://toe.yfazqb.com

Ruby: d1 < d2;  d1 == d2
来源：http://nkz.bbcook.cn

C#:   d1 < d2;  d1 == d2
来源：http://esw.shzxlz.cn

[J08] 提取年月日与星期
来源：http://ajp.ybcxt.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zle.c1oappe.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://try.zdbjq.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wvp.jlsjyb.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://brl.vqdsnc.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ynr.shuidangran.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vkn.jinqigufen.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ioa.cdnleiting.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lcc.jiagoushi.top

[J09] 时区处理
来源：http://dps.aibaodan.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tge.yj20258.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kwo.xuanzx.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lrv.cucudq.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hej.chenlongwang.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cbt.yueranfly.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nmn.andypj.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://pjn.yangfankeji.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mbb.jinqigufen.top

[J10] 取今天 / 本月第一天
来源：http://zmx.snrcjt.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://olq.aizwys.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mcm.hfpthk.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kzw.dianchejie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hud.hfpthk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sjo.zhongyouzk.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xrr.xuetiantiany.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://but.guowangkeji.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://faq.fzhhl.top

================================================================================
来源：http://oku.fktsv.cn

K. JSON 与序列化
来源：http://nik.ehwqpu.com

================================================================================
来源：http://vvi.zhoulong.xyz

[K01] 对象转 JSON 字符串
来源：http://mue.xuetiantiany.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://djn.zhengqikj.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qio.snrcjt.cn

JS:   JSON.stringify(obj)
来源：http://zin.hysaishi.cn

TS:   JSON.stringify(obj)
来源：http://iyy.pengpengdd.cyou

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jgn.zdbjq.cn

Go:   json.Marshal(obj)
来源：http://bwd.jinqigfzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://uom.zhengqikj.top

C#:   JsonSerializer.Serialize(obj)
来源：http://bni.epnwcf.com

[K02] JSON 字符串转对象
来源：http://qxj.hysaishi.cn

Py:   json.loads(s)
来源：http://fdz.yj20258888.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kws.hnxiangtu.top

JS:   JSON.parse(s)
来源：http://frs.nwbrower.top

TS:   JSON.parse(s)
来源：http://nms.cqqwz.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vew.jinqigufen.top

Go:   json.Unmarshal(data, &v)
来源：http://ysc.cucudq.cn

Ruby: JSON.parse(s)
来源：http://wvc.zhiwuduotai.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ewj.pengpengdd.cyou

[K03] JSON 美化输出（带缩进）
来源：http://eez.ybcxt.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ege.daxiang520.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vrn.zhijiandao.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yag.yfazqb.com

TS:   JSON.stringify(obj, null, 2)
来源：http://czp.hesvh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cdo.yonumen.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tut.zhiwuduotai.top

Ruby: JSON.pretty_generate(obj)
来源：http://bcc.9152youxi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://crj.xuetiantiany.cn

[K04] 读取 JSON 文件
来源：http://ogb.zhoulong.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jmc.shuidangran.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jwt.meibo888.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xjp.fengsongda.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jrh.aibaodan.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zrj.wangdashe.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://myr.fanxiaobao.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://ybx.ydzc1.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wiv.smart0.xyz

[K05] 深拷贝对象
来源：http://tdr.hfpthk.cn

Py:   copy.deepcopy(obj)
来源：http://kej.cucudq.cn

PHP:  unserialize(serialize($obj));
来源：http://pey.chenjidiqi.icu

JS:   structuredClone(obj)
来源：http://qjj.wangshuangyany.cn

TS:   structuredClone(obj)
来源：http://ugy.hnqzz.top

Java: // 手写拷贝构造，或序列化往返
来源：http://boy.pycfn.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nto.hcnkem.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wys.hfpthk.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kqd.aibaodan.cn

[K06] 解析 URL 查询串
来源：http://bxl.ydjk.org.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mlz.wangdashe.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gaf.yj20258.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bos.tarul.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tje.sxryk.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://etm.yueranfly.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ave.nanxuanxn.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cum.jinqigfzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ran.xylfe.cn

[K07] 进制转换
来源：http://pgm.hysaishi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hcv.cucudq.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ryz.0kj1m.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kxf.nwbrower.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tcw.shanyushiyangkeji.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dsb.ybcxt.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ids.tanke756.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kjs.zdqjudy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wii.zhiwuduotai.top

[K08] 二进制序列化（非 JSON）
来源：http://zvf.jiagoushi.top

Py:   pickle.dumps(obj)
来源：http://ctt.feifeiyinyue.top

PHP:  serialize($obj);  unserialize($s);
来源：http://imo.yangfankeji.com

JS:   v8.serialize(obj)        // Node
来源：http://anu.fktsv.cn

TS:   v8.serialize(obj)        // Node
来源：http://rjr.cqqwz.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://iqu.gogol.net.cn

Go:   encoding/gob
来源：http://eii.tarul.cn

Ruby: Marshal.dump(obj)
来源：http://nke.guannengcc.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rlj.yanxiufei.cn

================================================================================
来源：http://kyz.yvedp.cn

L. 网络请求
来源：http://qil.yanxiufei.cn

================================================================================
来源：http://cnf.yfazqb.com

[L01] 发送 GET 请求
来源：http://syg.cdnleiting.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mms.ppjwa.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uft.zhijiandao.cn

JS:   await fetch(url)
来源：http://fgg.nanxuanxn.top

TS:   await fetch(url)
来源：http://dog.fengsongda.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oep.wangshuangyany.cn

Go:   resp, err := http.Get(url)
来源：http://iph.ydjk.org.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://nfo.sweek.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cgq.kuanghao11.cn

[L02] 发送 POST JSON
来源：http://tqm.jqgfzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://fxn.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lot.sysykeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rmy.cqqwz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gni.nwbrower.top


<!-- 参考信息 -->