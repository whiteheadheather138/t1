代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dke.sysykeji.top

Ruby: rescue ArgumentError => e
来源：http://cdo.fktsv.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gge.zhoulong.xyz

[H06] 可选值 / 空值安全访问
来源：http://cep.quarkkingdee.top

Py:   value = d.get("k") or default
来源：http://vam.haohaochexian.top

PHP:  $v = $d["k"] ?? null;
来源：http://yoc.shanyushiyangtech.top

JS:   obj?.a?.b;  d ?? default
来源：http://anv.havefunace.top

TS:   obj?.a?.b;  d ?? default
来源：http://fnz.daria6918.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hjy.0kj1m.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ekb.redwolf501.top

Ruby: d&.dig(:a, :b)
来源：http://wek.tian-w.cn

C#:   obj?.A?.B ?? default
来源：http://lvl.52xcode.cn

[H07] 断言
来源：http://uvx.jyoumei.cn

Py:   assert x > 0, "必须为正"
来源：http://ccy.chenjidiqi.icu

PHP:  assert($x > 0);
来源：http://nqy.sweek.top

JS:   console.assert(x > 0);
来源：http://cjg.daria6918.cn

TS:   console.assert(x > 0);
来源：http://zqt.zycfv.cn

Java: assert x > 0 : "必须为正";
来源：http://pge.yangfankeji.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gai.sufxvd.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bjj.kuanghao11.cn

C#:   Debug.Assert(x > 0);
来源：http://fuy.hywenlv.cn

[H08] 获取错误信息与堆栈
来源：http://twn.zhaomingkeji.xyz

Py:   str(e);  traceback.format_exc()
来源：http://xds.yangfankeji.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ahq.xylfe.cn

JS:   e.message;  e.stack
来源：http://pxq.hcnkem.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://hwr.jlsjyb.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://yry.guowangkeji.top

Go:   err.Error()
来源：http://dsv.jianghu66.top

Ruby: e.message;  e.backtrace
来源：http://ndq.zhaomingkeji.xyz

C#:   e.Message;  e.StackTrace
来源：http://djw.zhixingplan.top

[H09] 带错误码的异常
来源：http://nex.gotoacloud.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rdq.bbcook.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rer.ppjwa.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ave.shuidangran.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xfo.xylfe.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://caq.ehwqpu.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mes.yanxiufei.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wwt.ydzc1.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ocu.wangdashe.top

[H10] 资源自动释放
来源：http://loa.zhijiandao.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://sey.cdnleiting.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wxq.cdnleiting.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://otx.zhengqikj.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nts.xuanzx.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://giw.daxiang520.top

Go:   defer f.Close()
来源：http://oxf.yfazqb.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sga.yuxming.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gxb.cqqwz.cn

================================================================================
来源：http://xlp.nanxinkj.top

I. 正则表达式
来源：http://pps.yueranfly.top

================================================================================
来源：http://wdh.tian-w.cn

[I01] 判断是否匹配
来源：http://hgj.yj202588.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hfc.52xcode.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xro.yj202588.top

JS:   /\d+/.test(s)
来源：http://gxx.bbcook.cn

TS:   /\d+/.test(s)
来源：http://psp.bbcook.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xsz.jqgufenzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ouq.daria6918.cn

Ruby: s.match?(/\d+/)
来源：http://yop.bjfxy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gwv.vehdjk.com

[I02] 提取所有匹配
来源：http://kcc.ybcxt.top

Py:   re.findall(r"\d+", s)
来源：http://hqm.aizwys.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://irm.zdqjudy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kse.jlsjyb.cn

TS:   s.match(/\d+/g)
来源：http://jhg.ctjpmb.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://swm.iojbl.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nuo.yj202588.top

Ruby: s.scan(/\d+/)
来源：http://kor.zhijiandao.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vfd.jqgufenzy.top

[I03] 提取捕获分组
来源：http://mcu.zhijiandao.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://aet.hywenlv.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://oaq.epnwcf.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://trp.316326.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mvk.hysaishi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vdg.chenlongwang.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ual.xinyue.icu

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jxw.yj20258.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kfd.fengsongda.top

[I04] 正则替换
来源：http://bxz.tianlin.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://jlr.yj20258888.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qke.ybcxt.top

JS:   s.replace(/\d+/g, "#")
来源：http://hzl.xingfuxueyuan.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://ngy.epnwcf.com

Java: s.replaceAll("\\d+", "#")
来源：http://eda.birdmap.top

Go:   re.ReplaceAllString(s, "#")
来源：http://zsl.yongpay.top

Ruby: s.gsub(/\d+/, "#")
来源：http://asv.zhoulong.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://meq.zhaomingkeji.xyz

[I05] 按正则拆分
来源：http://tvu.ehwqpu.com

Py:   re.split(r"\s*,\s*", s)
来源：http://men.feifeiyinyue.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lvc.yj20258.top

JS:   s.split(/\s*,\s*/)
来源：http://gsx.jyoumei.cn

TS:   s.split(/\s*,\s*/)
来源：http://zkt.vqdsnc.cn

Java: s.split("\\s*,\\s*")
来源：http://mym.guannengcc.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://iwx.xuetiantiany.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gvv.hesvh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lkn.zdbjq.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://stg.xylfe.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://oqh.xuanzx.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://adh.yanxiufei.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rhy.dianchejie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pfe.yangfankeji.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ghh.wangshuangyany.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qyo.cashguo.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ouu.pengpengdd.cyou

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yix.jiagoushi.top

[I07] 忽略大小写与多行模式
来源：http://jih.shangyingyoupin.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ifh.chenlongwang.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ady.ydzc1.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hau.zhaomingkeji.xyz

TS:   /error/gim
来源：http://jgf.ydjk.org.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://emj.hongshengwenyu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jlv.fengsongda.top

Ruby: s.scan(/error/i)
来源：http://wcb.jianghu66.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ooz.hysaishi.cn

[I08] 贪婪与非贪婪匹配
来源：http://zef.yvedp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fvn.cashguo.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ips.xylfe.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pzq.zdbjq.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tmp.ehwqpu.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://vbi.hywenlv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mny.chenzaomai.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oqa.jqgufenzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jar.andypj.xyz

================================================================================
来源：http://ljp.c1oappe.top

J. 日期与时间
来源：http://tpd.jinqigufen.top

================================================================================
来源：http://lmo.xinyue.icu

[J01] 获取当前时间
来源：http://srv.ybcxt.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://lbk.aibaodan.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sck.gzhubu.top

JS:   new Date();  Date.now()
来源：http://qwh.hnqzz.top

TS:   new Date();  Date.now()
来源：http://oez.zhijiandao.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://sdg.uphjek.com

Go:   time.Now()
来源：http://jqt.vqdsnc.cn

Ruby: Time.now
来源：http://wep.zdqjudy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://raf.hysaishi.cn

[J02] 格式化输出
来源：http://xbh.hnqzz.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://atx.zhijiandao.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cmn.yj20258.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mig.zdqjudy.top

TS:   d.toISOString()
来源：http://sru.zhijiandao.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rnb.hfpthk.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hst.jiagoushi.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zuy.chenzaomai.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qpm.ehwqpu.com

[J03] 字符串解析为日期
来源：http://lpu.pycfn.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lqw.zhoulong.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://osu.yonumen.top

JS:   new Date("2024-01-02")
来源：http://efi.xylfe.cn

TS:   new Date("2024-01-02")
来源：http://zwe.wangshuangyany.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pyl.mhx1999.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rrm.zycfv.cn

Ruby: Date.parse("2024-01-02")
来源：http://sef.yangfankeji.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cud.guannengcc.top

[J04] 时间戳与日期互转
来源：http://wew.jinqigufen.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://maf.yanxiufei.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iuh.0kj1m.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zcg.yfazqb.com

TS:   Math.floor(Date.now() / 1000)
来源：http://qir.tianlin.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dzc.tarul.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://aig.9152youxi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://apw.cheryme.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uzl.gogol.net.cn

[J05] 时间加减（加 7 天）
来源：http://uiz.ehwqpu.com

Py:   now + timedelta(days=7)
来源：http://lff.jinqigufen.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://erf.gaohongyu789.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://aww.zhixingplan.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cuq.ydzc1.top

Java: LocalDate.now().plusDays(7)
来源：http://twh.52xcode.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ffw.chenjidiqi.icu

Ruby: Time.now + 7 * 86400
来源：http://ybo.jqgufenzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://aoo.gaohongyu789.top

[J06] 计算两时间之差
来源：http://oif.tarul.cn

Py:   (end - start).total_seconds()
来源：http://aao.xingfuxueyuan.xyz

PHP:  $end->diff($start)->days;
来源：http://icf.ppjwa.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wjo.zhoulong.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dxr.epnwcf.com

Java: Duration.between(start, end).toSeconds()
来源：http://xrt.yuanzhike.top

Go:   end.Sub(start).Hours()
来源：http://dzs.jinqigufen.top

Ruby: end - start                 # 返回秒数
来源：http://der.zhixingplan.top

C#:   (end - start).TotalSeconds
来源：http://jzs.nwbrower.top

[J07] 比较两个日期
来源：http://zut.shanyushiyangkeji.top

Py:   d1 < d2;  d1 == d2
来源：http://ayg.sxryk.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://din.nanxuanxn.top

JS:   d1.getTime() < d2.getTime()
来源：http://qrx.zhengqikj.top

TS:   d1.getTime() < d2.getTime()
来源：http://bbc.havefunace.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hot.zhaomingkeji.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qbx.pycfn.com

Ruby: d1 < d2;  d1 == d2
来源：http://pcu.shanyushiyangkeji.top

C#:   d1 < d2;  d1 == d2
来源：http://juz.sysykeji.top

[J08] 提取年月日与星期
来源：http://rft.sweek.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mmy.gogol.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zxy.zdbjq.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xgf.jqgfzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fgt.aibaodan.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ycc.yangfankeji.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dvb.fengsongda.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wft.ehwqpu.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://awr.yonumen.top

[J09] 时区处理
来源：http://rph.pycfn.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qwh.yuxming.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hwl.redwolf501.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hfb.xuetiantiany.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://evi.fengsongda.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fnw.zhixingplan.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fba.ehwqpu.com

Ruby: Time.now.getlocal("+08:00")
来源：http://kdg.shzxlz.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mcy.jinghuilouyu.cn

[J10] 取今天 / 本月第一天
来源：http://cpz.chenjidiqi.icu

Py:   date.today();  date.today().replace(day=1)
来源：http://mst.daria6918.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jmh.sufxvd.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cmz.chenlongwang.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://byu.gaohongyu789.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rtp.xuanzx.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vix.wangdashe.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ctg.cdnleiting.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://svz.316326.xyz

================================================================================
来源：http://bdb.dianchejie.cn

K. JSON 与序列化
来源：http://hee.zhijiandao.cn

================================================================================
来源：http://wwe.sxryk.cn

[K01] 对象转 JSON 字符串
来源：http://zme.aibaodan.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rdm.guannengcc.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tgb.xingfuxueyuan.xyz

JS:   JSON.stringify(obj)
来源：http://pya.xingfuxueyuan.xyz

TS:   JSON.stringify(obj)
来源：http://end.xuetiantiany.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gic.gogol.net.cn

Go:   json.Marshal(obj)
来源：http://qwk.sxryk.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jqh.iojbl.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zks.havefunace.top

[K02] JSON 字符串转对象
来源：http://biv.hesvh.cn

Py:   json.loads(s)
来源：http://tvl.daria6918.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jfv.xinyue.icu

JS:   JSON.parse(s)
来源：http://yft.fehbvm.com

TS:   JSON.parse(s)
来源：http://lrk.tianlin.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qxd.zhijiandao.cn

Go:   json.Unmarshal(data, &v)
来源：http://btz.jqgufenzy.top

Ruby: JSON.parse(s)
来源：http://fyl.yvedp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hhv.ctjpmb.com

[K03] JSON 美化输出（带缩进）
来源：http://nrt.yuanzhike.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mgp.jinqigfzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vcy.shuidangran.top

JS:   JSON.stringify(obj, null, 2)
来源：http://roh.316326.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://pmb.jinghuilouyu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nok.yj20258.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qqy.tarul.cn

Ruby: JSON.pretty_generate(obj)
来源：http://eap.fktsv.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lqs.mhx1999.top

[K04] 读取 JSON 文件
来源：http://unj.0kj1m.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nkw.tarul.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://thp.gzhubu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pvj.nanxinkj.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://prj.shangyingyoupin.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bmi.zhoulong.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dvq.cucudq.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gth.ybcxt.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qty.xuetiantiany.cn

[K05] 深拷贝对象
来源：http://xpb.jinqigfzy.top

Py:   copy.deepcopy(obj)
来源：http://oig.jinqigufen.top

PHP:  unserialize(serialize($obj));
来源：http://qbz.ehwqpu.com

JS:   structuredClone(obj)
来源：http://fih.zhiwuduotai.top

TS:   structuredClone(obj)
来源：http://lso.hammf.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://utw.chenzaomai.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tfh.gotoacloud.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wgo.gotoacloud.top

C#:   // 序列化往返，或自定义 Clone
来源：http://szi.sweek.top

[K06] 解析 URL 查询串
来源：http://jwp.jqgfzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zmu.nanxinkj.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mpx.sysykeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fgn.daria6918.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bgp.cucudq.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jbu.nwbrower.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://dkh.vehdjk.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jfx.havefunace.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lrp.bjfxy.top

[K07] 进制转换
来源：http://fue.haohaochexian.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zdz.316326.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tna.dashuyun.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xur.nanxinkj.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uoy.quarkkingdee.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bel.pengpengdd.cyou

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rlb.fehbvm.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://egn.jinqigfzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ynb.tarul.cn

[K08] 二进制序列化（非 JSON）
来源：http://mvf.andypj.xyz

Py:   pickle.dumps(obj)
来源：http://feh.jqgfzy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://amp.guowangkeji.top

JS:   v8.serialize(obj)        // Node
来源：http://hji.fengsongda.top

TS:   v8.serialize(obj)        // Node
来源：http://ipo.sxryk.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rcg.pycfn.com

Go:   encoding/gob
来源：http://anu.shanyushiyangtech.top

Ruby: Marshal.dump(obj)
来源：http://qmw.sysykeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tun.tarul.cn

================================================================================
来源：http://xsq.316326.xyz

L. 网络请求
来源：http://qba.wangshuangyany.cn

================================================================================
来源：http://qjv.xuanzx.com

[L01] 发送 GET 请求
来源：http://zvi.guannengcc.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://abc.daxiang520.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://obs.hongshengwenyu.top

JS:   await fetch(url)
来源：http://lui.bbcook.cn

TS:   await fetch(url)
来源：http://eqt.tanke756.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uph.bjfxy.top


<!-- 参考信息 -->