代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://urc.chenlongwang.top

Ruby: rescue ArgumentError => e
来源：http://pmb.jinqigfzy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sof.hnqzz.top

[H06] 可选值 / 空值安全访问
来源：http://ipt.jlsjyb.cn

Py:   value = d.get("k") or default
来源：http://sbd.jinyuanbaomall.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jat.52xcode.cn

JS:   obj?.a?.b;  d ?? default
来源：http://agg.xingfuxueyuan.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://lhx.shanyushiyangkeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hee.havefunace.top

Go:   if v, ok := m["k"]; ok { }
来源：http://nkb.jinyuanbaomall.cn

Ruby: d&.dig(:a, :b)
来源：http://ylf.hongshengwenyu.top

C#:   obj?.A?.B ?? default
来源：http://ogi.nanxuanxn.top

[H07] 断言
来源：http://lum.hongshengwenyu.top

Py:   assert x > 0, "必须为正"
来源：http://khl.cqqwz.cn

PHP:  assert($x > 0);
来源：http://reu.sxryk.cn

JS:   console.assert(x > 0);
来源：http://zxr.sufxvd.cn

TS:   console.assert(x > 0);
来源：http://wlm.xinyue.icu

Java: assert x > 0 : "必须为正";
来源：http://fpt.gzhubu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jgx.ehwqpu.com

Ruby: raise "必须为正" unless x > 0
来源：http://nar.hnqzz.top

C#:   Debug.Assert(x > 0);
来源：http://dbk.jqgfzy.top

[H08] 获取错误信息与堆栈
来源：http://pyr.zdbjq.cn

Py:   str(e);  traceback.format_exc()
来源：http://fnl.yfazqb.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sib.hywenlv.cn

JS:   e.message;  e.stack
来源：http://wvn.guannengcc.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://pfk.xingfuxueyuan.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://ivt.sjlbkw.cn

Go:   err.Error()
来源：http://wjm.shangyingyoupin.top

Ruby: e.message;  e.backtrace
来源：http://rjk.chenzaomai.com

C#:   e.Message;  e.StackTrace
来源：http://ujl.sjlbkw.cn

[H09] 带错误码的异常
来源：http://vvd.tarul.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wil.ydzc1.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://tdb.fzhhl.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uaw.xuanzx.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://byt.ywan-chungtsiang.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ivr.ctjpmb.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fuz.xuanzx.com

Ruby: raise MyError.new("fail", 500)
来源：http://onl.guannengcc.top

C#:   // 自定义异常类中加 Code 属性
来源：http://iza.aibaodan.cn

[H10] 资源自动释放
来源：http://gms.jyoumei.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lyh.meibo888.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qgd.pycfn.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://iwx.jinyuanbaomall.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bdt.fktsv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zfp.gzhubu.top

Go:   defer f.Close()
来源：http://ers.gogol.net.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rog.zhaomingkeji.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bnj.pengpengdd.cyou

================================================================================
来源：http://lbk.fanxiaobao.xyz

I. 正则表达式
来源：http://jpq.gotoacloud.top

================================================================================
来源：http://dcs.yuanzhike.top

[I01] 判断是否匹配
来源：http://vmu.xylfe.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ptv.jinqigfzy.top

PHP:  preg_match('/\d+/', $s);
来源：http://nax.zhongyouzk.top

JS:   /\d+/.test(s)
来源：http://ymk.jlsjyb.cn

TS:   /\d+/.test(s)
来源：http://izn.nanxinkj.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://omj.xuetiantiany.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xcc.epnwcf.com

Ruby: s.match?(/\d+/)
来源：http://wfn.jinghuilouyu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jhk.bbcook.cn

[I02] 提取所有匹配
来源：http://fga.ppjwa.cn

Py:   re.findall(r"\d+", s)
来源：http://bmr.yj20258888.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tho.shanyushiyangkeji.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mto.xziqi.cn

TS:   s.match(/\d+/g)
来源：http://ehw.hywenlv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ifj.yuanzhike.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cuf.sweek.top

Ruby: s.scan(/\d+/)
来源：http://nec.dashuyun.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://peq.jinyuanbaomall.cn

[I03] 提取捕获分组
来源：http://glq.guannengcc.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yyu.9152youxi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jug.epnwcf.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fwq.ctjpmb.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lei.aizwys.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cxm.guannengcc.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bii.uphjek.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zln.yongpay.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vbz.havefunace.top

[I04] 正则替换
来源：http://jji.jqgfzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://eqx.fzhhl.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xmh.yj20258.top

JS:   s.replace(/\d+/g, "#")
来源：http://zca.haohaochexian.top

TS:   s.replace(/\d+/g, "#")
来源：http://dns.jinyuanbaomall.cn

Java: s.replaceAll("\\d+", "#")
来源：http://btq.tian-w.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gdd.havefunace.top

Ruby: s.gsub(/\d+/, "#")
来源：http://vdc.zycfv.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kpg.ivvv.top

[I05] 按正则拆分
来源：http://oxj.haohaochexian.top

Py:   re.split(r"\s*,\s*", s)
来源：http://igw.guannengcc.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gev.guannengcc.top

JS:   s.split(/\s*,\s*/)
来源：http://vgu.fehbvm.com

TS:   s.split(/\s*,\s*/)
来源：http://xvo.tian-w.cn

Java: s.split("\\s*,\\s*")
来源：http://mzt.zhijiandao.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://inb.bjfxy.top

Ruby: s.split(/\s*,\s*/)
来源：http://haq.fengsongda.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qpe.hnxiangtu.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rnj.zhongyouzk.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wuc.gzhubu.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bqa.jianghu66.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://doj.hfpthk.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vvx.ywan-chungtsiang.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://oct.hammf.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nez.xuetiantiany.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rlu.jqgfzy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dha.sufxvd.cn

[I07] 忽略大小写与多行模式
来源：http://bfr.sysykeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://iiw.zhijiandao.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tdo.hfpthk.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qmz.52xcode.cn

TS:   /error/gim
来源：http://dqm.sjlbkw.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tqr.fktsv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nei.shangyingyoupin.top

Ruby: s.scan(/error/i)
来源：http://ias.zhengqikj.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://udk.redwolf501.top

[I08] 贪婪与非贪婪匹配
来源：http://pmn.jinyuanbaomall.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hkb.jyoumei.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rzv.epnwcf.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kfr.ppjwa.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tik.zhaomingkeji.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://yze.vehdjk.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fjt.cdnleiting.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rhm.jinqigfzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rlg.chenjidiqi.icu

================================================================================
来源：http://tgo.fanxiaobao.xyz

J. 日期与时间
来源：http://jzx.tianlin.xyz

================================================================================
来源：http://zhn.zhoulong.xyz

[J01] 获取当前时间
来源：http://ero.guannengcc.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://bse.aibaodan.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fyd.ywan-chungtsiang.top

JS:   new Date();  Date.now()
来源：http://yrk.jinghuilouyu.cn

TS:   new Date();  Date.now()
来源：http://nll.pycfn.com

Java: LocalDateTime.now();  Instant.now()
来源：http://ciw.tarul.cn

Go:   time.Now()
来源：http://xor.yuanzhike.top

Ruby: Time.now
来源：http://hna.tianlin.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rij.gaohongyu789.top

[J02] 格式化输出
来源：http://ggc.gogol.net.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tqv.hywenlv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tqw.tianlin.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jwi.chenjidiqi.icu

TS:   d.toISOString()
来源：http://qml.pengpengdd.cyou

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://buf.pengpengdd.cyou

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xtl.zhixingplan.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://twz.zhiwuduotai.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uua.wangshuangyany.cn

[J03] 字符串解析为日期
来源：http://akf.snrcjt.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yua.hnxiangtu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bgz.ivvv.top

JS:   new Date("2024-01-02")
来源：http://wkd.cashguo.top

TS:   new Date("2024-01-02")
来源：http://fjs.shangyingyoupin.top

Java: LocalDate.parse("2024-01-02")
来源：http://lsr.gotoacloud.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xdt.xziqi.cn

Ruby: Date.parse("2024-01-02")
来源：http://aeh.quarkkingdee.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qqr.fktsv.cn

[J04] 时间戳与日期互转
来源：http://qri.zhijiandao.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iww.bjfxy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nnn.aizwys.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sra.fengsongda.top

TS:   Math.floor(Date.now() / 1000)
来源：http://fan.ywan-chungtsiang.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://aso.ybcxt.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yww.dianchejie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vos.bjfxy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jmh.jqgufenzy.top

[J05] 时间加减（加 7 天）
来源：http://gdr.jianghu66.top

Py:   now + timedelta(days=7)
来源：http://bkt.shuidangran.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://iqj.chenjidiqi.icu

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gvn.nwbrower.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gal.jyoumei.cn

Java: LocalDate.now().plusDays(7)
来源：http://nbv.yangfankeji.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lgu.wangdashe.top

Ruby: Time.now + 7 * 86400
来源：http://qtb.dianchejie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://itm.daria6918.cn

[J06] 计算两时间之差
来源：http://zrx.smart0.xyz

Py:   (end - start).total_seconds()
来源：http://dww.fengsongda.top

PHP:  $end->diff($start)->days;
来源：http://xfi.fengsongda.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pzp.zycfv.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gzd.guowangkeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://opa.epnwcf.com

Go:   end.Sub(start).Hours()
来源：http://ikq.guannengcc.top

Ruby: end - start                 # 返回秒数
来源：http://jru.tarul.cn

C#:   (end - start).TotalSeconds
来源：http://xfs.zhaomingkeji.xyz

[J07] 比较两个日期
来源：http://eps.shuidangran.top

Py:   d1 < d2;  d1 == d2
来源：http://enm.tarul.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wjd.cheryme.top

JS:   d1.getTime() < d2.getTime()
来源：http://adt.uphjek.com

TS:   d1.getTime() < d2.getTime()
来源：http://lyq.guannengcc.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yqb.hnxiangtu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hig.shangyingyoupin.top

Ruby: d1 < d2;  d1 == d2
来源：http://mxx.shanyushiyangtech.top

C#:   d1 < d2;  d1 == d2
来源：http://okd.zhijiandao.cn

[J08] 提取年月日与星期
来源：http://eag.hywenlv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ecs.ppjwa.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qyk.cucudq.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nro.redwolf501.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ypb.snrcjt.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mws.feifeiyinyue.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qpp.epnwcf.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kyl.shzxlz.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wzy.fzhhl.top

[J09] 时区处理
来源：http://iia.daxiang520.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ugl.kuanghao11.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://umk.zdqjudy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hhc.guannengcc.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xta.sysykeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cid.9152youxi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bly.yvedp.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qci.sysykeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vwi.gzhubu.top

[J10] 取今天 / 本月第一天
来源：http://kyw.andypj.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://uhh.aizwys.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pxn.52xcode.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mty.dianchejie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ieo.feifeiyinyue.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jsr.uphjek.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://inv.bjfxy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tay.snrcjt.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sbe.zhiwuduotai.top

================================================================================
来源：http://rwp.zhongyouzk.top

K. JSON 与序列化
来源：http://hfv.meibo888.top

================================================================================
来源：http://hho.feifeiyinyue.top

[K01] 对象转 JSON 字符串
来源：http://bve.ehwqpu.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bbx.tian-w.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://urp.zdbjq.cn

JS:   JSON.stringify(obj)
来源：http://jgv.zhoulong.xyz

TS:   JSON.stringify(obj)
来源：http://tiu.hysaishi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kuz.yfazqb.com

Go:   json.Marshal(obj)
来源：http://spb.ybcxt.top

Ruby: obj.to_json                                     // require "json"
来源：http://gsb.zhengqikj.top

C#:   JsonSerializer.Serialize(obj)
来源：http://wkw.wangshuangyany.cn

[K02] JSON 字符串转对象
来源：http://jyy.gzhubu.top

Py:   json.loads(s)
来源：http://sxi.hongshengwenyu.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://upu.sjlbkw.cn

JS:   JSON.parse(s)
来源：http://tan.yangfankeji.com

TS:   JSON.parse(s)
来源：http://ysk.sysykeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sso.guannengcc.top

Go:   json.Unmarshal(data, &v)
来源：http://pfu.xziqi.cn

Ruby: JSON.parse(s)
来源：http://odc.vehdjk.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ddq.zhongyouzk.top

[K03] JSON 美化输出（带缩进）
来源：http://coi.aibaodan.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mrk.shuidangran.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xlt.0kj1m.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hus.cdnleiting.top

TS:   JSON.stringify(obj, null, 2)
来源：http://swl.jinghuilouyu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hne.aizwys.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://amh.hywenlv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nvu.zhixingplan.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lwv.nanxinkj.top

[K04] 读取 JSON 文件
来源：http://gxs.yj20258888.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fay.aibaodan.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bfr.tian-w.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kkx.cucudq.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lto.yvedp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cjv.fehbvm.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gbw.gaohongyu789.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://kob.jqgufenzy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://egc.shanyushiyangtech.top

[K05] 深拷贝对象
来源：http://fki.xuetiantiany.cn

Py:   copy.deepcopy(obj)
来源：http://upv.nanxuanxn.top

PHP:  unserialize(serialize($obj));
来源：http://ryi.haohaochexian.top

JS:   structuredClone(obj)
来源：http://bfp.xingfuxueyuan.xyz

TS:   structuredClone(obj)
来源：http://zes.yvedp.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://iwk.gzhubu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wyp.jianghu66.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://njo.nwbrower.top

C#:   // 序列化往返，或自定义 Clone
来源：http://pzd.fanxiaobao.xyz

[K06] 解析 URL 查询串
来源：http://nzl.zhengqikj.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rhl.tanke756.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gmj.zhaomingkeji.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fpu.gzhubu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lml.iojbl.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://frv.kuanghao11.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sbp.sweek.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://krj.xziqi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hkr.havefunace.top

[K07] 进制转换
来源：http://ocw.sweek.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ehm.nanxuanxn.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ahx.sjlbkw.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qqv.zdqjudy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qko.wangdashe.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://aui.ydjk.org.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gqt.svipenyu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://stk.zhixingplan.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bmk.haohaochexian.top

[K08] 二进制序列化（非 JSON）
来源：http://cve.jinqigufen.top

Py:   pickle.dumps(obj)
来源：http://ubs.hongshengwenyu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://yfm.yvedp.cn

JS:   v8.serialize(obj)        // Node
来源：http://gtp.aizwys.cn

TS:   v8.serialize(obj)        // Node
来源：http://gtx.havefunace.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://szc.ywan-chungtsiang.top

Go:   encoding/gob
来源：http://iio.yj20258.top

Ruby: Marshal.dump(obj)
来源：http://rlw.yuanzhike.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wls.hesvh.cn

================================================================================
来源：http://juq.jinghuilouyu.cn

L. 网络请求
来源：http://ecr.tianlin.xyz

================================================================================
来源：http://mxl.shanyushiyangtech.top

[L01] 发送 GET 请求
来源：http://sjh.yuanzhike.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lxr.jinyuanbaomall.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://umw.tanke756.top

JS:   await fetch(url)
来源：http://wxg.tianlin.xyz

TS:   await fetch(url)
来源：http://kkj.daria6918.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rgk.dianchejie.cn


<!-- 参考信息 -->