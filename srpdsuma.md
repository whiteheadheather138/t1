代发 wailian999

TS:   console.assert(x > 0);
来源：http://iin.smart0.xyz

Java: assert x > 0 : "必须为正";
来源：http://uvc.zhijiandao.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mth.havefunace.top

Ruby: raise "必须为正" unless x > 0
来源：http://hgi.uphjek.com

C#:   Debug.Assert(x > 0);
来源：http://ziw.yj20258.top

[H08] 获取错误信息与堆栈
来源：http://ugh.hnxiangtu.top

Py:   str(e);  traceback.format_exc()
来源：http://jgj.andypj.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://eir.shangyingyoupin.top

JS:   e.message;  e.stack
来源：http://hjq.daxiang520.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ffh.cdnleiting.top

Java: e.getMessage();  e.printStackTrace()
来源：http://qwc.iojbl.cn

Go:   err.Error()
来源：http://yhp.andypj.xyz

Ruby: e.message;  e.backtrace
来源：http://ily.chenlongwang.top

C#:   e.Message;  e.StackTrace
来源：http://foz.dashuyun.cn

[H09] 带错误码的异常
来源：http://jnh.havefunace.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://obe.gzhubu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://tuz.dianchejie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://the.cashguo.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cfo.xylfe.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cub.cashguo.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ghl.cheryme.top

Ruby: raise MyError.new("fail", 500)
来源：http://fml.jinghuilouyu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://jrz.shuidangran.top

[H10] 资源自动释放
来源：http://buz.yj202588.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://pev.ctjpmb.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lro.jianghu66.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wam.daria6918.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qig.zycfv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dpv.pycfn.com

Go:   defer f.Close()
来源：http://wzs.zhiwuduotai.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jfr.gogol.net.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yru.sweek.top

================================================================================
来源：http://wip.fengsongda.top

I. 正则表达式
来源：http://ijr.sysykeji.top

================================================================================
来源：http://fzb.redwolf501.top

[I01] 判断是否匹配
来源：http://ynl.jinqigufen.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://eif.daria6918.cn

PHP:  preg_match('/\d+/', $s);
来源：http://lyc.jqgfzy.top

JS:   /\d+/.test(s)
来源：http://kcd.shanyushiyangtech.top

TS:   /\d+/.test(s)
来源：http://wee.pycfn.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://aow.hcnkem.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zfu.hysaishi.cn

Ruby: s.match?(/\d+/)
来源：http://kax.quarkkingdee.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sgv.gaohongyu789.top

[I02] 提取所有匹配
来源：http://arx.vehdjk.com

Py:   re.findall(r"\d+", s)
来源：http://xcn.chenzaomai.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ptq.svipenyu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hbl.yanxiufei.cn

TS:   s.match(/\d+/g)
来源：http://tcu.c1oappe.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wwl.zhoulong.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ono.pengpengdd.cyou

Ruby: s.scan(/\d+/)
来源：http://ati.nanxuanxn.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nyb.c1oappe.top

[I03] 提取捕获分组
来源：http://blp.zdbjq.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://aoq.jqgfzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://whj.xuetiantiany.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://akx.jinghuilouyu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qqy.tarul.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ctn.chenlongwang.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://eqg.pycfn.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vgp.xuetiantiany.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cxi.jinghuilouyu.cn

[I04] 正则替换
来源：http://avx.52xcode.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://pjk.c1oappe.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xyn.tanke756.top

JS:   s.replace(/\d+/g, "#")
来源：http://plv.sysykeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://gih.wangshuangyany.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xxw.nanxuanxn.top

Go:   re.ReplaceAllString(s, "#")
来源：http://sxw.mhx1999.top

Ruby: s.gsub(/\d+/, "#")
来源：http://sbk.birdmap.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xyo.smart0.xyz

[I05] 按正则拆分
来源：http://gkq.hnqzz.top

Py:   re.split(r"\s*,\s*", s)
来源：http://njp.jyoumei.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jhd.gzhubu.top

JS:   s.split(/\s*,\s*/)
来源：http://qku.hesvh.cn

TS:   s.split(/\s*,\s*/)
来源：http://axc.zhiwuduotai.top

Java: s.split("\\s*,\\s*")
来源：http://nov.chenlongwang.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xbo.ybcxt.top

Ruby: s.split(/\s*,\s*/)
来源：http://gep.pycfn.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ncq.xuetiantiany.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mgv.jinqigufen.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cuo.zycfv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yjx.52xcode.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hup.ppjwa.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vfl.vqdsnc.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yye.tian-w.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dli.yj20258.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ibb.quarkkingdee.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cvv.nwbrower.top

[I07] 忽略大小写与多行模式
来源：http://ffs.dianchejie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xtc.iojbl.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wiv.hongshengwenyu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ayd.pengpengdd.cyou

TS:   /error/gim
来源：http://ses.52xcode.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hqk.ywan-chungtsiang.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://obk.daria6918.cn

Ruby: s.scan(/error/i)
来源：http://kyb.ydzc1.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hre.jianghu66.top

[I08] 贪婪与非贪婪匹配
来源：http://etc.52xcode.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pax.jinqigfzy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rqs.dianchejie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://luw.yangfankeji.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qoo.jiagoushi.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ewj.hfpthk.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ghm.zhixingplan.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vxp.epnwcf.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kkj.xuanzx.com

================================================================================
来源：http://oae.yj20258.top

J. 日期与时间
来源：http://pun.vqdsnc.cn

================================================================================
来源：http://oju.hfpthk.cn

[J01] 获取当前时间
来源：http://lpi.bbcook.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://idm.xingfuxueyuan.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://iwj.chenlongwang.top

JS:   new Date();  Date.now()
来源：http://chs.bjfxy.top

TS:   new Date();  Date.now()
来源：http://ubw.cdnleiting.top

Java: LocalDateTime.now();  Instant.now()
来源：http://urf.xylfe.cn

Go:   time.Now()
来源：http://biy.guowangkeji.top

Ruby: Time.now
来源：http://oej.nanxinkj.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xgj.bbcook.cn

[J02] 格式化输出
来源：http://ndw.hysaishi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tux.cqqwz.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qwm.shzxlz.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qbg.haohaochexian.top

TS:   d.toISOString()
来源：http://ijm.ehwqpu.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pgu.smart0.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rgk.xuanzx.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qbb.tanke756.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dzu.hfpthk.cn

[J03] 字符串解析为日期
来源：http://ely.fzhhl.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hev.chenlongwang.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dxe.cqqwz.cn

JS:   new Date("2024-01-02")
来源：http://dnk.svipenyu.cn

TS:   new Date("2024-01-02")
来源：http://xvo.gotoacloud.top

Java: LocalDate.parse("2024-01-02")
来源：http://zeu.kuanghao11.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tnp.yj20258888.top

Ruby: Date.parse("2024-01-02")
来源：http://zwt.ydjk.org.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vek.yj202588.top

[J04] 时间戳与日期互转
来源：http://ruk.mhx1999.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://csh.yangfankeji.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://juq.shanyushiyangkeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lxi.fanxiaobao.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://saz.gzhubu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xiz.yonumen.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gjf.zdbjq.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lry.yongpay.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vzz.aibaodan.cn

[J05] 时间加减（加 7 天）
来源：http://ays.fktsv.cn

Py:   now + timedelta(days=7)
来源：http://kcl.sxryk.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ycv.aizwys.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uyk.sjlbkw.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vch.zhaomingkeji.xyz

Java: LocalDate.now().plusDays(7)
来源：http://qcp.zhongyouzk.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fur.zhongyouzk.top

Ruby: Time.now + 7 * 86400
来源：http://gts.gzhubu.top

C#:   DateTime.Now.AddDays(7)
来源：http://eom.sxryk.cn

[J06] 计算两时间之差
来源：http://cyr.fzhhl.top

Py:   (end - start).total_seconds()
来源：http://kqf.hfpthk.cn

PHP:  $end->diff($start)->days;
来源：http://svg.shangyingyoupin.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://arr.tian-w.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lmc.gzhubu.top

Java: Duration.between(start, end).toSeconds()
来源：http://kez.cucudq.cn

Go:   end.Sub(start).Hours()
来源：http://znp.redwolf501.top

Ruby: end - start                 # 返回秒数
来源：http://rvs.gzhubu.top

C#:   (end - start).TotalSeconds
来源：http://awi.svipenyu.cn

[J07] 比较两个日期
来源：http://asq.ctjpmb.com

Py:   d1 < d2;  d1 == d2
来源：http://mnz.ppjwa.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lgp.dashuyun.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ihf.yfazqb.com

TS:   d1.getTime() < d2.getTime()
来源：http://ygp.hywenlv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mru.redwolf501.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zia.iojbl.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yhn.0kj1m.cn

C#:   d1 < d2;  d1 == d2
来源：http://nbf.sysykeji.top

[J08] 提取年月日与星期
来源：http://pzy.redwolf501.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ciy.jlsjyb.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ihe.tanke756.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qba.fzhhl.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://awd.guowangkeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://oqk.cdnleiting.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qcd.yangfankeji.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tic.0kj1m.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jfz.gzhubu.top

[J09] 时区处理
来源：http://ibd.ybcxt.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fhr.feifeiyinyue.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cpz.yanxiufei.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mmq.chenlongwang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tqu.cheryme.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zvz.yongpay.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qch.bjfxy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ova.fengsongda.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pfn.bjfxy.top

[J10] 取今天 / 本月第一天
来源：http://cbd.yuxming.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wwv.zhaomingkeji.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qex.xingfuxueyuan.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jbe.hammf.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mwp.tianlin.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://irs.iojbl.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wct.jinyuanbaomall.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ohg.uphjek.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xvv.cashguo.top

================================================================================
来源：http://voh.hywenlv.cn

K. JSON 与序列化
来源：http://vny.jinghuilouyu.cn

================================================================================
来源：http://mzp.yj20258888.top

[K01] 对象转 JSON 字符串
来源：http://dak.kuanghao11.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vft.sufxvd.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jun.meibo888.top

JS:   JSON.stringify(obj)
来源：http://soe.gogol.net.cn

TS:   JSON.stringify(obj)
来源：http://wem.fzhhl.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kkw.tianlin.xyz

Go:   json.Marshal(obj)
来源：http://fyr.yj20258888.top

Ruby: obj.to_json                                     // require "json"
来源：http://ywx.quarkkingdee.top

C#:   JsonSerializer.Serialize(obj)
来源：http://xlb.guowangkeji.top

[K02] JSON 字符串转对象
来源：http://xim.chenjidiqi.icu

Py:   json.loads(s)
来源：http://fqa.zhongyouzk.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://eky.52xcode.cn

JS:   JSON.parse(s)
来源：http://rdu.shanyushiyangkeji.top

TS:   JSON.parse(s)
来源：http://htj.yongpay.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://whz.hfpthk.cn

Go:   json.Unmarshal(data, &v)
来源：http://dky.jqgfzy.top

Ruby: JSON.parse(s)
来源：http://uhk.zhongyouzk.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lpe.gotoacloud.top

[K03] JSON 美化输出（带缩进）
来源：http://mjo.yuxming.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jep.chenzaomai.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vry.shanyushiyangtech.top

JS:   JSON.stringify(obj, null, 2)
来源：http://kqu.feifeiyinyue.top

TS:   JSON.stringify(obj, null, 2)
来源：http://hai.jyoumei.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hkm.wangdashe.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jqp.hywenlv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://lry.epnwcf.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rvu.meibo888.top

[K04] 读取 JSON 文件
来源：http://kha.shanyushiyangkeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cxz.bjfxy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jrx.yueranfly.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://atq.xylfe.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rpo.xuanzx.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ieo.0kj1m.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rac.xingfuxueyuan.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://gaz.jinqigufen.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kzp.xziqi.cn

[K05] 深拷贝对象
来源：http://jvt.pycfn.com

Py:   copy.deepcopy(obj)
来源：http://qvh.hcnkem.com

PHP:  unserialize(serialize($obj));
来源：http://jbq.shzxlz.cn

JS:   structuredClone(obj)
来源：http://hqg.redwolf501.top

TS:   structuredClone(obj)
来源：http://ypd.gzhubu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://upe.cucudq.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qpy.cheryme.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rwm.iojbl.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xoj.cdnleiting.top

[K06] 解析 URL 查询串
来源：http://ykx.sysykeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gjq.zhaomingkeji.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rfd.iojbl.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sni.hcnkem.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://izf.zhongyouzk.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://edt.uphjek.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://rxw.jqgufenzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wuz.tanke756.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lcb.fehbvm.com

[K07] 进制转换
来源：http://tzu.yanxiufei.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lmj.sxryk.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ukz.fktsv.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kmc.guannengcc.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wpp.aizwys.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://erq.jinghuilouyu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xia.zdbjq.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://azt.tarul.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ghf.havefunace.top

[K08] 二进制序列化（非 JSON）
来源：http://zoq.gzhubu.top

Py:   pickle.dumps(obj)
来源：http://xbv.daria6918.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wos.zycfv.cn

JS:   v8.serialize(obj)        // Node
来源：http://twx.tianlin.xyz

TS:   v8.serialize(obj)        // Node
来源：http://tvr.zhixingplan.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qcy.yonumen.top

Go:   encoding/gob
来源：http://lfl.bjfxy.top

Ruby: Marshal.dump(obj)
来源：http://cem.shanyushiyangkeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sqk.feifeiyinyue.top

================================================================================
来源：http://jzx.hammf.cn

L. 网络请求
来源：http://qpu.yj20258888.top

================================================================================
来源：http://wze.jlsjyb.cn

[L01] 发送 GET 请求
来源：http://csq.0kj1m.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ioh.zdbjq.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xhw.daxiang520.top

JS:   await fetch(url)
来源：http://poe.dianchejie.cn

TS:   await fetch(url)
来源：http://kgs.cucudq.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jae.shanyushiyangkeji.top

Go:   resp, err := http.Get(url)
来源：http://lrg.fehbvm.com

Ruby: Net::HTTP.get(URI(url))
来源：http://fbm.tianlin.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vdt.cucudq.cn

[L02] 发送 POST JSON
来源：http://eoe.shanyushiyangtech.top

Py:   requests.post(url, json={"a": 1})
来源：http://tyy.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dky.epnwcf.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zsm.nwbrower.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rtx.tianlin.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zyt.316326.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cue.hnxiangtu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fho.zhixingplan.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pdg.zhiwuduotai.top

[L03] 设置自定义请求头
来源：http://ckx.daria6918.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://urm.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ijp.yj20258888.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fzm.chenjidiqi.icu


<!-- 参考信息 -->