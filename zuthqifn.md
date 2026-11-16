代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://zoe.ctjpmb.com

[H08] 获取错误信息与堆栈
来源：http://noh.fanxiaobao.xyz

Py:   str(e);  traceback.format_exc()
来源：http://tfo.bjfxy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xoi.ywan-chungtsiang.top

JS:   e.message;  e.stack
来源：http://jgg.xuanzx.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://gmb.fengsongda.top

Java: e.getMessage();  e.printStackTrace()
来源：http://kgn.wangdashe.top

Go:   err.Error()
来源：http://tmx.zhiwuduotai.top

Ruby: e.message;  e.backtrace
来源：http://vrg.xuetiantiany.cn

C#:   e.Message;  e.StackTrace
来源：http://scs.yj20258888.top

[H09] 带错误码的异常
来源：http://fpt.c1oappe.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://oor.ehwqpu.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://ptg.jinqigfzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://khe.hnqzz.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://eak.chenlongwang.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hun.yangfankeji.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://iwz.redwolf501.top

Ruby: raise MyError.new("fail", 500)
来源：http://saj.jinqigufen.top

C#:   // 自定义异常类中加 Code 属性
来源：http://blj.0kj1m.cn

[H10] 资源自动释放
来源：http://tth.yvedp.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lfq.meibo888.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zfg.xinyue.icu

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zer.hfpthk.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://eev.ctjpmb.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://roy.feifeiyinyue.top

Go:   defer f.Close()
来源：http://guv.zdqjudy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zvv.yanxiufei.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cso.hongshengwenyu.top

================================================================================
来源：http://bxr.nanxuanxn.top

I. 正则表达式
来源：http://pgu.andypj.xyz

================================================================================
来源：http://zzi.quarkkingdee.top

[I01] 判断是否匹配
来源：http://ukk.ivvv.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://acl.ybcxt.top

PHP:  preg_match('/\d+/', $s);
来源：http://llf.dianchejie.cn

JS:   /\d+/.test(s)
来源：http://mrk.sweek.top

TS:   /\d+/.test(s)
来源：http://cyz.jianghu66.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://npt.yonumen.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ovu.ydjk.org.cn

Ruby: s.match?(/\d+/)
来源：http://blp.yueranfly.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ifx.nwbrower.top

[I02] 提取所有匹配
来源：http://zpf.dashuyun.cn

Py:   re.findall(r"\d+", s)
来源：http://ekx.shuidangran.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yuh.sufxvd.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://asq.yj202588.top

TS:   s.match(/\d+/g)
来源：http://hne.pycfn.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://psw.redwolf501.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://byf.uphjek.com

Ruby: s.scan(/\d+/)
来源：http://rby.bbcook.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://thj.ehwqpu.com

[I03] 提取捕获分组
来源：http://kve.ybcxt.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rqd.tianlin.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fyn.hnqzz.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ula.kuanghao11.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vkk.hfpthk.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wxw.chenzaomai.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bhf.sjlbkw.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rip.aizwys.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qke.daria6918.cn

[I04] 正则替换
来源：http://hmu.kuanghao11.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ptg.xinyue.icu

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wzl.xylfe.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ebx.hysaishi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ujk.gaohongyu789.top

Java: s.replaceAll("\\d+", "#")
来源：http://rat.yj202588.top

Go:   re.ReplaceAllString(s, "#")
来源：http://vxn.tianlin.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://vbk.nanxinkj.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fzn.meibo888.top

[I05] 按正则拆分
来源：http://bpn.xuanzx.com

Py:   re.split(r"\s*,\s*", s)
来源：http://enh.sxryk.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dmw.dashuyun.cn

JS:   s.split(/\s*,\s*/)
来源：http://krw.nanxinkj.top

TS:   s.split(/\s*,\s*/)
来源：http://dhq.nanxinkj.top

Java: s.split("\\s*,\\s*")
来源：http://efy.52xcode.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xgo.ydjk.org.cn

Ruby: s.split(/\s*,\s*/)
来源：http://tsq.yonumen.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xul.jqgfzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jkj.meibo888.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vmk.pengpengdd.cyou

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hks.xziqi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ibp.shanyushiyangkeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bez.nwbrower.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ecz.bjfxy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jqq.bjfxy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gpd.snrcjt.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://owj.chenzaomai.com

[I07] 忽略大小写与多行模式
来源：http://pls.smart0.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mfe.yangfankeji.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fqm.gzhubu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://apz.yangfankeji.com

TS:   /error/gim
来源：http://rfx.zdbjq.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jdv.nanxinkj.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dfz.bjfxy.top

Ruby: s.scan(/error/i)
来源：http://svs.shanyushiyangtech.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ooa.cqqwz.cn

[I08] 贪婪与非贪婪匹配
来源：http://kar.jinghuilouyu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qiq.dashuyun.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jtj.gaohongyu789.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://iwb.zycfv.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ied.xingfuxueyuan.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://fbh.ppjwa.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sfp.ctjpmb.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lzm.wangdashe.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wte.gaohongyu789.top

================================================================================
来源：http://dly.wangdashe.top

J. 日期与时间
来源：http://tzf.nwbrower.top

================================================================================
来源：http://eap.sjlbkw.cn

[J01] 获取当前时间
来源：http://brd.iojbl.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://uxm.sjlbkw.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://msh.gaohongyu789.top

JS:   new Date();  Date.now()
来源：http://yaf.vqdsnc.cn

TS:   new Date();  Date.now()
来源：http://jmi.yuanzhike.top

Java: LocalDateTime.now();  Instant.now()
来源：http://uez.uphjek.com

Go:   time.Now()
来源：http://gxs.tian-w.cn

Ruby: Time.now
来源：http://isw.cqqwz.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vkl.hammf.cn

[J02] 格式化输出
来源：http://owe.jiagoushi.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eof.cdnleiting.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xty.zhixingplan.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xzm.shuidangran.top

TS:   d.toISOString()
来源：http://zty.sufxvd.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cke.zhongyouzk.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rda.hcnkem.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qod.fzhhl.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jvc.fehbvm.com

[J03] 字符串解析为日期
来源：http://lnh.redwolf501.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hej.316326.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bqt.andypj.xyz

JS:   new Date("2024-01-02")
来源：http://qfu.xingfuxueyuan.xyz

TS:   new Date("2024-01-02")
来源：http://tqs.jlsjyb.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jfe.daria6918.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://leo.hysaishi.cn

Ruby: Date.parse("2024-01-02")
来源：http://bhr.jlsjyb.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://eeq.tanke756.top

[J04] 时间戳与日期互转
来源：http://gwt.gotoacloud.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://szu.cheryme.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qzw.jinghuilouyu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qeq.hnqzz.top

TS:   Math.floor(Date.now() / 1000)
来源：http://pdq.ppjwa.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://aaa.yueranfly.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yfu.zhaomingkeji.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wrw.yanxiufei.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lgp.wangshuangyany.cn

[J05] 时间加减（加 7 天）
来源：http://ssu.hfpthk.cn

Py:   now + timedelta(days=7)
来源：http://okv.zycfv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://huq.jinqigufen.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gfr.yj20258.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qwe.zhengqikj.top

Java: LocalDate.now().plusDays(7)
来源：http://nhc.guannengcc.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uws.snrcjt.cn

Ruby: Time.now + 7 * 86400
来源：http://slc.bjfxy.top

C#:   DateTime.Now.AddDays(7)
来源：http://lld.wangshuangyany.cn

[J06] 计算两时间之差
来源：http://tll.feifeiyinyue.top

Py:   (end - start).total_seconds()
来源：http://rrg.havefunace.top

PHP:  $end->diff($start)->days;
来源：http://exu.sysykeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ryn.kuanghao11.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hoy.jqgufenzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://ojf.pycfn.com

Go:   end.Sub(start).Hours()
来源：http://fyt.quarkkingdee.top

Ruby: end - start                 # 返回秒数
来源：http://tjd.cdnleiting.top

C#:   (end - start).TotalSeconds
来源：http://syq.c1oappe.top

[J07] 比较两个日期
来源：http://mjm.mhx1999.top

Py:   d1 < d2;  d1 == d2
来源：http://bxi.jinqigufen.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nac.yvedp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://aks.hnxiangtu.top

TS:   d1.getTime() < d2.getTime()
来源：http://qst.yangfankeji.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://iex.cdnleiting.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qhm.smart0.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://ykv.jianghu66.top

C#:   d1 < d2;  d1 == d2
来源：http://svr.jinqigfzy.top

[J08] 提取年月日与星期
来源：http://lxy.zycfv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vqf.gzhubu.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sqj.chenlongwang.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hja.ppjwa.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ovs.svipenyu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qna.xylfe.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kew.shzxlz.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://drv.hnqzz.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zjt.pengpengdd.cyou

[J09] 时区处理
来源：http://zfa.gotoacloud.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kib.ehwqpu.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nud.daria6918.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ywm.shanyushiyangtech.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zky.gotoacloud.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ajp.yj202588.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bzt.fehbvm.com

Ruby: Time.now.getlocal("+08:00")
来源：http://vuw.sjlbkw.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sbt.yongpay.top

[J10] 取今天 / 本月第一天
来源：http://naa.nanxinkj.top

Py:   date.today();  date.today().replace(day=1)
来源：http://mgc.quarkkingdee.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://drf.ctjpmb.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vra.jinqigfzy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cig.vqdsnc.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bxt.shuidangran.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lec.hfpthk.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ysz.yongpay.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xdq.havefunace.top

================================================================================
来源：http://cmi.316326.xyz

K. JSON 与序列化
来源：http://eod.wangdashe.top

================================================================================
来源：http://sgu.dianchejie.cn

[K01] 对象转 JSON 字符串
来源：http://ggb.0kj1m.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lcw.yuanzhike.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zno.fktsv.cn

JS:   JSON.stringify(obj)
来源：http://ogq.jqgufenzy.top

TS:   JSON.stringify(obj)
来源：http://ewv.xuetiantiany.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cmo.xuanzx.com

Go:   json.Marshal(obj)
来源：http://nil.pycfn.com

Ruby: obj.to_json                                     // require "json"
来源：http://cmq.fzhhl.top

C#:   JsonSerializer.Serialize(obj)
来源：http://kfp.xinyue.icu

[K02] JSON 字符串转对象
来源：http://jde.nanxuanxn.top

Py:   json.loads(s)
来源：http://erj.tianlin.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cwn.jinghuilouyu.cn

JS:   JSON.parse(s)
来源：http://qdu.yonumen.top

TS:   JSON.parse(s)
来源：http://jpf.shangyingyoupin.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wvk.jianghu66.top

Go:   json.Unmarshal(data, &v)
来源：http://nyg.xingfuxueyuan.xyz

Ruby: JSON.parse(s)
来源：http://sld.svipenyu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://apw.ydjk.org.cn

[K03] JSON 美化输出（带缩进）
来源：http://nel.birdmap.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://djw.ydjk.org.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kbc.jlsjyb.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://brx.zdbjq.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zls.redwolf501.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uzu.ctjpmb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://isi.tian-w.cn

Ruby: JSON.pretty_generate(obj)
来源：http://aye.aibaodan.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://anb.wangdashe.top

[K04] 读取 JSON 文件
来源：http://xhb.zhiwuduotai.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jxl.yongpay.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tsj.fengsongda.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fhp.cashguo.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iin.yanxiufei.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mmg.sjlbkw.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ogx.chenlongwang.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://gxr.zycfv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kek.gogol.net.cn

[K05] 深拷贝对象
来源：http://phf.chenzaomai.com

Py:   copy.deepcopy(obj)
来源：http://yzf.pengpengdd.cyou

PHP:  unserialize(serialize($obj));
来源：http://kwq.smart0.xyz

JS:   structuredClone(obj)
来源：http://pqm.316326.xyz

TS:   structuredClone(obj)
来源：http://hij.52xcode.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gtu.wangshuangyany.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mud.fehbvm.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ylz.hysaishi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fxj.hfpthk.cn

[K06] 解析 URL 查询串
来源：http://njp.tarul.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ool.cheryme.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://exb.ehwqpu.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nes.epnwcf.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iva.jqgfzy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ric.hnqzz.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ysw.ybcxt.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bby.nwbrower.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://djv.chenjidiqi.icu

[K07] 进制转换
来源：http://trk.aibaodan.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://htn.hywenlv.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://idq.zhiwuduotai.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kvt.sysykeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://upf.sxryk.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bhz.sysykeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vjo.52xcode.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zhe.tianlin.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://njp.iojbl.cn

[K08] 二进制序列化（非 JSON）
来源：http://svd.hysaishi.cn

Py:   pickle.dumps(obj)
来源：http://jak.shanyushiyangkeji.top

PHP:  serialize($obj);  unserialize($s);
来源：http://sgd.chenzaomai.com

JS:   v8.serialize(obj)        // Node
来源：http://cou.wangdashe.top

TS:   v8.serialize(obj)        // Node
来源：http://ayd.jyoumei.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cnx.jinqigufen.top

Go:   encoding/gob
来源：http://qkr.cashguo.top

Ruby: Marshal.dump(obj)
来源：http://zvo.yuxming.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qsx.xingfuxueyuan.xyz

================================================================================
来源：http://acd.yanxiufei.cn

L. 网络请求
来源：http://zqe.yj20258888.top

================================================================================
来源：http://gku.zhiwuduotai.top

[L01] 发送 GET 请求
来源：http://jjv.zhixingplan.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wih.xuanzx.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://syf.hongshengwenyu.top

JS:   await fetch(url)
来源：http://kih.shuidangran.top

TS:   await fetch(url)
来源：http://vli.yj202588.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://caf.hcnkem.com

Go:   resp, err := http.Get(url)
来源：http://akm.shzxlz.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://oqh.jyoumei.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sos.vehdjk.com

[L02] 发送 POST JSON
来源：http://yrm.hfpthk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nqr.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ure.hnxiangtu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vpt.gaohongyu789.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dni.jqgfzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mqm.yangfankeji.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bmt.iojbl.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xvx.guannengcc.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dzo.fanxiaobao.xyz

[L03] 设置自定义请求头
来源：http://wzh.tian-w.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rqm.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wmc.hesvh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mdm.0kj1m.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hut.ybcxt.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pki.sjlbkw.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jea.hysaishi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://oho.jqgufenzy.top


<!-- 参考信息 -->