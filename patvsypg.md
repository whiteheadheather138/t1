代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://qzs.uphjek.com

[H08] 获取错误信息与堆栈
来源：http://bgc.jqgufenzy.top

Py:   str(e);  traceback.format_exc()
来源：http://gdp.yj20258888.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xgu.chenjidiqi.icu

JS:   e.message;  e.stack
来源：http://hfh.havefunace.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ekk.sxryk.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fso.xylfe.cn

Go:   err.Error()
来源：http://ynp.yj20258888.top

Ruby: e.message;  e.backtrace
来源：http://yyk.chenlongwang.top

C#:   e.Message;  e.StackTrace
来源：http://nvw.gzhubu.top

[H09] 带错误码的异常
来源：http://yxo.xuetiantiany.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lmp.daria6918.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qmr.jlsjyb.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fjy.gzhubu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yrl.0kj1m.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cur.ppjwa.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ers.52xcode.cn

Ruby: raise MyError.new("fail", 500)
来源：http://quc.sweek.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ikw.yongpay.top

[H10] 资源自动释放
来源：http://dnz.zhijiandao.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xlh.hywenlv.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hgw.jinqigufen.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cna.uphjek.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nwf.yj20258888.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://eln.yfazqb.com

Go:   defer f.Close()
来源：http://zcj.feifeiyinyue.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://knk.nwbrower.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ywg.shanyushiyangtech.top

================================================================================
来源：http://xzr.cqqwz.cn

I. 正则表达式
来源：http://ugp.pengpengdd.cyou

================================================================================
来源：http://zau.jinqigfzy.top

[I01] 判断是否匹配
来源：http://man.haohaochexian.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://urh.hcnkem.com

PHP:  preg_match('/\d+/', $s);
来源：http://joj.hesvh.cn

JS:   /\d+/.test(s)
来源：http://gna.xylfe.cn

TS:   /\d+/.test(s)
来源：http://jiy.jinqigufen.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bym.hysaishi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tbf.epnwcf.com

Ruby: s.match?(/\d+/)
来源：http://oqr.yj202588.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uff.ydzc1.top

[I02] 提取所有匹配
来源：http://ova.sjlbkw.cn

Py:   re.findall(r"\d+", s)
来源：http://jqq.ydjk.org.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pek.smart0.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vff.jinyuanbaomall.cn

TS:   s.match(/\d+/g)
来源：http://lio.hongshengwenyu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jln.yj202588.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qyu.birdmap.top

Ruby: s.scan(/\d+/)
来源：http://qpj.xingfuxueyuan.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mwh.guowangkeji.top

[I03] 提取捕获分组
来源：http://mcg.sxryk.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uok.zhongyouzk.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kxl.snrcjt.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vgh.hesvh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://aka.ctjpmb.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fns.gogol.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ywx.hammf.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://beq.tian-w.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yzz.nanxinkj.top

[I04] 正则替换
来源：http://ztp.bbcook.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zpk.0kj1m.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yej.ywan-chungtsiang.top

JS:   s.replace(/\d+/g, "#")
来源：http://idl.jlsjyb.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wem.cdnleiting.top

Java: s.replaceAll("\\d+", "#")
来源：http://ses.yongpay.top

Go:   re.ReplaceAllString(s, "#")
来源：http://bst.shanyushiyangtech.top

Ruby: s.gsub(/\d+/, "#")
来源：http://bin.9152youxi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hmc.vehdjk.com

[I05] 按正则拆分
来源：http://wsn.chenlongwang.top

Py:   re.split(r"\s*,\s*", s)
来源：http://oce.nwbrower.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tnp.cucudq.cn

JS:   s.split(/\s*,\s*/)
来源：http://ebr.xziqi.cn

TS:   s.split(/\s*,\s*/)
来源：http://tdk.yj20258.top

Java: s.split("\\s*,\\s*")
来源：http://caz.yj202588.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vqu.daxiang520.top

Ruby: s.split(/\s*,\s*/)
来源：http://bxr.smart0.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yww.ydzc1.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hlt.quarkkingdee.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nrs.jqgfzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rnn.guannengcc.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blk.aibaodan.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tbk.zdbjq.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rac.chenjidiqi.icu

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qmb.zhongyouzk.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://teh.havefunace.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://drn.sysykeji.top

[I07] 忽略大小写与多行模式
来源：http://bms.zhongyouzk.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qgu.cqqwz.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rwn.havefunace.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xfu.chenlongwang.top

TS:   /error/gim
来源：http://xba.dashuyun.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ylb.jyoumei.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rxf.jyoumei.cn

Ruby: s.scan(/error/i)
来源：http://yqc.chenzaomai.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://khh.smart0.xyz

[I08] 贪婪与非贪婪匹配
来源：http://hab.ydjk.org.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://neq.wangshuangyany.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://but.gaohongyu789.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qkl.ywan-chungtsiang.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ahi.zhengqikj.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://hdt.zhiwuduotai.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uku.shanyushiyangtech.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hga.ppjwa.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yxa.jyoumei.cn

================================================================================
来源：http://omm.gaohongyu789.top

J. 日期与时间
来源：http://bzh.jinqigufen.top

================================================================================
来源：http://aps.yongpay.top

[J01] 获取当前时间
来源：http://nei.zycfv.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://uho.chenzaomai.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zpc.gotoacloud.top

JS:   new Date();  Date.now()
来源：http://quh.aibaodan.cn

TS:   new Date();  Date.now()
来源：http://mwu.nwbrower.top

Java: LocalDateTime.now();  Instant.now()
来源：http://avm.ivvv.top

Go:   time.Now()
来源：http://vje.fehbvm.com

Ruby: Time.now
来源：http://jre.zhijiandao.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jzc.cashguo.top

[J02] 格式化输出
来源：http://epi.shangyingyoupin.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iay.zhiwuduotai.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zye.pycfn.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pcr.vqdsnc.cn

TS:   d.toISOString()
来源：http://bbo.52xcode.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tyy.xingfuxueyuan.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://owg.xuanzx.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ihe.sjlbkw.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mmz.jqgfzy.top

[J03] 字符串解析为日期
来源：http://wnf.sufxvd.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yuq.cqqwz.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://llg.feifeiyinyue.top

JS:   new Date("2024-01-02")
来源：http://jzv.jqgfzy.top

TS:   new Date("2024-01-02")
来源：http://rtt.yfazqb.com

Java: LocalDate.parse("2024-01-02")
来源：http://dig.xziqi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://knl.gzhubu.top

Ruby: Date.parse("2024-01-02")
来源：http://zze.dashuyun.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://znx.fzhhl.top

[J04] 时间戳与日期互转
来源：http://fyc.xuanzx.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ugs.daxiang520.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ane.epnwcf.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ywn.hnqzz.top

TS:   Math.floor(Date.now() / 1000)
来源：http://mnk.haohaochexian.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fss.jiagoushi.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cwe.hywenlv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fjp.gotoacloud.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rnm.svipenyu.cn

[J05] 时间加减（加 7 天）
来源：http://kpl.yueranfly.top

Py:   now + timedelta(days=7)
来源：http://snn.0kj1m.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rnx.yj202588.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nsn.ydjk.org.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vdg.jinghuilouyu.cn

Java: LocalDate.now().plusDays(7)
来源：http://vsz.wangshuangyany.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fwu.yvedp.cn

Ruby: Time.now + 7 * 86400
来源：http://yaa.jinghuilouyu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://cub.ydjk.org.cn

[J06] 计算两时间之差
来源：http://qyt.yj20258888.top

Py:   (end - start).total_seconds()
来源：http://mnf.tarul.cn

PHP:  $end->diff($start)->days;
来源：http://daf.hysaishi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qqq.jianghu66.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jkn.birdmap.top

Java: Duration.between(start, end).toSeconds()
来源：http://iao.316326.xyz

Go:   end.Sub(start).Hours()
来源：http://gcl.smart0.xyz

Ruby: end - start                 # 返回秒数
来源：http://fls.hcnkem.com

C#:   (end - start).TotalSeconds
来源：http://bkt.sufxvd.cn

[J07] 比较两个日期
来源：http://aul.aizwys.cn

Py:   d1 < d2;  d1 == d2
来源：http://qbt.jinghuilouyu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nbe.mhx1999.top

JS:   d1.getTime() < d2.getTime()
来源：http://xti.hysaishi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ank.tianlin.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vlv.havefunace.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://syv.yangfankeji.com

Ruby: d1 < d2;  d1 == d2
来源：http://dmy.cqqwz.cn

C#:   d1 < d2;  d1 == d2
来源：http://xfp.yj202588.top

[J08] 提取年月日与星期
来源：http://wzq.ydzc1.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dqk.xingfuxueyuan.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xlx.jqgufenzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hmz.zhixingplan.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ugo.jinqigufen.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dej.epnwcf.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pam.zhoulong.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sfx.nanxinkj.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://izg.yueranfly.top

[J09] 时区处理
来源：http://kfo.yongpay.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kuc.vqdsnc.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://etw.hesvh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rmg.ybcxt.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kxe.gotoacloud.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://aze.sufxvd.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yes.dashuyun.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zgy.wangdashe.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xzu.cqqwz.cn

[J10] 取今天 / 本月第一天
来源：http://ccp.xuanzx.com

Py:   date.today();  date.today().replace(day=1)
来源：http://ysu.fengsongda.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ukb.jlsjyb.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://waq.jyoumei.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://smd.hnqzz.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://puh.cucudq.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gvj.kuanghao11.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://oin.gaohongyu789.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://txx.yj202588.top

================================================================================
来源：http://skr.sjlbkw.cn

K. JSON 与序列化
来源：http://hxa.jqgufenzy.top

================================================================================
来源：http://bkx.xziqi.cn

[K01] 对象转 JSON 字符串
来源：http://qof.sufxvd.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nvs.tian-w.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wbh.yonumen.top

JS:   JSON.stringify(obj)
来源：http://igl.zhiwuduotai.top

TS:   JSON.stringify(obj)
来源：http://yrv.cashguo.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ltb.kuanghao11.cn

Go:   json.Marshal(obj)
来源：http://nxp.gaohongyu789.top

Ruby: obj.to_json                                     // require "json"
来源：http://yjd.vqdsnc.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://eoc.meibo888.top

[K02] JSON 字符串转对象
来源：http://zuu.c1oappe.top

Py:   json.loads(s)
来源：http://yxz.tarul.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sli.ybcxt.top

JS:   JSON.parse(s)
来源：http://mfc.chenjidiqi.icu

TS:   JSON.parse(s)
来源：http://gpk.aibaodan.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mpw.hnxiangtu.top

Go:   json.Unmarshal(data, &v)
来源：http://lnr.fehbvm.com

Ruby: JSON.parse(s)
来源：http://vwn.hysaishi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mbt.daxiang520.top

[K03] JSON 美化输出（带缩进）
来源：http://lif.uphjek.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xls.guannengcc.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ucq.zhengqikj.top

JS:   JSON.stringify(obj, null, 2)
来源：http://tod.xingfuxueyuan.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://zdi.hfpthk.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hxv.havefunace.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gqx.cucudq.cn

Ruby: JSON.pretty_generate(obj)
来源：http://mgt.chenjidiqi.icu

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dre.wangshuangyany.cn

[K04] 读取 JSON 文件
来源：http://lcd.havefunace.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nyp.ydzc1.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://crn.yfazqb.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ulw.yongpay.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ldi.fzhhl.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ewv.wangshuangyany.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dox.yuxming.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hju.dianchejie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dqn.yfazqb.com

[K05] 深拷贝对象
来源：http://epi.hfpthk.cn

Py:   copy.deepcopy(obj)
来源：http://znj.yueranfly.top

PHP:  unserialize(serialize($obj));
来源：http://osr.ydzc1.top

JS:   structuredClone(obj)
来源：http://zvo.jiagoushi.top

TS:   structuredClone(obj)
来源：http://khl.hcnkem.com

Java: // 手写拷贝构造，或序列化往返
来源：http://bdj.sjlbkw.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://weh.aizwys.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ljw.zhijiandao.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wie.bbcook.cn

[K06] 解析 URL 查询串
来源：http://nlt.yonumen.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tvb.hnqzz.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://agk.feifeiyinyue.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sky.zhengqikj.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qrv.shuidangran.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hbi.dianchejie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gvu.smart0.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ics.bbcook.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rbo.andypj.xyz

[K07] 进制转换
来源：http://ghl.meibo888.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kys.sweek.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tsm.sufxvd.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mww.yongpay.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ryc.hcnkem.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vky.xingfuxueyuan.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ssx.wangdashe.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ijt.hammf.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://aga.hammf.cn

[K08] 二进制序列化（非 JSON）
来源：http://ckc.hongshengwenyu.top

Py:   pickle.dumps(obj)
来源：http://ywv.hcnkem.com

PHP:  serialize($obj);  unserialize($s);
来源：http://nwh.jyoumei.cn

JS:   v8.serialize(obj)        // Node
来源：http://ebk.zdbjq.cn

TS:   v8.serialize(obj)        // Node
来源：http://rit.yfazqb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mla.redwolf501.top

Go:   encoding/gob
来源：http://via.zdbjq.cn

Ruby: Marshal.dump(obj)
来源：http://cvo.hfpthk.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://afx.uphjek.com

================================================================================
来源：http://kzx.ybcxt.top

L. 网络请求
来源：http://zhl.haohaochexian.top

================================================================================
来源：http://tjr.tianlin.xyz

[L01] 发送 GET 请求
来源：http://zho.gotoacloud.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kfd.daria6918.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://thj.redwolf501.top

JS:   await fetch(url)
来源：http://tvv.hnxiangtu.top

TS:   await fetch(url)
来源：http://oal.andypj.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fcu.iojbl.cn

Go:   resp, err := http.Get(url)
来源：http://mhh.uphjek.com

Ruby: Net::HTTP.get(URI(url))
来源：http://oci.wangshuangyany.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fou.epnwcf.com

[L02] 发送 POST JSON
来源：http://wip.hcnkem.com

Py:   requests.post(url, json={"a": 1})
来源：http://kdf.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nvw.yanxiufei.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xcj.zhijiandao.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gqg.yuxming.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dlt.jinghuilouyu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kfr.yangfankeji.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xzo.pengpengdd.cyou

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gqs.cashguo.top

[L03] 设置自定义请求头
来源：http://uph.cucudq.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://syw.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kah.daria6918.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wqw.yanxiufei.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bim.9152youxi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://apl.daria6918.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ajw.gogol.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lgw.nanxinkj.top


<!-- 参考信息 -->