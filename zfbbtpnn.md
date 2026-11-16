代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://xdj.tian-w.cn

[H08] 获取错误信息与堆栈
来源：http://glh.pycfn.com

Py:   str(e);  traceback.format_exc()
来源：http://mdn.zhongyouzk.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kdx.kuanghao11.cn

JS:   e.message;  e.stack
来源：http://kxf.xziqi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vve.uphjek.com

Java: e.getMessage();  e.printStackTrace()
来源：http://rfj.hywenlv.cn

Go:   err.Error()
来源：http://ndk.yj20258888.top

Ruby: e.message;  e.backtrace
来源：http://nck.tianlin.xyz

C#:   e.Message;  e.StackTrace
来源：http://uxg.tianlin.xyz

[H09] 带错误码的异常
来源：http://tph.jinyuanbaomall.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fhy.jlsjyb.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://beq.epnwcf.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gtf.havefunace.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://phs.hcnkem.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lzr.yonumen.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://arb.yj202588.top

Ruby: raise MyError.new("fail", 500)
来源：http://fvo.gzhubu.top

C#:   // 自定义异常类中加 Code 属性
来源：http://miw.ehwqpu.com

[H10] 资源自动释放
来源：http://blk.hcnkem.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://rlv.xuanzx.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tph.zhoulong.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kjo.fengsongda.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nbz.dashuyun.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uif.sjlbkw.cn

Go:   defer f.Close()
来源：http://wnp.vehdjk.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nua.aibaodan.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hwd.cashguo.top

================================================================================
来源：http://vbw.jinghuilouyu.cn

I. 正则表达式
来源：http://nlc.gzhubu.top

================================================================================
来源：http://uul.guannengcc.top

[I01] 判断是否匹配
来源：http://uam.mhx1999.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lsq.hysaishi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wyx.haohaochexian.top

JS:   /\d+/.test(s)
来源：http://usb.sweek.top

TS:   /\d+/.test(s)
来源：http://eye.nwbrower.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://twz.redwolf501.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ywl.ctjpmb.com

Ruby: s.match?(/\d+/)
来源：http://ejk.tian-w.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ntz.jlsjyb.cn

[I02] 提取所有匹配
来源：http://uds.svipenyu.cn

Py:   re.findall(r"\d+", s)
来源：http://oju.gotoacloud.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://okh.ivvv.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nwl.yvedp.cn

TS:   s.match(/\d+/g)
来源：http://idm.svipenyu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://omv.fengsongda.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ywf.hysaishi.cn

Ruby: s.scan(/\d+/)
来源：http://waz.gaohongyu789.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rys.hnxiangtu.top

[I03] 提取捕获分组
来源：http://rlj.sweek.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ijl.hcnkem.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ndm.zhijiandao.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yvz.jlsjyb.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gfl.cqqwz.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kbz.guowangkeji.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lpy.gaohongyu789.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fmh.shanyushiyangkeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vso.cucudq.cn

[I04] 正则替换
来源：http://oam.zhongyouzk.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qud.zycfv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cyq.dianchejie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kej.ehwqpu.com

TS:   s.replace(/\d+/g, "#")
来源：http://fap.kuanghao11.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bnc.zdqjudy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ltu.sxryk.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qfr.hnxiangtu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wfa.birdmap.top

[I05] 按正则拆分
来源：http://mfg.redwolf501.top

Py:   re.split(r"\s*,\s*", s)
来源：http://bgn.zhoulong.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vgp.ydjk.org.cn

JS:   s.split(/\s*,\s*/)
来源：http://kiw.haohaochexian.top

TS:   s.split(/\s*,\s*/)
来源：http://gep.zhaomingkeji.xyz

Java: s.split("\\s*,\\s*")
来源：http://ahp.gotoacloud.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jzj.kuanghao11.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mcr.52xcode.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://eew.zhaomingkeji.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://erv.hfpthk.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dnz.aizwys.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kyp.chenzaomai.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pro.mhx1999.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yal.aizwys.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://scf.jinqigufen.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zpx.sjlbkw.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nkn.fzhhl.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://boy.zhixingplan.top

[I07] 忽略大小写与多行模式
来源：http://buf.jlsjyb.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ola.ybcxt.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bro.yueranfly.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ejy.52xcode.cn

TS:   /error/gim
来源：http://rnt.cucudq.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rlt.fktsv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lay.dashuyun.cn

Ruby: s.scan(/error/i)
来源：http://yrq.uphjek.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vel.hnxiangtu.top

[I08] 贪婪与非贪婪匹配
来源：http://puf.jinghuilouyu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gaa.316326.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ueq.aibaodan.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://shd.ywan-chungtsiang.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vjv.cqqwz.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hqq.nanxuanxn.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vul.jqgufenzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lfq.chenlongwang.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fqq.daxiang520.top

================================================================================
来源：http://wwp.gotoacloud.top

J. 日期与时间
来源：http://dkk.52xcode.cn

================================================================================
来源：http://xiu.xziqi.cn

[J01] 获取当前时间
来源：http://yzl.gzhubu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://izg.dashuyun.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ywu.zycfv.cn

JS:   new Date();  Date.now()
来源：http://zim.bbcook.cn

TS:   new Date();  Date.now()
来源：http://csl.hywenlv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://iax.xingfuxueyuan.xyz

Go:   time.Now()
来源：http://pxh.ydzc1.top

Ruby: Time.now
来源：http://jkq.sjlbkw.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://iia.ybcxt.top

[J02] 格式化输出
来源：http://ixj.bbcook.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://odt.bjfxy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rga.aizwys.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ziy.ppjwa.cn

TS:   d.toISOString()
来源：http://ver.hammf.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zwd.shangyingyoupin.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jvk.ywan-chungtsiang.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hbk.quarkkingdee.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://iuk.jqgfzy.top

[J03] 字符串解析为日期
来源：http://waw.tanke756.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pzx.jqgufenzy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pxa.cheryme.top

JS:   new Date("2024-01-02")
来源：http://wns.bbcook.cn

TS:   new Date("2024-01-02")
来源：http://hkl.ybcxt.top

Java: LocalDate.parse("2024-01-02")
来源：http://ytl.fanxiaobao.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pzn.jlsjyb.cn

Ruby: Date.parse("2024-01-02")
来源：http://ogc.gotoacloud.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ctf.zhiwuduotai.top

[J04] 时间戳与日期互转
来源：http://jkt.yonumen.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gnf.hywenlv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nlv.jinqigufen.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tnl.yanxiufei.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://guk.gaohongyu789.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wvp.ehwqpu.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hpr.zycfv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://izo.pycfn.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://liv.fengsongda.top

[J05] 时间加减（加 7 天）
来源：http://mhh.hongshengwenyu.top

Py:   now + timedelta(days=7)
来源：http://cgm.yfazqb.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://sgn.hcnkem.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://njy.sysykeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qqm.aizwys.cn

Java: LocalDate.now().plusDays(7)
来源：http://uwn.jianghu66.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://svj.ctjpmb.com

Ruby: Time.now + 7 * 86400
来源：http://tsi.shanyushiyangkeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://iem.ehwqpu.com

[J06] 计算两时间之差
来源：http://zmz.smart0.xyz

Py:   (end - start).total_seconds()
来源：http://gfn.hysaishi.cn

PHP:  $end->diff($start)->days;
来源：http://agq.sxryk.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ekk.shanyushiyangkeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sox.ydjk.org.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bix.tianlin.xyz

Go:   end.Sub(start).Hours()
来源：http://bit.sysykeji.top

Ruby: end - start                 # 返回秒数
来源：http://zgs.hfpthk.cn

C#:   (end - start).TotalSeconds
来源：http://cew.xingfuxueyuan.xyz

[J07] 比较两个日期
来源：http://pso.quarkkingdee.top

Py:   d1 < d2;  d1 == d2
来源：http://ayn.nanxinkj.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cly.daxiang520.top

JS:   d1.getTime() < d2.getTime()
来源：http://trm.yj20258.top

TS:   d1.getTime() < d2.getTime()
来源：http://dib.epnwcf.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ybx.dashuyun.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xrl.shangyingyoupin.top

Ruby: d1 < d2;  d1 == d2
来源：http://fnx.jqgfzy.top

C#:   d1 < d2;  d1 == d2
来源：http://dfh.birdmap.top

[J08] 提取年月日与星期
来源：http://akk.pycfn.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fgm.chenzaomai.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://odp.bbcook.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mez.yangfankeji.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rbi.gaohongyu789.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jxj.vqdsnc.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wde.zhoulong.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pus.jlsjyb.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ksp.jqgufenzy.top

[J09] 时区处理
来源：http://pqg.fzhhl.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://amw.sufxvd.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wts.52xcode.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zxs.daria6918.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wus.yj20258888.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hgv.cheryme.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lwx.vehdjk.com

Ruby: Time.now.getlocal("+08:00")
来源：http://ojr.bbcook.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://npz.ydzc1.top

[J10] 取今天 / 本月第一天
来源：http://sba.tian-w.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jel.ehwqpu.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sfp.zhijiandao.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://plx.0kj1m.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://prr.dianchejie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hxd.zhijiandao.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lae.jianghu66.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hdv.pengpengdd.cyou

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ash.316326.xyz

================================================================================
来源：http://hsb.svipenyu.cn

K. JSON 与序列化
来源：http://ehi.aibaodan.cn

================================================================================
来源：http://idu.haohaochexian.top

[K01] 对象转 JSON 字符串
来源：http://bxc.uphjek.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nrw.dashuyun.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vrc.9152youxi.cn

JS:   JSON.stringify(obj)
来源：http://zmk.pengpengdd.cyou

TS:   JSON.stringify(obj)
来源：http://thd.zdqjudy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nys.zhoulong.xyz

Go:   json.Marshal(obj)
来源：http://ris.wangshuangyany.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zgw.guannengcc.top

C#:   JsonSerializer.Serialize(obj)
来源：http://dxj.zdqjudy.top

[K02] JSON 字符串转对象
来源：http://spl.yvedp.cn

Py:   json.loads(s)
来源：http://vay.yueranfly.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://meq.daxiang520.top

JS:   JSON.parse(s)
来源：http://ywn.sysykeji.top

TS:   JSON.parse(s)
来源：http://pbo.jianghu66.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fzx.gogol.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://nfm.dianchejie.cn

Ruby: JSON.parse(s)
来源：http://ovz.guowangkeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ifw.aibaodan.cn

[K03] JSON 美化输出（带缩进）
来源：http://rud.cashguo.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rfo.zhixingplan.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mgz.shzxlz.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bns.gaohongyu789.top

TS:   JSON.stringify(obj, null, 2)
来源：http://naz.jinghuilouyu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yrx.yongpay.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lww.ctjpmb.com

Ruby: JSON.pretty_generate(obj)
来源：http://zja.havefunace.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qae.jlsjyb.cn

[K04] 读取 JSON 文件
来源：http://ase.hcnkem.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uim.c1oappe.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://byj.hnqzz.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ynb.fengsongda.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rai.smart0.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fig.yfazqb.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jdk.yangfankeji.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://bva.redwolf501.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nsc.sjlbkw.cn

[K05] 深拷贝对象
来源：http://ecn.hongshengwenyu.top

Py:   copy.deepcopy(obj)
来源：http://fdf.jyoumei.cn

PHP:  unserialize(serialize($obj));
来源：http://jwe.yuxming.cn

JS:   structuredClone(obj)
来源：http://izh.epnwcf.com

TS:   structuredClone(obj)
来源：http://qmm.bbcook.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xkn.ctjpmb.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://oec.dashuyun.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://djx.zhoulong.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://kvi.sysykeji.top

[K06] 解析 URL 查询串
来源：http://zur.andypj.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tgf.fengsongda.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://aff.havefunace.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://guc.redwolf501.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://scl.vqdsnc.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://clk.0kj1m.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bsv.aibaodan.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://psg.hfpthk.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pjy.mhx1999.top

[K07] 进制转换
来源：http://yft.yonumen.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gdu.gzhubu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mek.havefunace.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lxt.epnwcf.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ujj.birdmap.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qet.jiagoushi.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ech.yonumen.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ftx.snrcjt.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qeo.fanxiaobao.xyz

[K08] 二进制序列化（非 JSON）
来源：http://ngj.hcnkem.com

Py:   pickle.dumps(obj)
来源：http://axf.ppjwa.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pmp.fanxiaobao.xyz

JS:   v8.serialize(obj)        // Node
来源：http://pac.kuanghao11.cn

TS:   v8.serialize(obj)        // Node
来源：http://srs.hesvh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qin.ctjpmb.com

Go:   encoding/gob
来源：http://lgh.kuanghao11.cn

Ruby: Marshal.dump(obj)
来源：http://voz.zhijiandao.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rbl.hongshengwenyu.top

================================================================================
来源：http://eok.chenlongwang.top

L. 网络请求
来源：http://ges.zdbjq.cn

================================================================================
来源：http://mee.jiagoushi.top

[L01] 发送 GET 请求
来源：http://tto.havefunace.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://whr.hnxiangtu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fxk.shuidangran.top

JS:   await fetch(url)
来源：http://rjj.gogol.net.cn

TS:   await fetch(url)
来源：http://kzq.dashuyun.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://smk.xuanzx.com

Go:   resp, err := http.Get(url)
来源：http://ngg.hfpthk.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://eje.bjfxy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://srf.daxiang520.top

[L02] 发送 POST JSON
来源：http://azy.smart0.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://sut.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xfa.andypj.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vog.nanxuanxn.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ilt.zhoulong.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yms.hnqzz.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zql.52xcode.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gks.yvedp.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nwx.aizwys.cn

[L03] 设置自定义请求头
来源：http://wge.sxryk.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nvc.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uxq.hesvh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://idj.aizwys.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://otj.shanyushiyangtech.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lko.ivvv.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ktt.sysykeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zlk.tarul.cn


<!-- 参考信息 -->