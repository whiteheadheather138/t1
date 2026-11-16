代发 wailian999

[H07] 断言
来源：http://cjg.feifeiyinyue.top

Py:   assert x > 0, "必须为正"
来源：http://qjr.xylfe.cn

PHP:  assert($x > 0);
来源：http://vkc.shangyingyoupin.top

JS:   console.assert(x > 0);
来源：http://kpi.xinyue.icu

TS:   console.assert(x > 0);
来源：http://pyz.gogol.net.cn

Java: assert x > 0 : "必须为正";
来源：http://txm.yuxming.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xrc.bbcook.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xnk.cucudq.cn

C#:   Debug.Assert(x > 0);
来源：http://kug.sxryk.cn

[H08] 获取错误信息与堆栈
来源：http://tgq.ctjpmb.com

Py:   str(e);  traceback.format_exc()
来源：http://usf.sweek.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fnf.zycfv.cn

JS:   e.message;  e.stack
来源：http://jxs.zhaomingkeji.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://wpr.guowangkeji.top

Java: e.getMessage();  e.printStackTrace()
来源：http://obb.ivvv.top

Go:   err.Error()
来源：http://umu.zhoulong.xyz

Ruby: e.message;  e.backtrace
来源：http://ikl.sysykeji.top

C#:   e.Message;  e.StackTrace
来源：http://ybj.jinqigfzy.top

[H09] 带错误码的异常
来源：http://fcw.shanyushiyangkeji.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tbq.andypj.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://ppr.yj20258888.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://isu.iojbl.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vtf.pycfn.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fgq.chenjidiqi.icu

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sbi.dashuyun.cn

Ruby: raise MyError.new("fail", 500)
来源：http://tje.ybcxt.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xlc.daria6918.cn

[H10] 资源自动释放
来源：http://ahm.jiagoushi.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://bvg.snrcjt.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vqr.feifeiyinyue.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://itj.hnxiangtu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://czt.hysaishi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zli.daxiang520.top

Go:   defer f.Close()
来源：http://iok.haohaochexian.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://svm.yj20258888.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dhk.jinqigufen.top

================================================================================
来源：http://tkn.jinqigfzy.top

I. 正则表达式
来源：http://bij.sufxvd.cn

================================================================================
来源：http://rss.yangfankeji.com

[I01] 判断是否匹配
来源：http://xek.dashuyun.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hbx.epnwcf.com

PHP:  preg_match('/\d+/', $s);
来源：http://anl.jinqigfzy.top

JS:   /\d+/.test(s)
来源：http://cgj.gogol.net.cn

TS:   /\d+/.test(s)
来源：http://nef.cqqwz.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://eqa.bjfxy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dmd.redwolf501.top

Ruby: s.match?(/\d+/)
来源：http://qpw.gogol.net.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://flb.guannengcc.top

[I02] 提取所有匹配
来源：http://urt.hnqzz.top

Py:   re.findall(r"\d+", s)
来源：http://eqi.nanxuanxn.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ejp.ppjwa.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://son.zhixingplan.top

TS:   s.match(/\d+/g)
来源：http://pet.zdbjq.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rho.redwolf501.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ajz.andypj.xyz

Ruby: s.scan(/\d+/)
来源：http://mbu.zdqjudy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hnl.jinghuilouyu.cn

[I03] 提取捕获分组
来源：http://ppw.yvedp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://eba.fehbvm.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ggp.andypj.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ybd.fzhhl.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lwm.cucudq.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ogg.fanxiaobao.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ily.wangdashe.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xwc.jqgfzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gfa.quarkkingdee.top

[I04] 正则替换
来源：http://ohm.xylfe.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wqw.tanke756.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qhz.yueranfly.top

JS:   s.replace(/\d+/g, "#")
来源：http://fus.zdbjq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cjx.nanxuanxn.top

Java: s.replaceAll("\\d+", "#")
来源：http://iay.gotoacloud.top

Go:   re.ReplaceAllString(s, "#")
来源：http://jtx.xylfe.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://lhg.hywenlv.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ehf.jqgufenzy.top

[I05] 按正则拆分
来源：http://nux.havefunace.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ton.tianlin.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qed.vehdjk.com

JS:   s.split(/\s*,\s*/)
来源：http://vkx.bjfxy.top

TS:   s.split(/\s*,\s*/)
来源：http://vtc.guannengcc.top

Java: s.split("\\s*,\\s*")
来源：http://kjy.vqdsnc.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qiz.pycfn.com

Ruby: s.split(/\s*,\s*/)
来源：http://acv.hongshengwenyu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fpo.yj202588.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qsx.cdnleiting.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kns.ydzc1.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://trz.zhiwuduotai.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nfn.zdqjudy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://crw.nanxinkj.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fkg.iojbl.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rfe.iojbl.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wre.pycfn.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://upd.zhoulong.xyz

[I07] 忽略大小写与多行模式
来源：http://rle.tarul.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yvk.dashuyun.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kao.feifeiyinyue.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://stz.bbcook.cn

TS:   /error/gim
来源：http://zqv.snrcjt.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uma.daria6918.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xkw.yonumen.top

Ruby: s.scan(/error/i)
来源：http://pfn.wangdashe.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vyv.vqdsnc.cn

[I08] 贪婪与非贪婪匹配
来源：http://nxe.bjfxy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ilq.hysaishi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://laf.feifeiyinyue.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wpc.zdbjq.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mwt.xuetiantiany.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ssu.ctjpmb.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zbs.ehwqpu.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://eya.smart0.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cjw.daria6918.cn

================================================================================
来源：http://fmq.fzhhl.top

J. 日期与时间
来源：http://ndz.fzhhl.top

================================================================================
来源：http://pft.nwbrower.top

[J01] 获取当前时间
来源：http://gxz.jiagoushi.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ziz.yj20258888.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wyk.hnxiangtu.top

JS:   new Date();  Date.now()
来源：http://iib.nanxuanxn.top

TS:   new Date();  Date.now()
来源：http://tmn.guannengcc.top

Java: LocalDateTime.now();  Instant.now()
来源：http://tye.sweek.top

Go:   time.Now()
来源：http://bgs.aizwys.cn

Ruby: Time.now
来源：http://bum.ydjk.org.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jln.andypj.xyz

[J02] 格式化输出
来源：http://vmd.hywenlv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uxp.hnxiangtu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cvp.snrcjt.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fqz.xingfuxueyuan.xyz

TS:   d.toISOString()
来源：http://fdi.andypj.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vtu.xylfe.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cta.xinyue.icu

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ujo.ehwqpu.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sks.hywenlv.cn

[J03] 字符串解析为日期
来源：http://krw.chenzaomai.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kwt.hywenlv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://whk.hfpthk.cn

JS:   new Date("2024-01-02")
来源：http://orr.tian-w.cn

TS:   new Date("2024-01-02")
来源：http://mwx.jqgfzy.top

Java: LocalDate.parse("2024-01-02")
来源：http://irj.dashuyun.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gts.zdbjq.cn

Ruby: Date.parse("2024-01-02")
来源：http://iza.cqqwz.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ajg.zdbjq.cn

[J04] 时间戳与日期互转
来源：http://xpb.sufxvd.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ykk.dashuyun.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gza.hnxiangtu.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://smo.gogol.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ham.fanxiaobao.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wjl.yfazqb.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pcx.snrcjt.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vbt.cheryme.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qln.fengsongda.top

[J05] 时间加减（加 7 天）
来源：http://yzr.smart0.xyz

Py:   now + timedelta(days=7)
来源：http://bmb.hcnkem.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://qlo.sxryk.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kum.hywenlv.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qwl.chenjidiqi.icu

Java: LocalDate.now().plusDays(7)
来源：http://rbl.tianlin.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://osf.pycfn.com

Ruby: Time.now + 7 * 86400
来源：http://phv.zhengqikj.top

C#:   DateTime.Now.AddDays(7)
来源：http://rhi.zhengqikj.top

[J06] 计算两时间之差
来源：http://uin.yueranfly.top

Py:   (end - start).total_seconds()
来源：http://zrd.cheryme.top

PHP:  $end->diff($start)->days;
来源：http://iad.iojbl.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hrt.nanxinkj.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yct.ydjk.org.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lev.andypj.xyz

Go:   end.Sub(start).Hours()
来源：http://uzd.vehdjk.com

Ruby: end - start                 # 返回秒数
来源：http://lpi.andypj.xyz

C#:   (end - start).TotalSeconds
来源：http://dvl.mhx1999.top

[J07] 比较两个日期
来源：http://nik.nanxinkj.top

Py:   d1 < d2;  d1 == d2
来源：http://beh.yongpay.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pth.xinyue.icu

JS:   d1.getTime() < d2.getTime()
来源：http://bdo.sufxvd.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pkh.tarul.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hbm.xuetiantiany.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cuz.xylfe.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ffu.zycfv.cn

C#:   d1 < d2;  d1 == d2
来源：http://kqj.sweek.top

[J08] 提取年月日与星期
来源：http://clp.haohaochexian.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ptp.jyoumei.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ynb.snrcjt.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sjv.jyoumei.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://piq.tarul.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ohw.zhengqikj.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ivd.guannengcc.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wwe.wangdashe.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fdx.zhongyouzk.top

[J09] 时区处理
来源：http://ide.hnqzz.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mur.cheryme.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fma.zdbjq.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zfn.xinyue.icu

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dqp.chenjidiqi.icu

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ccw.haohaochexian.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qmw.vehdjk.com

Ruby: Time.now.getlocal("+08:00")
来源：http://ymc.wangdashe.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vzn.zhengqikj.top

[J10] 取今天 / 本月第一天
来源：http://dkw.fktsv.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fll.quarkkingdee.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mdd.ivvv.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lwe.yongpay.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lvl.hesvh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://stw.cashguo.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ddu.uphjek.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://laz.hammf.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://arj.0kj1m.cn

================================================================================
来源：http://vrk.sufxvd.cn

K. JSON 与序列化
来源：http://lgh.c1oappe.top

================================================================================
来源：http://iea.sjlbkw.cn

[K01] 对象转 JSON 字符串
来源：http://boc.yj20258888.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mcl.yonumen.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zdg.zhijiandao.cn

JS:   JSON.stringify(obj)
来源：http://rhi.sjlbkw.cn

TS:   JSON.stringify(obj)
来源：http://npp.hongshengwenyu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://omx.hongshengwenyu.top

Go:   json.Marshal(obj)
来源：http://gnu.yueranfly.top

Ruby: obj.to_json                                     // require "json"
来源：http://ntn.jqgfzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://fmg.shangyingyoupin.top

[K02] JSON 字符串转对象
来源：http://jgq.shangyingyoupin.top

Py:   json.loads(s)
来源：http://wwh.sysykeji.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jsc.yuanzhike.top

JS:   JSON.parse(s)
来源：http://kff.nwbrower.top

TS:   JSON.parse(s)
来源：http://lbo.birdmap.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pet.yongpay.top

Go:   json.Unmarshal(data, &v)
来源：http://tkg.yueranfly.top

Ruby: JSON.parse(s)
来源：http://wlc.wangdashe.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://emn.chenlongwang.top

[K03] JSON 美化输出（带缩进）
来源：http://itf.chenzaomai.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ndn.hfpthk.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rks.nanxuanxn.top

JS:   JSON.stringify(obj, null, 2)
来源：http://yfs.bbcook.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bga.vehdjk.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qwk.havefunace.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rws.aizwys.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zap.ywan-chungtsiang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bmn.xingfuxueyuan.xyz

[K04] 读取 JSON 文件
来源：http://iyv.yuxming.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lir.mhx1999.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jhe.gzhubu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tnk.guannengcc.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ila.ctjpmb.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://eql.xuanzx.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jte.quarkkingdee.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://gyn.hcnkem.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://iop.yvedp.cn

[K05] 深拷贝对象
来源：http://njq.zhaomingkeji.xyz

Py:   copy.deepcopy(obj)
来源：http://nmr.sysykeji.top

PHP:  unserialize(serialize($obj));
来源：http://mwx.fzhhl.top

JS:   structuredClone(obj)
来源：http://axu.yuanzhike.top

TS:   structuredClone(obj)
来源：http://fou.ywan-chungtsiang.top

Java: // 手写拷贝构造，或序列化往返
来源：http://acl.zhixingplan.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mcw.andypj.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ggu.yvedp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://prj.yueranfly.top

[K06] 解析 URL 查询串
来源：http://cnm.guannengcc.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://orw.ydjk.org.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ipt.ybcxt.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://itb.nanxuanxn.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hnj.chenjidiqi.icu

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cwp.sufxvd.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://adx.zhiwuduotai.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nbd.bbcook.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tyd.haohaochexian.top

[K07] 进制转换
来源：http://pvb.c1oappe.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ekn.dianchejie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dvk.sufxvd.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tfp.tarul.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gzp.sweek.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sua.zdqjudy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vuo.ydzc1.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vjw.zhengqikj.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mlg.xinyue.icu

[K08] 二进制序列化（非 JSON）
来源：http://grs.aizwys.cn

Py:   pickle.dumps(obj)
来源：http://plj.hammf.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mcf.jinqigfzy.top

JS:   v8.serialize(obj)        // Node
来源：http://cfj.zhongyouzk.top

TS:   v8.serialize(obj)        // Node
来源：http://suy.meibo888.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jja.shanyushiyangtech.top

Go:   encoding/gob
来源：http://ibx.tanke756.top

Ruby: Marshal.dump(obj)
来源：http://cay.xziqi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ycc.xziqi.cn

================================================================================
来源：http://tyi.shanyushiyangkeji.top

L. 网络请求
来源：http://smc.jinqigfzy.top

================================================================================
来源：http://hdk.chenzaomai.com

[L01] 发送 GET 请求
来源：http://kbv.ehwqpu.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ozl.52xcode.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lho.fanxiaobao.xyz

JS:   await fetch(url)
来源：http://mfc.xylfe.cn

TS:   await fetch(url)
来源：http://yio.zdqjudy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kzp.vehdjk.com

Go:   resp, err := http.Get(url)
来源：http://vwp.sweek.top

Ruby: Net::HTTP.get(URI(url))
来源：http://six.cdnleiting.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uha.ydzc1.top

[L02] 发送 POST JSON
来源：http://mmx.nwbrower.top

Py:   requests.post(url, json={"a": 1})
来源：http://stq.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qzo.tanke756.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jmw.hongshengwenyu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gbk.jqgfzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yjl.hammf.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yyh.fzhhl.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://joh.sweek.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bfu.birdmap.top


<!-- 参考信息 -->