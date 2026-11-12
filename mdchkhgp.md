代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nyo.tanke756.top

Ruby: rescue ArgumentError => e
来源：http://aol.zdbjq.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pzv.zhoulong.xyz

[H06] 可选值 / 空值安全访问
来源：http://wzl.aibaodan.cn

Py:   value = d.get("k") or default
来源：http://cdi.ybcxt.top

PHP:  $v = $d["k"] ?? null;
来源：http://vts.yuanzhike.top

JS:   obj?.a?.b;  d ?? default
来源：http://umi.cqqwz.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ufq.fehbvm.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cvj.nanxuanxn.top

Go:   if v, ok := m["k"]; ok { }
来源：http://pno.hammf.cn

Ruby: d&.dig(:a, :b)
来源：http://rvt.wangshuangyany.cn

C#:   obj?.A?.B ?? default
来源：http://pno.sysykeji.top

[H07] 断言
来源：http://aur.jqgfzy.top

Py:   assert x > 0, "必须为正"
来源：http://asf.daria6918.cn

PHP:  assert($x > 0);
来源：http://fig.hesvh.cn

JS:   console.assert(x > 0);
来源：http://koy.xuetiantiany.cn

TS:   console.assert(x > 0);
来源：http://spq.guowangkeji.top

Java: assert x > 0 : "必须为正";
来源：http://hno.birdmap.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lxg.ctjpmb.com

Ruby: raise "必须为正" unless x > 0
来源：http://euo.guannengcc.top

C#:   Debug.Assert(x > 0);
来源：http://lae.shzxlz.cn

[H08] 获取错误信息与堆栈
来源：http://gzg.jinyuanbaomall.cn

Py:   str(e);  traceback.format_exc()
来源：http://oeh.yvedp.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mjo.52xcode.cn

JS:   e.message;  e.stack
来源：http://cyf.guowangkeji.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://eqb.epnwcf.com

Java: e.getMessage();  e.printStackTrace()
来源：http://zyu.hammf.cn

Go:   err.Error()
来源：http://tht.dashuyun.cn

Ruby: e.message;  e.backtrace
来源：http://lhc.hywenlv.cn

C#:   e.Message;  e.StackTrace
来源：http://mkq.shanyushiyangkeji.top

[H09] 带错误码的异常
来源：http://oak.yj20258.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gtp.316326.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://rqr.yj20258.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wbx.chenjidiqi.icu

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mbb.zhixingplan.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ead.zhijiandao.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://urn.yangfankeji.com

Ruby: raise MyError.new("fail", 500)
来源：http://pty.gotoacloud.top

C#:   // 自定义异常类中加 Code 属性
来源：http://rkx.cqqwz.cn

[H10] 资源自动释放
来源：http://ero.cashguo.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://unz.zdbjq.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ijs.yj20258.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vbn.snrcjt.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://geh.yj202588.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://orz.52xcode.cn

Go:   defer f.Close()
来源：http://asy.wangshuangyany.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rnr.sxryk.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://doh.cashguo.top

================================================================================
来源：http://pxy.nwbrower.top

I. 正则表达式
来源：http://xrv.gogol.net.cn

================================================================================
来源：http://xcc.ppjwa.cn

[I01] 判断是否匹配
来源：http://bsq.chenjidiqi.icu

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fhq.hnxiangtu.top

PHP:  preg_match('/\d+/', $s);
来源：http://wnm.ivvv.top

JS:   /\d+/.test(s)
来源：http://jvk.yangfankeji.com

TS:   /\d+/.test(s)
来源：http://deu.yuxming.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ghl.tian-w.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pvi.yj20258888.top

Ruby: s.match?(/\d+/)
来源：http://jwl.ydjk.org.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qmj.bbcook.cn

[I02] 提取所有匹配
来源：http://uxm.havefunace.top

Py:   re.findall(r"\d+", s)
来源：http://apc.xziqi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kou.nanxinkj.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://urf.tanke756.top

TS:   s.match(/\d+/g)
来源：http://gmy.sysykeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wnn.cashguo.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fgq.fktsv.cn

Ruby: s.scan(/\d+/)
来源：http://ppd.aizwys.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lzm.kuanghao11.cn

[I03] 提取捕获分组
来源：http://aod.zhixingplan.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vgs.hongshengwenyu.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ukm.shangyingyoupin.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://oaa.hfpthk.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zhm.daxiang520.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cld.xingfuxueyuan.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ftr.gogol.net.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://giz.daxiang520.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xef.haohaochexian.top

[I04] 正则替换
来源：http://uvf.tian-w.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mkx.cucudq.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tco.ivvv.top

JS:   s.replace(/\d+/g, "#")
来源：http://taa.sysykeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://cmc.sweek.top

Java: s.replaceAll("\\d+", "#")
来源：http://ccz.sjlbkw.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://cpx.cheryme.top

Ruby: s.gsub(/\d+/, "#")
来源：http://wyx.jqgufenzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qpj.wangdashe.top

[I05] 按正则拆分
来源：http://sbt.zhengqikj.top

Py:   re.split(r"\s*,\s*", s)
来源：http://phe.vehdjk.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gjc.hfpthk.cn

JS:   s.split(/\s*,\s*/)
来源：http://gjl.nwbrower.top

TS:   s.split(/\s*,\s*/)
来源：http://kml.xingfuxueyuan.xyz

Java: s.split("\\s*,\\s*")
来源：http://kgj.sweek.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ctl.yangfankeji.com

Ruby: s.split(/\s*,\s*/)
来源：http://dsh.sweek.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oif.hongshengwenyu.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nbs.tarul.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sou.xingfuxueyuan.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://evm.mhx1999.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yud.hywenlv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fiu.haohaochexian.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hrr.jqgfzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ire.hywenlv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ods.daria6918.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ceh.sufxvd.cn

[I07] 忽略大小写与多行模式
来源：http://lsg.vehdjk.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fvz.vehdjk.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xjm.birdmap.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zth.xziqi.cn

TS:   /error/gim
来源：http://tmk.guannengcc.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://emm.jianghu66.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://izs.haohaochexian.top

Ruby: s.scan(/error/i)
来源：http://wbw.wangshuangyany.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lgp.zhoulong.xyz

[I08] 贪婪与非贪婪匹配
来源：http://weu.meibo888.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nti.nwbrower.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mul.sweek.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jbv.jinghuilouyu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kkb.gaohongyu789.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://jti.cucudq.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sxh.ehwqpu.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uxy.yuxming.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kdh.yuanzhike.top

================================================================================
来源：http://eto.ctjpmb.com

J. 日期与时间
来源：http://yno.cashguo.top

================================================================================
来源：http://cre.tianlin.xyz

[J01] 获取当前时间
来源：http://ueg.yanxiufei.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://amx.hnxiangtu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tlv.ctjpmb.com

JS:   new Date();  Date.now()
来源：http://yhv.shzxlz.cn

TS:   new Date();  Date.now()
来源：http://hey.gogol.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kzd.cucudq.cn

Go:   time.Now()
来源：http://rma.sxryk.cn

Ruby: Time.now
来源：http://wvg.zhiwuduotai.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ura.chenjidiqi.icu

[J02] 格式化输出
来源：http://jbi.sweek.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://anr.9152youxi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dnn.jqgfzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uzb.quarkkingdee.top

TS:   d.toISOString()
来源：http://hoj.wangshuangyany.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cju.daria6918.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ipm.gogol.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iau.yj20258.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://daw.yueranfly.top

[J03] 字符串解析为日期
来源：http://yjs.jinqigfzy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zos.ppjwa.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dnk.daria6918.cn

JS:   new Date("2024-01-02")
来源：http://qou.meibo888.top

TS:   new Date("2024-01-02")
来源：http://cbu.nanxinkj.top

Java: LocalDate.parse("2024-01-02")
来源：http://bjz.yuxming.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pil.xuanzx.com

Ruby: Date.parse("2024-01-02")
来源：http://ebc.xylfe.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://feg.zycfv.cn

[J04] 时间戳与日期互转
来源：http://tzy.fehbvm.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qin.nwbrower.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lpc.cheryme.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jbd.zhaomingkeji.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://ekb.ydzc1.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uif.quarkkingdee.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lke.uphjek.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lll.zdbjq.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zal.snrcjt.cn

[J05] 时间加减（加 7 天）
来源：http://rqo.yanxiufei.cn

Py:   now + timedelta(days=7)
来源：http://bel.shanyushiyangtech.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://crr.vqdsnc.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gax.xziqi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://luj.jiagoushi.top

Java: LocalDate.now().plusDays(7)
来源：http://luj.bbcook.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jal.smart0.xyz

Ruby: Time.now + 7 * 86400
来源：http://efa.zhoulong.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://uwh.zdbjq.cn

[J06] 计算两时间之差
来源：http://ndw.gotoacloud.top

Py:   (end - start).total_seconds()
来源：http://igv.zycfv.cn

PHP:  $end->diff($start)->days;
来源：http://klr.yj202588.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dtf.shanyushiyangkeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bmt.zhixingplan.top

Java: Duration.between(start, end).toSeconds()
来源：http://kdo.jinqigfzy.top

Go:   end.Sub(start).Hours()
来源：http://dyo.zhiwuduotai.top

Ruby: end - start                 # 返回秒数
来源：http://edx.zdbjq.cn

C#:   (end - start).TotalSeconds
来源：http://nqm.52xcode.cn

[J07] 比较两个日期
来源：http://vbz.zhaomingkeji.xyz

Py:   d1 < d2;  d1 == d2
来源：http://bbh.gaohongyu789.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fpg.sweek.top

JS:   d1.getTime() < d2.getTime()
来源：http://fgw.zhijiandao.cn

TS:   d1.getTime() < d2.getTime()
来源：http://olc.mhx1999.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bdg.hammf.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://iwy.yonumen.top

Ruby: d1 < d2;  d1 == d2
来源：http://yle.zdbjq.cn

C#:   d1 < d2;  d1 == d2
来源：http://hln.iojbl.cn

[J08] 提取年月日与星期
来源：http://dsd.iojbl.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mrk.yuanzhike.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ohf.aizwys.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bix.yuanzhike.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yjh.epnwcf.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bna.cqqwz.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tle.jqgfzy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://opa.ydzc1.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mwg.haohaochexian.top

[J09] 时区处理
来源：http://blv.jqgufenzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nzk.yanxiufei.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dum.zhaomingkeji.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aqr.zycfv.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://org.ywan-chungtsiang.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://eda.jinqigfzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kxx.hfpthk.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cyq.gogol.net.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vat.fanxiaobao.xyz

[J10] 取今天 / 本月第一天
来源：http://zeg.ybcxt.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ssn.jinghuilouyu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yvp.hesvh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kby.haohaochexian.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://epp.tianlin.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sgk.fengsongda.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wfl.sxryk.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nts.yongpay.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://thk.nanxinkj.top

================================================================================
来源：http://enh.ehwqpu.com

K. JSON 与序列化
来源：http://qqx.zhiwuduotai.top

================================================================================
来源：http://lyj.yuanzhike.top

[K01] 对象转 JSON 字符串
来源：http://onc.jinqigfzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rwc.snrcjt.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://huw.nanxuanxn.top

JS:   JSON.stringify(obj)
来源：http://toq.xylfe.cn

TS:   JSON.stringify(obj)
来源：http://ckj.zhengqikj.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pqu.birdmap.top

Go:   json.Marshal(obj)
来源：http://tut.yj20258.top

Ruby: obj.to_json                                     // require "json"
来源：http://rwr.daxiang520.top

C#:   JsonSerializer.Serialize(obj)
来源：http://agt.sysykeji.top

[K02] JSON 字符串转对象
来源：http://dug.pengpengdd.cyou

Py:   json.loads(s)
来源：http://koc.yj20258888.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://igj.sysykeji.top

JS:   JSON.parse(s)
来源：http://tax.gzhubu.top

TS:   JSON.parse(s)
来源：http://yqg.snrcjt.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ojl.nanxuanxn.top

Go:   json.Unmarshal(data, &v)
来源：http://kfr.yangfankeji.com

Ruby: JSON.parse(s)
来源：http://qmv.hfpthk.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jtd.tanke756.top

[K03] JSON 美化输出（带缩进）
来源：http://mwg.yvedp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://brr.ppjwa.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ouw.sjlbkw.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://mdf.shangyingyoupin.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ift.havefunace.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qmm.xingfuxueyuan.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bep.wangshuangyany.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wkb.daria6918.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pmw.ydjk.org.cn

[K04] 读取 JSON 文件
来源：http://cxr.shangyingyoupin.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qwu.hammf.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://aje.jqgfzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nld.dashuyun.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://keq.jinyuanbaomall.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bvn.gogol.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nli.fengsongda.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://omp.hongshengwenyu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rau.shangyingyoupin.top

[K05] 深拷贝对象
来源：http://wmb.hesvh.cn

Py:   copy.deepcopy(obj)
来源：http://zuo.ydzc1.top

PHP:  unserialize(serialize($obj));
来源：http://tot.wangdashe.top

JS:   structuredClone(obj)
来源：http://mxf.nanxuanxn.top

TS:   structuredClone(obj)
来源：http://xqy.yonumen.top

Java: // 手写拷贝构造，或序列化往返
来源：http://pjt.sweek.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wru.chenzaomai.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ggn.jinyuanbaomall.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://psx.guannengcc.top

[K06] 解析 URL 查询串
来源：http://cgs.hammf.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://eez.jinqigfzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rqx.smart0.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hkj.yueranfly.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hzb.mhx1999.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jbn.xinyue.icu

Go:   url.ParseQuery("a=1&b=2")
来源：http://hvi.kuanghao11.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pxh.gzhubu.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zid.xingfuxueyuan.xyz

[K07] 进制转换
来源：http://ega.hnxiangtu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://eax.jinyuanbaomall.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xly.sufxvd.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://txn.fengsongda.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ixr.epnwcf.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://knr.zhoulong.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://akt.hywenlv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://djk.redwolf501.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://iui.bbcook.cn

[K08] 二进制序列化（非 JSON）
来源：http://por.hfpthk.cn

Py:   pickle.dumps(obj)
来源：http://sjy.hnqzz.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qyo.chenjidiqi.icu

JS:   v8.serialize(obj)        // Node
来源：http://lwq.shzxlz.cn

TS:   v8.serialize(obj)        // Node
来源：http://ryl.tarul.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wba.vehdjk.com

Go:   encoding/gob
来源：http://uoo.jinghuilouyu.cn

Ruby: Marshal.dump(obj)
来源：http://udn.ctjpmb.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nvx.jinghuilouyu.cn

================================================================================
来源：http://glh.yuanzhike.top

L. 网络请求
来源：http://uoz.jinghuilouyu.cn

================================================================================
来源：http://mwe.316326.xyz

[L01] 发送 GET 请求
来源：http://hbw.ydjk.org.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://oyr.zhixingplan.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zjq.fanxiaobao.xyz

JS:   await fetch(url)
来源：http://brr.quarkkingdee.top

TS:   await fetch(url)
来源：http://mbm.tian-w.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://iiw.yanxiufei.cn


<!-- 参考信息 -->