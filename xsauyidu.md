代发 wailian999

TS:   console.assert(x > 0);
来源：http://qfl.nanxinkj.top

Java: assert x > 0 : "必须为正";
来源：http://wty.yueranfly.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rap.fanxiaobao.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://hjk.hesvh.cn

C#:   Debug.Assert(x > 0);
来源：http://fxs.cqqwz.cn

[H08] 获取错误信息与堆栈
来源：http://fwg.dianchejie.cn

Py:   str(e);  traceback.format_exc()
来源：http://sat.cheryme.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cbc.hesvh.cn

JS:   e.message;  e.stack
来源：http://ysq.wangdashe.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://sxz.jinqigufen.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ihp.xinyue.icu

Go:   err.Error()
来源：http://uxm.bbcook.cn

Ruby: e.message;  e.backtrace
来源：http://tto.gotoacloud.top

C#:   e.Message;  e.StackTrace
来源：http://euz.jyoumei.cn

[H09] 带错误码的异常
来源：http://cum.sjlbkw.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gbk.ydjk.org.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mso.xziqi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lwp.nanxinkj.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gyk.yj20258888.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qdj.tanke756.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zsr.hongshengwenyu.top

Ruby: raise MyError.new("fail", 500)
来源：http://lmq.tianlin.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://puy.epnwcf.com

[H10] 资源自动释放
来源：http://aes.9152youxi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xwn.shangyingyoupin.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rsh.yuanzhike.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nbf.fanxiaobao.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kfx.jianghu66.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hvk.gaohongyu789.top

Go:   defer f.Close()
来源：http://loy.snrcjt.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jdp.zdbjq.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pks.mhx1999.top

================================================================================
来源：http://htl.sweek.top

I. 正则表达式
来源：http://zvh.jinqigufen.top

================================================================================
来源：http://wie.cashguo.top

[I01] 判断是否匹配
来源：http://ecb.gotoacloud.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cfk.hysaishi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zdo.jiagoushi.top

JS:   /\d+/.test(s)
来源：http://xok.zycfv.cn

TS:   /\d+/.test(s)
来源：http://sgg.ppjwa.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gvb.ehwqpu.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pzi.tarul.cn

Ruby: s.match?(/\d+/)
来源：http://tae.jinyuanbaomall.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://upj.nanxuanxn.top

[I02] 提取所有匹配
来源：http://jqq.pycfn.com

Py:   re.findall(r"\d+", s)
来源：http://ifi.pycfn.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vzz.yj20258888.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qzh.jqgufenzy.top

TS:   s.match(/\d+/g)
来源：http://xgz.redwolf501.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://eaa.jinqigufen.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xus.fanxiaobao.xyz

Ruby: s.scan(/\d+/)
来源：http://yqc.shzxlz.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://klb.sufxvd.cn

[I03] 提取捕获分组
来源：http://mee.ywan-chungtsiang.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zky.hysaishi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ifn.quarkkingdee.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vjj.yj20258888.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mlg.yangfankeji.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zis.fengsongda.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dbg.nanxinkj.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ttk.hongshengwenyu.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cla.shanyushiyangkeji.top

[I04] 正则替换
来源：http://yxt.ivvv.top

Py:   re.sub(r"\d+", "#", s)
来源：http://fnj.mhx1999.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nib.cdnleiting.top

JS:   s.replace(/\d+/g, "#")
来源：http://syt.tanke756.top

TS:   s.replace(/\d+/g, "#")
来源：http://bxy.smart0.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://nju.xinyue.icu

Go:   re.ReplaceAllString(s, "#")
来源：http://hip.jyoumei.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://bta.xuetiantiany.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nyx.cdnleiting.top

[I05] 按正则拆分
来源：http://ezb.smart0.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://sag.cqqwz.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lwh.yonumen.top

JS:   s.split(/\s*,\s*/)
来源：http://qoh.gaohongyu789.top

TS:   s.split(/\s*,\s*/)
来源：http://qtv.xinyue.icu

Java: s.split("\\s*,\\s*")
来源：http://dnc.hysaishi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bkx.pycfn.com

Ruby: s.split(/\s*,\s*/)
来源：http://kxc.jinyuanbaomall.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://naw.mhx1999.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rkq.yfazqb.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wsq.nwbrower.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://afz.daria6918.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://esh.zhijiandao.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jih.316326.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://skk.jqgfzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ebf.chenlongwang.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ytn.zhongyouzk.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jsv.uphjek.com

[I07] 忽略大小写与多行模式
来源：http://uls.kuanghao11.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mtk.smart0.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cbr.sufxvd.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xzf.316326.xyz

TS:   /error/gim
来源：http://oyj.jiagoushi.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ejl.ybcxt.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dcd.xuanzx.com

Ruby: s.scan(/error/i)
来源：http://qbw.feifeiyinyue.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pjz.aizwys.cn

[I08] 贪婪与非贪婪匹配
来源：http://vvu.yvedp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qrq.aibaodan.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fnt.snrcjt.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gwp.tian-w.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://owd.hammf.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://iui.sufxvd.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ppu.iojbl.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ors.yfazqb.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hjm.shanyushiyangtech.top

================================================================================
来源：http://vzw.xziqi.cn

J. 日期与时间
来源：http://yct.fzhhl.top

================================================================================
来源：http://gdt.cheryme.top

[J01] 获取当前时间
来源：http://ivk.hammf.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://muw.aizwys.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sjo.ydjk.org.cn

JS:   new Date();  Date.now()
来源：http://ylf.birdmap.top

TS:   new Date();  Date.now()
来源：http://zxi.yfazqb.com

Java: LocalDateTime.now();  Instant.now()
来源：http://fli.chenlongwang.top

Go:   time.Now()
来源：http://paf.pycfn.com

Ruby: Time.now
来源：http://enw.jianghu66.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lqf.sufxvd.cn

[J02] 格式化输出
来源：http://zah.bjfxy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pyi.c1oappe.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wwj.shangyingyoupin.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lqk.vehdjk.com

TS:   d.toISOString()
来源：http://udd.jlsjyb.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qla.gzhubu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xxt.tanke756.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rzw.kuanghao11.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://eeo.dashuyun.cn

[J03] 字符串解析为日期
来源：http://sjm.ydjk.org.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zjn.gzhubu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://srt.tarul.cn

JS:   new Date("2024-01-02")
来源：http://atz.9152youxi.cn

TS:   new Date("2024-01-02")
来源：http://vbg.jinqigufen.top

Java: LocalDate.parse("2024-01-02")
来源：http://tjq.zhoulong.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ozc.ehwqpu.com

Ruby: Date.parse("2024-01-02")
来源：http://roe.jqgfzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qcp.xuanzx.com

[J04] 时间戳与日期互转
来源：http://bps.0kj1m.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://oix.yonumen.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gjv.yangfankeji.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jdw.ywan-chungtsiang.top

TS:   Math.floor(Date.now() / 1000)
来源：http://uua.jinqigfzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://onn.shzxlz.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yox.sweek.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tgi.yuxming.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fhr.jinyuanbaomall.cn

[J05] 时间加减（加 7 天）
来源：http://lnf.chenzaomai.com

Py:   now + timedelta(days=7)
来源：http://czw.jiagoushi.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://wzf.cdnleiting.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wsu.iojbl.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mdh.sufxvd.cn

Java: LocalDate.now().plusDays(7)
来源：http://fnv.52xcode.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dxz.yuxming.cn

Ruby: Time.now + 7 * 86400
来源：http://wgk.haohaochexian.top

C#:   DateTime.Now.AddDays(7)
来源：http://pjz.shangyingyoupin.top

[J06] 计算两时间之差
来源：http://nvv.cashguo.top

Py:   (end - start).total_seconds()
来源：http://yec.zhijiandao.cn

PHP:  $end->diff($start)->days;
来源：http://qzz.zhongyouzk.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rux.sxryk.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ywg.tian-w.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gvv.hywenlv.cn

Go:   end.Sub(start).Hours()
来源：http://xgx.fzhhl.top

Ruby: end - start                 # 返回秒数
来源：http://opr.jinghuilouyu.cn

C#:   (end - start).TotalSeconds
来源：http://qpq.mhx1999.top

[J07] 比较两个日期
来源：http://lhl.fanxiaobao.xyz

Py:   d1 < d2;  d1 == d2
来源：http://yjm.chenzaomai.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jlh.fengsongda.top

JS:   d1.getTime() < d2.getTime()
来源：http://fdw.kuanghao11.cn

TS:   d1.getTime() < d2.getTime()
来源：http://heq.daria6918.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://txl.cashguo.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bty.cdnleiting.top

Ruby: d1 < d2;  d1 == d2
来源：http://jgl.quarkkingdee.top

C#:   d1 < d2;  d1 == d2
来源：http://kzg.yfazqb.com

[J08] 提取年月日与星期
来源：http://maf.uphjek.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bxm.zhoulong.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qgi.jqgufenzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zuy.shanyushiyangkeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wsw.yuxming.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zci.sufxvd.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gwz.sysykeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qan.jqgufenzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rhw.daxiang520.top

[J09] 时区处理
来源：http://yln.ctjpmb.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ltw.zhixingplan.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://poh.shuidangran.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bnv.wangdashe.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ckp.dianchejie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xpw.nwbrower.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bwr.shanyushiyangkeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://mro.bjfxy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://odm.andypj.xyz

[J10] 取今天 / 本月第一天
来源：http://krw.aizwys.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://uiq.cqqwz.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wms.ydzc1.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ajp.fktsv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fwt.sweek.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qeo.jinqigufen.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://omh.guowangkeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pno.yonumen.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wnh.yj202588.top

================================================================================
来源：http://vof.tianlin.xyz

K. JSON 与序列化
来源：http://ljn.c1oappe.top

================================================================================
来源：http://rpn.havefunace.top

[K01] 对象转 JSON 字符串
来源：http://ano.shzxlz.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wuc.yonumen.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pin.shangyingyoupin.top

JS:   JSON.stringify(obj)
来源：http://sbh.yvedp.cn

TS:   JSON.stringify(obj)
来源：http://wcz.fktsv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vvh.guannengcc.top

Go:   json.Marshal(obj)
来源：http://tug.nwbrower.top

Ruby: obj.to_json                                     // require "json"
来源：http://vhk.jqgufenzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://bgf.yvedp.cn

[K02] JSON 字符串转对象
来源：http://bhb.vqdsnc.cn

Py:   json.loads(s)
来源：http://oma.fanxiaobao.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fdu.kuanghao11.cn

JS:   JSON.parse(s)
来源：http://trx.xylfe.cn

TS:   JSON.parse(s)
来源：http://bfp.zhixingplan.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rho.yuanzhike.top

Go:   json.Unmarshal(data, &v)
来源：http://sua.zhengqikj.top

Ruby: JSON.parse(s)
来源：http://asi.yj20258888.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://msz.iojbl.cn

[K03] JSON 美化输出（带缩进）
来源：http://say.zhengqikj.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xkf.xziqi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hzt.nanxinkj.top

JS:   JSON.stringify(obj, null, 2)
来源：http://sfa.xziqi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ygx.gaohongyu789.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lpk.gotoacloud.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://crn.guannengcc.top

Ruby: JSON.pretty_generate(obj)
来源：http://kbf.yangfankeji.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bof.jinqigfzy.top

[K04] 读取 JSON 文件
来源：http://tvw.pycfn.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pyk.dashuyun.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vvy.shanyushiyangtech.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hdw.xziqi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hje.xylfe.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zhw.xuanzx.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wzt.sweek.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://vaq.redwolf501.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lxh.cashguo.top

[K05] 深拷贝对象
来源：http://jqj.dashuyun.cn

Py:   copy.deepcopy(obj)
来源：http://tpe.feifeiyinyue.top

PHP:  unserialize(serialize($obj));
来源：http://ggs.sweek.top

JS:   structuredClone(obj)
来源：http://ejd.52xcode.cn

TS:   structuredClone(obj)
来源：http://awd.gotoacloud.top

Java: // 手写拷贝构造，或序列化往返
来源：http://zth.yongpay.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://glv.cqqwz.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yqf.epnwcf.com

C#:   // 序列化往返，或自定义 Clone
来源：http://kwz.ydjk.org.cn

[K06] 解析 URL 查询串
来源：http://aaa.fzhhl.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nuj.iojbl.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://oob.zdbjq.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://giq.vqdsnc.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uvm.fanxiaobao.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vfn.zhoulong.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://vej.yj20258888.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ajb.shanyushiyangtech.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fug.vehdjk.com

[K07] 进制转换
来源：http://dup.snrcjt.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lky.yongpay.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vfh.jinghuilouyu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pcv.dashuyun.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://csl.sufxvd.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uwp.jinghuilouyu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dvn.sxryk.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cxk.yj20258888.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rzs.epnwcf.com

[K08] 二进制序列化（非 JSON）
来源：http://ioh.chenzaomai.com

Py:   pickle.dumps(obj)
来源：http://dur.jinyuanbaomall.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zyd.mhx1999.top

JS:   v8.serialize(obj)        // Node
来源：http://jle.zhijiandao.cn

TS:   v8.serialize(obj)        // Node
来源：http://niq.tanke756.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hgj.redwolf501.top

Go:   encoding/gob
来源：http://fkz.hysaishi.cn

Ruby: Marshal.dump(obj)
来源：http://vkq.redwolf501.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://emw.dashuyun.cn

================================================================================
来源：http://pqz.zhixingplan.top

L. 网络请求
来源：http://uzj.xuanzx.com

================================================================================
来源：http://ttz.shuidangran.top

[L01] 发送 GET 请求
来源：http://kao.tanke756.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ymu.vehdjk.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xib.nanxuanxn.top

JS:   await fetch(url)
来源：http://skq.fanxiaobao.xyz

TS:   await fetch(url)
来源：http://fmq.zdbjq.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mqp.hammf.cn

Go:   resp, err := http.Get(url)
来源：http://vdf.nwbrower.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ndc.yfazqb.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kil.shzxlz.cn

[L02] 发送 POST JSON
来源：http://xis.shanyushiyangtech.top

Py:   requests.post(url, json={"a": 1})
来源：http://vco.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ekv.wangshuangyany.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://laz.zhongyouzk.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iat.yj20258888.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xip.jqgfzy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qci.uphjek.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://khp.redwolf501.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://otm.jiagoushi.top

[L03] 设置自定义请求头
来源：http://gqh.daxiang520.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rjt.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xhr.pycfn.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://svl.xinyue.icu


<!-- 参考信息 -->