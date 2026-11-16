代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://rnp.hfpthk.cn

[H08] 获取错误信息与堆栈
来源：http://eeg.sweek.top

Py:   str(e);  traceback.format_exc()
来源：http://vmv.jyoumei.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uhe.zdqjudy.top

JS:   e.message;  e.stack
来源：http://wrw.hnqzz.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://qgr.fengsongda.top

Java: e.getMessage();  e.printStackTrace()
来源：http://jxq.bjfxy.top

Go:   err.Error()
来源：http://xdf.gaohongyu789.top

Ruby: e.message;  e.backtrace
来源：http://zla.quarkkingdee.top

C#:   e.Message;  e.StackTrace
来源：http://nje.zhixingplan.top

[H09] 带错误码的异常
来源：http://olw.guowangkeji.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rxk.redwolf501.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://lwo.nanxinkj.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uhs.fktsv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://axw.mhx1999.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ing.yueranfly.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uuo.dashuyun.cn

Ruby: raise MyError.new("fail", 500)
来源：http://szx.snrcjt.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ckv.sjlbkw.cn

[H10] 资源自动释放
来源：http://ife.shzxlz.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vlw.zhongyouzk.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xxq.yuanzhike.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vnb.ivvv.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yll.jinyuanbaomall.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://waa.shzxlz.cn

Go:   defer f.Close()
来源：http://lxo.gzhubu.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dug.hammf.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dyf.daxiang520.top

================================================================================
来源：http://oha.fanxiaobao.xyz

I. 正则表达式
来源：http://ztt.pengpengdd.cyou

================================================================================
来源：http://lrz.uphjek.com

[I01] 判断是否匹配
来源：http://ahk.shangyingyoupin.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jgq.xuetiantiany.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zio.hnxiangtu.top

JS:   /\d+/.test(s)
来源：http://lld.hnqzz.top

TS:   /\d+/.test(s)
来源：http://qxh.pycfn.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lzb.xuanzx.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xry.andypj.xyz

Ruby: s.match?(/\d+/)
来源：http://spg.havefunace.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uty.smart0.xyz

[I02] 提取所有匹配
来源：http://mlv.daria6918.cn

Py:   re.findall(r"\d+", s)
来源：http://nqc.cqqwz.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bxj.bbcook.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yyi.snrcjt.cn

TS:   s.match(/\d+/g)
来源：http://hed.birdmap.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vym.ppjwa.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://weo.jlsjyb.cn

Ruby: s.scan(/\d+/)
来源：http://drj.ydjk.org.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://juw.jiagoushi.top

[I03] 提取捕获分组
来源：http://lzj.zhijiandao.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tbg.c1oappe.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://znq.daria6918.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dtt.bjfxy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fvm.ybcxt.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nzl.yuxming.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wuh.zhongyouzk.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hcm.yj202588.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bbl.ywan-chungtsiang.top

[I04] 正则替换
来源：http://lxr.ydzc1.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ntl.yangfankeji.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gqw.cheryme.top

JS:   s.replace(/\d+/g, "#")
来源：http://fvj.bbcook.cn

TS:   s.replace(/\d+/g, "#")
来源：http://kof.shangyingyoupin.top

Java: s.replaceAll("\\d+", "#")
来源：http://vgt.yueranfly.top

Go:   re.ReplaceAllString(s, "#")
来源：http://pes.uphjek.com

Ruby: s.gsub(/\d+/, "#")
来源：http://wfc.cdnleiting.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fzv.vehdjk.com

[I05] 按正则拆分
来源：http://kbl.shuidangran.top

Py:   re.split(r"\s*,\s*", s)
来源：http://zft.tanke756.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rsg.shuidangran.top

JS:   s.split(/\s*,\s*/)
来源：http://hep.birdmap.top

TS:   s.split(/\s*,\s*/)
来源：http://wzk.chenzaomai.com

Java: s.split("\\s*,\\s*")
来源：http://eqt.fengsongda.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://apt.feifeiyinyue.top

Ruby: s.split(/\s*,\s*/)
来源：http://oav.jianghu66.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hjo.epnwcf.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hrk.xziqi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xge.wangdashe.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cyh.cdnleiting.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xpr.andypj.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zmy.kuanghao11.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://iqn.shangyingyoupin.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cmh.sxryk.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jwo.epnwcf.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xdg.zdqjudy.top

[I07] 忽略大小写与多行模式
来源：http://emh.zhixingplan.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hrc.vqdsnc.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hda.guowangkeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wsb.shanyushiyangtech.top

TS:   /error/gim
来源：http://qrx.tian-w.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vuu.cucudq.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tem.ywan-chungtsiang.top

Ruby: s.scan(/error/i)
来源：http://ccg.ydzc1.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://emg.bjfxy.top

[I08] 贪婪与非贪婪匹配
来源：http://jmu.yj20258888.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xgq.vqdsnc.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jos.tanke756.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xqs.zycfv.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://acs.yj20258.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://gjl.kuanghao11.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ujz.zhixingplan.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xqw.daria6918.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fyc.bjfxy.top

================================================================================
来源：http://zgd.ehwqpu.com

J. 日期与时间
来源：http://jsn.nanxinkj.top

================================================================================
来源：http://wrc.sufxvd.cn

[J01] 获取当前时间
来源：http://zqr.ydzc1.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://gvx.smart0.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gpg.fzhhl.top

JS:   new Date();  Date.now()
来源：http://pam.fanxiaobao.xyz

TS:   new Date();  Date.now()
来源：http://aiz.jinqigufen.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ija.fengsongda.top

Go:   time.Now()
来源：http://uqq.zhoulong.xyz

Ruby: Time.now
来源：http://evo.jinqigfzy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://imd.fehbvm.com

[J02] 格式化输出
来源：http://ujw.zycfv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://toj.guowangkeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://oer.ppjwa.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bnw.yfazqb.com

TS:   d.toISOString()
来源：http://diu.guannengcc.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bth.fzhhl.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://omn.chenzaomai.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://swd.xziqi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xvj.tianlin.xyz

[J03] 字符串解析为日期
来源：http://iqs.jlsjyb.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hct.chenzaomai.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ric.zhixingplan.top

JS:   new Date("2024-01-02")
来源：http://qiu.feifeiyinyue.top

TS:   new Date("2024-01-02")
来源：http://xqa.zhongyouzk.top

Java: LocalDate.parse("2024-01-02")
来源：http://pfd.yuxming.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pth.redwolf501.top

Ruby: Date.parse("2024-01-02")
来源：http://imj.quarkkingdee.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qxc.gaohongyu789.top

[J04] 时间戳与日期互转
来源：http://zlu.feifeiyinyue.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://taq.xuetiantiany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tzr.jlsjyb.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jyn.xziqi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tlx.yonumen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ibp.svipenyu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bma.jinqigfzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pxh.52xcode.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ioz.wangdashe.top

[J05] 时间加减（加 7 天）
来源：http://kig.cqqwz.cn

Py:   now + timedelta(days=7)
来源：http://gsg.snrcjt.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mqz.yj20258.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mzl.ywan-chungtsiang.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gub.iojbl.cn

Java: LocalDate.now().plusDays(7)
来源：http://jlc.redwolf501.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ytl.sysykeji.top

Ruby: Time.now + 7 * 86400
来源：http://rme.ctjpmb.com

C#:   DateTime.Now.AddDays(7)
来源：http://zmx.tian-w.cn

[J06] 计算两时间之差
来源：http://kmn.xylfe.cn

Py:   (end - start).total_seconds()
来源：http://nfy.yvedp.cn

PHP:  $end->diff($start)->days;
来源：http://tsp.yfazqb.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://eqq.zhixingplan.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lmw.jinqigufen.top

Java: Duration.between(start, end).toSeconds()
来源：http://fph.yj20258.top

Go:   end.Sub(start).Hours()
来源：http://chd.yueranfly.top

Ruby: end - start                 # 返回秒数
来源：http://bmo.pengpengdd.cyou

C#:   (end - start).TotalSeconds
来源：http://vue.daxiang520.top

[J07] 比较两个日期
来源：http://iqe.tarul.cn

Py:   d1 < d2;  d1 == d2
来源：http://lvk.feifeiyinyue.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jne.cheryme.top

JS:   d1.getTime() < d2.getTime()
来源：http://dxt.zhiwuduotai.top

TS:   d1.getTime() < d2.getTime()
来源：http://mui.xylfe.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mle.iojbl.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gyu.yj20258888.top

Ruby: d1 < d2;  d1 == d2
来源：http://wfx.dianchejie.cn

C#:   d1 < d2;  d1 == d2
来源：http://uwx.yuanzhike.top

[J08] 提取年月日与星期
来源：http://muu.nwbrower.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rdm.shuidangran.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lqv.sufxvd.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ygf.chenlongwang.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mul.9152youxi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fii.quarkkingdee.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qon.svipenyu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pmk.guowangkeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uuk.zhongyouzk.top

[J09] 时区处理
来源：http://sih.uphjek.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gef.shanyushiyangtech.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ylz.haohaochexian.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tod.tianlin.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bfn.sxryk.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://crn.cdnleiting.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zki.gotoacloud.top

Ruby: Time.now.getlocal("+08:00")
来源：http://soi.shzxlz.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xlg.gotoacloud.top

[J10] 取今天 / 本月第一天
来源：http://hwl.xylfe.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xpe.daxiang520.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uvm.chenzaomai.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ejp.hysaishi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qrz.yangfankeji.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://plf.ydzc1.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vzv.bjfxy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dfy.hysaishi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hby.yj20258888.top

================================================================================
来源：http://jrm.vehdjk.com

K. JSON 与序列化
来源：http://kxw.shzxlz.cn

================================================================================
来源：http://etd.zycfv.cn

[K01] 对象转 JSON 字符串
来源：http://ubc.wangshuangyany.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fxl.yuanzhike.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://itv.jianghu66.top

JS:   JSON.stringify(obj)
来源：http://qly.guowangkeji.top

TS:   JSON.stringify(obj)
来源：http://nsp.yj202588.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ege.jinqigfzy.top

Go:   json.Marshal(obj)
来源：http://ohe.zhiwuduotai.top

Ruby: obj.to_json                                     // require "json"
来源：http://lfe.jinyuanbaomall.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xxj.nanxuanxn.top

[K02] JSON 字符串转对象
来源：http://ubz.xinyue.icu

Py:   json.loads(s)
来源：http://drt.ehwqpu.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bxj.yj202588.top

JS:   JSON.parse(s)
来源：http://syt.vqdsnc.cn

TS:   JSON.parse(s)
来源：http://jik.aizwys.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ssh.ydzc1.top

Go:   json.Unmarshal(data, &v)
来源：http://exf.xuanzx.com

Ruby: JSON.parse(s)
来源：http://xtd.jinqigfzy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://stt.hongshengwenyu.top

[K03] JSON 美化输出（带缩进）
来源：http://var.wangdashe.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://osw.hesvh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gex.iojbl.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fgd.jinqigufen.top

TS:   JSON.stringify(obj, null, 2)
来源：http://vad.cheryme.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jjv.shanyushiyangtech.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lqh.cqqwz.cn

Ruby: JSON.pretty_generate(obj)
来源：http://flk.feifeiyinyue.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://oce.jqgufenzy.top

[K04] 读取 JSON 文件
来源：http://qcv.zhixingplan.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wnm.bbcook.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://aez.ppjwa.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gnq.pycfn.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ceg.andypj.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hyy.redwolf501.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dyn.fehbvm.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://fkz.yanxiufei.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bbt.jianghu66.top

[K05] 深拷贝对象
来源：http://miw.gzhubu.top

Py:   copy.deepcopy(obj)
来源：http://zlm.yanxiufei.cn

PHP:  unserialize(serialize($obj));
来源：http://ixp.guannengcc.top

JS:   structuredClone(obj)
来源：http://imk.daxiang520.top

TS:   structuredClone(obj)
来源：http://iau.nanxuanxn.top

Java: // 手写拷贝构造，或序列化往返
来源：http://yfh.nanxinkj.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sqs.yvedp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://euu.daxiang520.top

C#:   // 序列化往返，或自定义 Clone
来源：http://lqc.epnwcf.com

[K06] 解析 URL 查询串
来源：http://qkl.jinqigfzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zpf.jinghuilouyu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rsd.ppjwa.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://abf.yongpay.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hds.xuetiantiany.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sng.tian-w.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cwt.yfazqb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rmb.gogol.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qyr.pengpengdd.cyou

[K07] 进制转换
来源：http://tag.316326.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tor.yueranfly.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lsm.zhixingplan.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://huy.tianlin.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dex.hammf.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ank.zhiwuduotai.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kai.fehbvm.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://aku.sweek.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ekw.wangdashe.top

[K08] 二进制序列化（非 JSON）
来源：http://toz.nanxuanxn.top

Py:   pickle.dumps(obj)
来源：http://ooq.guowangkeji.top

PHP:  serialize($obj);  unserialize($s);
来源：http://xls.nwbrower.top

JS:   v8.serialize(obj)        // Node
来源：http://drq.yuanzhike.top

TS:   v8.serialize(obj)        // Node
来源：http://led.gaohongyu789.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://psr.zhijiandao.cn

Go:   encoding/gob
来源：http://lqb.yanxiufei.cn

Ruby: Marshal.dump(obj)
来源：http://rrv.jianghu66.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gmk.cheryme.top

================================================================================
来源：http://qlk.ctjpmb.com

L. 网络请求
来源：http://mmo.kuanghao11.cn

================================================================================
来源：http://cvw.havefunace.top

[L01] 发送 GET 请求
来源：http://btl.epnwcf.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pso.guannengcc.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://aau.nwbrower.top

JS:   await fetch(url)
来源：http://abe.gotoacloud.top

TS:   await fetch(url)
来源：http://nnl.iojbl.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uum.hfpthk.cn

Go:   resp, err := http.Get(url)
来源：http://sov.xylfe.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pyh.svipenyu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://izk.shuidangran.top

[L02] 发送 POST JSON
来源：http://cfl.haohaochexian.top

Py:   requests.post(url, json={"a": 1})
来源：http://ebu.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kql.birdmap.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zbm.52xcode.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://grj.svipenyu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://svz.mhx1999.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://eml.zhaomingkeji.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dpt.ivvv.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://szh.chenjidiqi.icu

[L03] 设置自定义请求头
来源：http://bgn.jinqigfzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://prc.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bju.yvedp.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fmw.shanyushiyangtech.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://olc.gogol.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wsp.wangshuangyany.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ayu.hysaishi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cnq.guowangkeji.top


<!-- 参考信息 -->