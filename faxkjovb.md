代发 wailian999

Py:   value = d.get("k") or default
来源：http://hlm.pengpengdd.cyou

PHP:  $v = $d["k"] ?? null;
来源：http://uol.yuanzhike.top

JS:   obj?.a?.b;  d ?? default
来源：http://rsc.nanxinkj.top

TS:   obj?.a?.b;  d ?? default
来源：http://zvo.zhengqikj.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jcc.gotoacloud.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ocf.ywan-chungtsiang.top

Ruby: d&.dig(:a, :b)
来源：http://bjl.yuxming.cn

C#:   obj?.A?.B ?? default
来源：http://mzb.yueranfly.top

[H07] 断言
来源：http://hgr.kuanghao11.cn

Py:   assert x > 0, "必须为正"
来源：http://qmn.jinyuanbaomall.cn

PHP:  assert($x > 0);
来源：http://kot.vqdsnc.cn

JS:   console.assert(x > 0);
来源：http://cbk.yangfankeji.com

TS:   console.assert(x > 0);
来源：http://oof.gotoacloud.top

Java: assert x > 0 : "必须为正";
来源：http://axz.aibaodan.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://iac.c1oappe.top

Ruby: raise "必须为正" unless x > 0
来源：http://jsj.yuxming.cn

C#:   Debug.Assert(x > 0);
来源：http://ahi.yj202588.top

[H08] 获取错误信息与堆栈
来源：http://zui.tianlin.xyz

Py:   str(e);  traceback.format_exc()
来源：http://ujy.jinqigfzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fpc.tian-w.cn

JS:   e.message;  e.stack
来源：http://mag.cashguo.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://qmy.zhixingplan.top

Java: e.getMessage();  e.printStackTrace()
来源：http://mkl.vehdjk.com

Go:   err.Error()
来源：http://oyo.havefunace.top

Ruby: e.message;  e.backtrace
来源：http://psi.tanke756.top

C#:   e.Message;  e.StackTrace
来源：http://spn.fehbvm.com

[H09] 带错误码的异常
来源：http://ecv.jiagoushi.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fxo.fanxiaobao.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://nbc.bjfxy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jkp.yuxming.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ihg.hnxiangtu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tvm.smart0.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rnv.sxryk.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ubw.uphjek.com

C#:   // 自定义异常类中加 Code 属性
来源：http://prb.fktsv.cn

[H10] 资源自动释放
来源：http://yqi.daria6918.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://isi.guannengcc.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gxl.sxryk.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dxz.dashuyun.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fsy.ybcxt.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xqp.yj20258.top

Go:   defer f.Close()
来源：http://mvh.xinyue.icu

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fqi.ybcxt.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://msh.ydjk.org.cn

================================================================================
来源：http://zxs.cashguo.top

I. 正则表达式
来源：http://oef.yvedp.cn

================================================================================
来源：http://cpi.redwolf501.top

[I01] 判断是否匹配
来源：http://prn.yueranfly.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://avq.yangfankeji.com

PHP:  preg_match('/\d+/', $s);
来源：http://set.zhengqikj.top

JS:   /\d+/.test(s)
来源：http://sjg.quarkkingdee.top

TS:   /\d+/.test(s)
来源：http://lwn.jinqigfzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tvx.jyoumei.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mgf.daria6918.cn

Ruby: s.match?(/\d+/)
来源：http://jnj.hcnkem.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bvy.ydzc1.top

[I02] 提取所有匹配
来源：http://pnk.snrcjt.cn

Py:   re.findall(r"\d+", s)
来源：http://res.0kj1m.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rvy.yj20258.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://beq.gzhubu.top

TS:   s.match(/\d+/g)
来源：http://pxf.zhixingplan.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://geg.ehwqpu.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wkp.tanke756.top

Ruby: s.scan(/\d+/)
来源：http://xbz.ppjwa.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qkx.cdnleiting.top

[I03] 提取捕获分组
来源：http://fan.jyoumei.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kyi.hywenlv.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lla.nanxuanxn.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ixv.gaohongyu789.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sft.316326.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rgt.shangyingyoupin.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qxq.gotoacloud.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nau.ydjk.org.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xnz.yj202588.top

[I04] 正则替换
来源：http://klc.cucudq.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://dli.gzhubu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ita.cdnleiting.top

JS:   s.replace(/\d+/g, "#")
来源：http://vox.tanke756.top

TS:   s.replace(/\d+/g, "#")
来源：http://qpg.redwolf501.top

Java: s.replaceAll("\\d+", "#")
来源：http://cyi.gaohongyu789.top

Go:   re.ReplaceAllString(s, "#")
来源：http://amw.hcnkem.com

Ruby: s.gsub(/\d+/, "#")
来源：http://kbo.xuetiantiany.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hbl.zdbjq.cn

[I05] 按正则拆分
来源：http://uco.fehbvm.com

Py:   re.split(r"\s*,\s*", s)
来源：http://vcf.dashuyun.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gyf.zhongyouzk.top

JS:   s.split(/\s*,\s*/)
来源：http://bmi.yonumen.top

TS:   s.split(/\s*,\s*/)
来源：http://afv.zhixingplan.top

Java: s.split("\\s*,\\s*")
来源：http://gub.jiagoushi.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dfb.shuidangran.top

Ruby: s.split(/\s*,\s*/)
来源：http://emd.zhijiandao.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tzw.cqqwz.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cuc.yuanzhike.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kqe.cucudq.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cct.xuetiantiany.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ylh.jinghuilouyu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yqh.vqdsnc.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://got.hfpthk.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://oar.shuidangran.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://izc.jinqigufen.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xyk.tarul.cn

[I07] 忽略大小写与多行模式
来源：http://gba.andypj.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://atd.52xcode.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rav.xuanzx.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xuf.yuanzhike.top

TS:   /error/gim
来源：http://xvz.vqdsnc.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uwa.cheryme.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lfn.mhx1999.top

Ruby: s.scan(/error/i)
来源：http://ijh.zhongyouzk.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ljw.zdbjq.cn

[I08] 贪婪与非贪婪匹配
来源：http://fsf.birdmap.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ciq.ctjpmb.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wmq.hysaishi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mee.gotoacloud.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ufd.andypj.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://yed.sjlbkw.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zmd.wangdashe.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bie.yongpay.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kxn.guannengcc.top

================================================================================
来源：http://ydt.yongpay.top

J. 日期与时间
来源：http://riq.fehbvm.com

================================================================================
来源：http://jbh.cheryme.top

[J01] 获取当前时间
来源：http://pah.uphjek.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://icg.52xcode.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://njo.zdbjq.cn

JS:   new Date();  Date.now()
来源：http://kef.hysaishi.cn

TS:   new Date();  Date.now()
来源：http://dxn.zdbjq.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bue.feifeiyinyue.top

Go:   time.Now()
来源：http://hdh.fengsongda.top

Ruby: Time.now
来源：http://era.daxiang520.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://amk.wangshuangyany.cn

[J02] 格式化输出
来源：http://rwb.zdbjq.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uod.ywan-chungtsiang.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kjg.birdmap.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ipu.xuetiantiany.cn

TS:   d.toISOString()
来源：http://quk.yuanzhike.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kze.tianlin.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rvs.shzxlz.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yij.hcnkem.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xrc.tarul.cn

[J03] 字符串解析为日期
来源：http://xgh.jinqigufen.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sak.yj202588.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xsf.iojbl.cn

JS:   new Date("2024-01-02")
来源：http://ilw.fktsv.cn

TS:   new Date("2024-01-02")
来源：http://jrh.9152youxi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vqb.yj202588.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://obx.feifeiyinyue.top

Ruby: Date.parse("2024-01-02")
来源：http://grb.yongpay.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ssd.yvedp.cn

[J04] 时间戳与日期互转
来源：http://rqz.zhixingplan.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://udw.chenzaomai.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zdd.tian-w.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jwa.yvedp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lnz.yuanzhike.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bmd.xuanzx.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xwf.daria6918.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wdv.hesvh.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://eae.bjfxy.top

[J05] 时间加减（加 7 天）
来源：http://dwc.aizwys.cn

Py:   now + timedelta(days=7)
来源：http://hau.cucudq.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wmn.andypj.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dji.dashuyun.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cby.jyoumei.cn

Java: LocalDate.now().plusDays(7)
来源：http://xmv.yongpay.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ech.zhoulong.xyz

Ruby: Time.now + 7 * 86400
来源：http://rua.fengsongda.top

C#:   DateTime.Now.AddDays(7)
来源：http://ibe.birdmap.top

[J06] 计算两时间之差
来源：http://olq.yfazqb.com

Py:   (end - start).total_seconds()
来源：http://xyz.jinghuilouyu.cn

PHP:  $end->diff($start)->days;
来源：http://anm.vehdjk.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hgt.shanyushiyangtech.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mhx.shzxlz.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pqk.fengsongda.top

Go:   end.Sub(start).Hours()
来源：http://mjr.fzhhl.top

Ruby: end - start                 # 返回秒数
来源：http://kgx.zhengqikj.top

C#:   (end - start).TotalSeconds
来源：http://kql.316326.xyz

[J07] 比较两个日期
来源：http://clu.daria6918.cn

Py:   d1 < d2;  d1 == d2
来源：http://ibu.birdmap.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://oqm.316326.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://hji.wangshuangyany.cn

TS:   d1.getTime() < d2.getTime()
来源：http://nob.yueranfly.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wak.aizwys.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cnt.sjlbkw.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lcl.xziqi.cn

C#:   d1 < d2;  d1 == d2
来源：http://veu.guannengcc.top

[J08] 提取年月日与星期
来源：http://koq.jlsjyb.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hdm.cashguo.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cjv.zhiwuduotai.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dla.gzhubu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rvd.shzxlz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rhi.xuetiantiany.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lio.redwolf501.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wrc.yuanzhike.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nho.sxryk.cn

[J09] 时区处理
来源：http://wss.aizwys.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lkf.shzxlz.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tny.shanyushiyangtech.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kzu.hywenlv.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jch.52xcode.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dbr.iojbl.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qsq.aibaodan.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ito.jinghuilouyu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vct.nwbrower.top

[J10] 取今天 / 本月第一天
来源：http://dxr.guowangkeji.top

Py:   date.today();  date.today().replace(day=1)
来源：http://hzs.jinyuanbaomall.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gni.hongshengwenyu.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ags.shzxlz.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://znh.havefunace.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ibz.hongshengwenyu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dha.birdmap.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ucr.hnqzz.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nhu.tarul.cn

================================================================================
来源：http://lvp.cashguo.top

K. JSON 与序列化
来源：http://jnf.xylfe.cn

================================================================================
来源：http://pom.shzxlz.cn

[K01] 对象转 JSON 字符串
来源：http://hdq.cheryme.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://srg.ydjk.org.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rhl.fktsv.cn

JS:   JSON.stringify(obj)
来源：http://biy.sxryk.cn

TS:   JSON.stringify(obj)
来源：http://boo.ydjk.org.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ily.ybcxt.top

Go:   json.Marshal(obj)
来源：http://efc.xuanzx.com

Ruby: obj.to_json                                     // require "json"
来源：http://veo.daria6918.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qez.gaohongyu789.top

[K02] JSON 字符串转对象
来源：http://aoa.cashguo.top

Py:   json.loads(s)
来源：http://vsb.vqdsnc.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xgq.xuanzx.com

JS:   JSON.parse(s)
来源：http://fbr.jqgfzy.top

TS:   JSON.parse(s)
来源：http://bbh.haohaochexian.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jjd.fanxiaobao.xyz

Go:   json.Unmarshal(data, &v)
来源：http://zgk.xuetiantiany.cn

Ruby: JSON.parse(s)
来源：http://uho.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ijy.yfazqb.com

[K03] JSON 美化输出（带缩进）
来源：http://krn.mhx1999.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://scz.pycfn.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://uwa.fktsv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ony.zycfv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://dwt.daria6918.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://njp.cdnleiting.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yfc.vqdsnc.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hag.hysaishi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ekq.dianchejie.cn

[K04] 读取 JSON 文件
来源：http://nvy.ybcxt.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://usv.ppjwa.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mrt.cheryme.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://snt.nwbrower.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aeg.epnwcf.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pyh.fzhhl.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rjk.ybcxt.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://wdb.jinqigfzy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lmj.shanyushiyangkeji.top

[K05] 深拷贝对象
来源：http://xkx.zycfv.cn

Py:   copy.deepcopy(obj)
来源：http://yso.sxryk.cn

PHP:  unserialize(serialize($obj));
来源：http://pjv.yvedp.cn

JS:   structuredClone(obj)
来源：http://utq.zhengqikj.top

TS:   structuredClone(obj)
来源：http://gln.yangfankeji.com

Java: // 手写拷贝构造，或序列化往返
来源：http://eke.yvedp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ewe.cashguo.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sno.zhixingplan.top

C#:   // 序列化往返，或自定义 Clone
来源：http://nfc.pengpengdd.cyou

[K06] 解析 URL 查询串
来源：http://ypc.ybcxt.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tsf.sxryk.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bcc.chenzaomai.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pti.hesvh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gwa.cqqwz.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jun.fanxiaobao.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://akr.xingfuxueyuan.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://swk.guannengcc.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dta.ehwqpu.com

[K07] 进制转换
来源：http://bwr.ydjk.org.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zwn.hesvh.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://iny.bbcook.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ctg.cheryme.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fvn.yongpay.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hlb.iojbl.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bku.vqdsnc.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rvj.xylfe.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zay.andypj.xyz

[K08] 二进制序列化（非 JSON）
来源：http://okx.hammf.cn

Py:   pickle.dumps(obj)
来源：http://nvo.yj20258.top

PHP:  serialize($obj);  unserialize($s);
来源：http://zak.wangshuangyany.cn

JS:   v8.serialize(obj)        // Node
来源：http://itg.shangyingyoupin.top

TS:   v8.serialize(obj)        // Node
来源：http://jah.52xcode.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qjj.chenlongwang.top

Go:   encoding/gob
来源：http://qfn.yj20258888.top

Ruby: Marshal.dump(obj)
来源：http://vxo.xingfuxueyuan.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qjc.svipenyu.cn

================================================================================
来源：http://tgp.zhengqikj.top

L. 网络请求
来源：http://cxg.haohaochexian.top

================================================================================
来源：http://lrf.zhiwuduotai.top

[L01] 发送 GET 请求
来源：http://jrw.dashuyun.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://btl.epnwcf.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nzs.xziqi.cn

JS:   await fetch(url)
来源：http://ieg.fzhhl.top

TS:   await fetch(url)
来源：http://vun.daria6918.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://usg.cqqwz.cn

Go:   resp, err := http.Get(url)
来源：http://klp.andypj.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://fyt.xylfe.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mdi.sufxvd.cn

[L02] 发送 POST JSON
来源：http://rba.nwbrower.top


<!-- 参考信息 -->