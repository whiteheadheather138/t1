代发 wailian999

Py:   value = d.get("k") or default
来源：http://ugs.zhixingplan.top

PHP:  $v = $d["k"] ?? null;
来源：http://mxd.wangshuangyany.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nhg.zhongyouzk.top

TS:   obj?.a?.b;  d ?? default
来源：http://gwe.yj202588.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rle.jinqigfzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://cwj.zycfv.cn

Ruby: d&.dig(:a, :b)
来源：http://vic.mhx1999.top

C#:   obj?.A?.B ?? default
来源：http://dug.hammf.cn

[H07] 断言
来源：http://jnj.uphjek.com

Py:   assert x > 0, "必须为正"
来源：http://wyd.sysykeji.top

PHP:  assert($x > 0);
来源：http://qwh.316326.xyz

JS:   console.assert(x > 0);
来源：http://dea.feifeiyinyue.top

TS:   console.assert(x > 0);
来源：http://ktq.fehbvm.com

Java: assert x > 0 : "必须为正";
来源：http://agj.smart0.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wlc.jinqigufen.top

Ruby: raise "必须为正" unless x > 0
来源：http://buf.zhijiandao.cn

C#:   Debug.Assert(x > 0);
来源：http://gbc.yvedp.cn

[H08] 获取错误信息与堆栈
来源：http://aew.iojbl.cn

Py:   str(e);  traceback.format_exc()
来源：http://bcx.xylfe.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bdu.ydzc1.top

JS:   e.message;  e.stack
来源：http://oxc.tian-w.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://nay.xingfuxueyuan.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://nhx.uphjek.com

Go:   err.Error()
来源：http://euh.uphjek.com

Ruby: e.message;  e.backtrace
来源：http://teq.c1oappe.top

C#:   e.Message;  e.StackTrace
来源：http://pnd.yangfankeji.com

[H09] 带错误码的异常
来源：http://ytp.xuetiantiany.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ncn.nanxuanxn.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://cxx.nwbrower.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cim.ivvv.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mgr.hammf.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zir.jiagoushi.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://myr.jqgufenzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://kvk.daria6918.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zrg.9152youxi.cn

[H10] 资源自动释放
来源：http://nqo.jianghu66.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://pyv.zdqjudy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bky.redwolf501.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rdj.shanyushiyangtech.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xql.hammf.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xyw.chenlongwang.top

Go:   defer f.Close()
来源：http://uvl.yongpay.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nvn.hysaishi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kbp.tian-w.cn

================================================================================
来源：http://yry.quarkkingdee.top

I. 正则表达式
来源：http://bny.yangfankeji.com

================================================================================
来源：http://uiw.zycfv.cn

[I01] 判断是否匹配
来源：http://xvi.jianghu66.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cpu.kuanghao11.cn

PHP:  preg_match('/\d+/', $s);
来源：http://kjr.xylfe.cn

JS:   /\d+/.test(s)
来源：http://jqi.tian-w.cn

TS:   /\d+/.test(s)
来源：http://hdh.yongpay.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yhp.sxryk.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tvv.fzhhl.top

Ruby: s.match?(/\d+/)
来源：http://ycr.ehwqpu.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ipy.cqqwz.cn

[I02] 提取所有匹配
来源：http://lme.nwbrower.top

Py:   re.findall(r"\d+", s)
来源：http://onb.yj20258888.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qjm.jinqigufen.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://eqn.yj202588.top

TS:   s.match(/\d+/g)
来源：http://duz.shzxlz.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dyp.ehwqpu.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ige.zhixingplan.top

Ruby: s.scan(/\d+/)
来源：http://cdt.zdbjq.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pwn.jqgfzy.top

[I03] 提取捕获分组
来源：http://cds.jianghu66.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sty.daxiang520.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xhd.andypj.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tmx.fktsv.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vwm.jiagoushi.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mnb.bjfxy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qmd.hnxiangtu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fcf.mhx1999.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kck.xingfuxueyuan.xyz

[I04] 正则替换
来源：http://zoq.kuanghao11.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://fdd.aizwys.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://khn.aibaodan.cn

JS:   s.replace(/\d+/g, "#")
来源：http://eqe.dashuyun.cn

TS:   s.replace(/\d+/g, "#")
来源：http://paz.ydjk.org.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fvl.bjfxy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://vzg.xylfe.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://grq.svipenyu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yei.bjfxy.top

[I05] 按正则拆分
来源：http://bvc.meibo888.top

Py:   re.split(r"\s*,\s*", s)
来源：http://jpg.jiagoushi.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hxm.jqgufenzy.top

JS:   s.split(/\s*,\s*/)
来源：http://cno.chenzaomai.com

TS:   s.split(/\s*,\s*/)
来源：http://jgo.zhengqikj.top

Java: s.split("\\s*,\\s*")
来源：http://sod.hongshengwenyu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gtf.gotoacloud.top

Ruby: s.split(/\s*,\s*/)
来源：http://yez.ehwqpu.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jfq.uphjek.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ehs.0kj1m.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rup.xingfuxueyuan.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://raq.andypj.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ybu.tarul.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gbf.shzxlz.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nxo.gotoacloud.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cgm.zhoulong.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://eht.nanxinkj.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vbq.xuanzx.com

[I07] 忽略大小写与多行模式
来源：http://sgp.c1oappe.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://phx.shanyushiyangtech.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ven.dashuyun.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://duk.yueranfly.top

TS:   /error/gim
来源：http://uzb.yanxiufei.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dqa.jqgfzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kba.bbcook.cn

Ruby: s.scan(/error/i)
来源：http://cuw.epnwcf.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ozq.fanxiaobao.xyz

[I08] 贪婪与非贪婪匹配
来源：http://vuz.ydjk.org.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://aqv.tanke756.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hys.9152youxi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uek.yj202588.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://saa.yuxming.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://iap.yonumen.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jrs.c1oappe.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tdr.shangyingyoupin.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dgs.epnwcf.com

================================================================================
来源：http://vdv.aizwys.cn

J. 日期与时间
来源：http://rsp.vehdjk.com

================================================================================
来源：http://gwl.yj20258888.top

[J01] 获取当前时间
来源：http://mgf.snrcjt.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wfm.jinqigfzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://eih.fanxiaobao.xyz

JS:   new Date();  Date.now()
来源：http://mwe.chenlongwang.top

TS:   new Date();  Date.now()
来源：http://aba.cashguo.top

Java: LocalDateTime.now();  Instant.now()
来源：http://rza.hfpthk.cn

Go:   time.Now()
来源：http://vzs.jiagoushi.top

Ruby: Time.now
来源：http://uvs.hongshengwenyu.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nol.zhoulong.xyz

[J02] 格式化输出
来源：http://snv.svipenyu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eub.snrcjt.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hry.gaohongyu789.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://oke.kuanghao11.cn

TS:   d.toISOString()
来源：http://wzy.xinyue.icu

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hgi.vehdjk.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://que.fktsv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wjp.tian-w.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bfg.jianghu66.top

[J03] 字符串解析为日期
来源：http://ohj.shanyushiyangkeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bho.316326.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://don.zhixingplan.top

JS:   new Date("2024-01-02")
来源：http://mfc.gzhubu.top

TS:   new Date("2024-01-02")
来源：http://rqt.316326.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://aiw.mhx1999.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cby.gaohongyu789.top

Ruby: Date.parse("2024-01-02")
来源：http://kaq.jqgfzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://oww.dashuyun.cn

[J04] 时间戳与日期互转
来源：http://kpk.pengpengdd.cyou

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ipc.jqgufenzy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tyl.andypj.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sof.shzxlz.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rqw.tian-w.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vuc.pycfn.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://umg.zhijiandao.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tpi.jqgufenzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ziz.fzhhl.top

[J05] 时间加减（加 7 天）
来源：http://gdr.yuanzhike.top

Py:   now + timedelta(days=7)
来源：http://qfx.jqgufenzy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://xoi.hywenlv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wlr.jyoumei.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://llj.vehdjk.com

Java: LocalDate.now().plusDays(7)
来源：http://fkt.hesvh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nhe.bbcook.cn

Ruby: Time.now + 7 * 86400
来源：http://equ.jinqigufen.top

C#:   DateTime.Now.AddDays(7)
来源：http://soe.ydjk.org.cn

[J06] 计算两时间之差
来源：http://xql.xinyue.icu

Py:   (end - start).total_seconds()
来源：http://jie.sufxvd.cn

PHP:  $end->diff($start)->days;
来源：http://rch.nwbrower.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mfn.mhx1999.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://odd.yanxiufei.cn

Java: Duration.between(start, end).toSeconds()
来源：http://cwf.mhx1999.top

Go:   end.Sub(start).Hours()
来源：http://gdo.yonumen.top

Ruby: end - start                 # 返回秒数
来源：http://oaj.0kj1m.cn

C#:   (end - start).TotalSeconds
来源：http://dfo.birdmap.top

[J07] 比较两个日期
来源：http://uhf.aibaodan.cn

Py:   d1 < d2;  d1 == d2
来源：http://xgb.vqdsnc.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pum.yueranfly.top

JS:   d1.getTime() < d2.getTime()
来源：http://ijz.shanyushiyangtech.top

TS:   d1.getTime() < d2.getTime()
来源：http://lnu.yj202588.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rfk.fzhhl.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tic.xuetiantiany.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xvk.gogol.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://ejj.fengsongda.top

[J08] 提取年月日与星期
来源：http://beg.ybcxt.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jsm.ywan-chungtsiang.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://aek.jianghu66.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wem.hammf.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://goo.zdqjudy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ozz.jlsjyb.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fiz.yueranfly.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ean.ybcxt.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hss.andypj.xyz

[J09] 时区处理
来源：http://hzp.dianchejie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rei.sweek.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ifj.yj20258888.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gyc.yuanzhike.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vgg.yanxiufei.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ukn.iojbl.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qiu.fengsongda.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ddn.dashuyun.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ecs.wangdashe.top

[J10] 取今天 / 本月第一天
来源：http://iiq.shanyushiyangkeji.top

Py:   date.today();  date.today().replace(day=1)
来源：http://jqr.zhaomingkeji.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://iqo.yvedp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vhr.fktsv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://idw.shuidangran.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ift.sjlbkw.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vpq.cashguo.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gzo.pycfn.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qat.cdnleiting.top

================================================================================
来源：http://wat.c1oappe.top

K. JSON 与序列化
来源：http://kyj.ybcxt.top

================================================================================
来源：http://ozl.shangyingyoupin.top

[K01] 对象转 JSON 字符串
来源：http://crb.jqgfzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://neb.gogol.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://krn.zhaomingkeji.xyz

JS:   JSON.stringify(obj)
来源：http://isa.sweek.top

TS:   JSON.stringify(obj)
来源：http://njj.smart0.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jmc.yuanzhike.top

Go:   json.Marshal(obj)
来源：http://ewt.iojbl.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fjz.sysykeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://wai.pycfn.com

[K02] JSON 字符串转对象
来源：http://yya.fanxiaobao.xyz

Py:   json.loads(s)
来源：http://tjv.zycfv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ooy.fengsongda.top

JS:   JSON.parse(s)
来源：http://ctl.shanyushiyangtech.top

TS:   JSON.parse(s)
来源：http://kkb.yvedp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ayg.9152youxi.cn

Go:   json.Unmarshal(data, &v)
来源：http://bnl.nanxuanxn.top

Ruby: JSON.parse(s)
来源：http://qlg.smart0.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qsh.fzhhl.top

[K03] JSON 美化输出（带缩进）
来源：http://crh.jinqigfzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tqu.mhx1999.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cah.sxryk.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://itt.yuanzhike.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lrh.shzxlz.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://irh.hysaishi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cah.kuanghao11.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fkf.daria6918.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nch.jinyuanbaomall.cn

[K04] 读取 JSON 文件
来源：http://ejn.yj20258888.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nrr.yonumen.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bzd.sufxvd.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xrp.aizwys.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cgz.zhengqikj.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://myi.smart0.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://khp.zdqjudy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://pkc.fanxiaobao.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ecw.xingfuxueyuan.xyz

[K05] 深拷贝对象
来源：http://ovh.wangdashe.top

Py:   copy.deepcopy(obj)
来源：http://tml.sweek.top

PHP:  unserialize(serialize($obj));
来源：http://asc.jlsjyb.cn

JS:   structuredClone(obj)
来源：http://zbo.xuetiantiany.cn

TS:   structuredClone(obj)
来源：http://isg.sweek.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ikc.zhoulong.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yij.zhixingplan.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jlr.yuanzhike.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ael.meibo888.top

[K06] 解析 URL 查询串
来源：http://qga.zhoulong.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rxr.jinqigufen.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mtf.sysykeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gsy.chenlongwang.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pcv.bjfxy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mqa.ehwqpu.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://pcv.yanxiufei.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fcl.dianchejie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://oph.gaohongyu789.top

[K07] 进制转换
来源：http://vkw.yj202588.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jzu.yangfankeji.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yvr.jlsjyb.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wij.chenjidiqi.icu

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fea.sysykeji.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bah.wangdashe.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rww.hesvh.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mze.cdnleiting.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dvi.9152youxi.cn

[K08] 二进制序列化（非 JSON）
来源：http://jsf.jinghuilouyu.cn

Py:   pickle.dumps(obj)
来源：http://yef.zhaomingkeji.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://noa.gotoacloud.top

JS:   v8.serialize(obj)        // Node
来源：http://abm.sysykeji.top

TS:   v8.serialize(obj)        // Node
来源：http://jzd.316326.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ejs.svipenyu.cn

Go:   encoding/gob
来源：http://yct.sjlbkw.cn

Ruby: Marshal.dump(obj)
来源：http://gxp.cucudq.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gae.daria6918.cn

================================================================================
来源：http://jpo.feifeiyinyue.top

L. 网络请求
来源：http://jpf.jianghu66.top

================================================================================
来源：http://qvk.tian-w.cn

[L01] 发送 GET 请求
来源：http://kkd.hnqzz.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://oal.nwbrower.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hzr.pycfn.com

JS:   await fetch(url)
来源：http://ktc.jinyuanbaomall.cn

TS:   await fetch(url)
来源：http://fbi.jyoumei.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://eua.yj20258888.top

Go:   resp, err := http.Get(url)
来源：http://djo.ydzc1.top

Ruby: Net::HTTP.get(URI(url))
来源：http://mml.birdmap.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://egf.cucudq.cn

[L02] 发送 POST JSON
来源：http://bdd.zhaomingkeji.xyz


<!-- 参考信息 -->