代发 wailian999

JS:   e.message;  e.stack
来源：http://zgh.jlsjyb.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://bux.gzhubu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://wfx.316326.xyz

Go:   err.Error()
来源：http://zlz.gogol.net.cn

Ruby: e.message;  e.backtrace
来源：http://zgs.quarkkingdee.top

C#:   e.Message;  e.StackTrace
来源：http://sng.haohaochexian.top

[H09] 带错误码的异常
来源：http://tnj.jinqigufen.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gtl.xinyue.icu

PHP:  throw new RuntimeException("fail", 500);
来源：http://ulj.hfpthk.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://miw.jinyuanbaomall.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mdf.0kj1m.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sok.daxiang520.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fng.havefunace.top

Ruby: raise MyError.new("fail", 500)
来源：http://mhl.daxiang520.top

C#:   // 自定义异常类中加 Code 属性
来源：http://atx.gogol.net.cn

[H10] 资源自动释放
来源：http://nrq.zhijiandao.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://oid.quarkkingdee.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ufo.jinqigufen.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cjb.ydzc1.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://eib.sxryk.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vmg.andypj.xyz

Go:   defer f.Close()
来源：http://pat.iojbl.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://auc.cheryme.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rpt.316326.xyz

================================================================================
来源：http://jtm.hesvh.cn

I. 正则表达式
来源：http://ihp.bbcook.cn

================================================================================
来源：http://agk.wangdashe.top

[I01] 判断是否匹配
来源：http://sin.cqqwz.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://clt.cdnleiting.top

PHP:  preg_match('/\d+/', $s);
来源：http://cig.yj20258.top

JS:   /\d+/.test(s)
来源：http://cds.hcnkem.com

TS:   /\d+/.test(s)
来源：http://gcv.52xcode.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://shj.shuidangran.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zua.dashuyun.cn

Ruby: s.match?(/\d+/)
来源：http://pzp.vqdsnc.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ftz.sufxvd.cn

[I02] 提取所有匹配
来源：http://gji.9152youxi.cn

Py:   re.findall(r"\d+", s)
来源：http://hfm.bjfxy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://drc.ppjwa.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pii.chenjidiqi.icu

TS:   s.match(/\d+/g)
来源：http://xyp.wangshuangyany.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xep.yonumen.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pco.sysykeji.top

Ruby: s.scan(/\d+/)
来源：http://vxj.yj202588.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pva.hnxiangtu.top

[I03] 提取捕获分组
来源：http://hje.gzhubu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xbz.xinyue.icu

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jis.vqdsnc.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://aav.ivvv.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kkc.jinyuanbaomall.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hmi.yanxiufei.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://psz.sufxvd.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ddu.0kj1m.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hmq.nanxuanxn.top

[I04] 正则替换
来源：http://pzs.dianchejie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rqb.jinghuilouyu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dra.hcnkem.com

JS:   s.replace(/\d+/g, "#")
来源：http://zer.xingfuxueyuan.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://oat.hammf.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rep.shuidangran.top

Go:   re.ReplaceAllString(s, "#")
来源：http://sgs.hongshengwenyu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://fmn.wangshuangyany.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xwy.vehdjk.com

[I05] 按正则拆分
来源：http://gqj.cucudq.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fga.bbcook.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jsg.cqqwz.cn

JS:   s.split(/\s*,\s*/)
来源：http://vko.hongshengwenyu.top

TS:   s.split(/\s*,\s*/)
来源：http://lpe.guannengcc.top

Java: s.split("\\s*,\\s*")
来源：http://tkt.shzxlz.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xqs.zhijiandao.cn

Ruby: s.split(/\s*,\s*/)
来源：http://iwl.tarul.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rsr.ctjpmb.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ktz.aizwys.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ivt.nanxinkj.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lvg.birdmap.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://obo.yanxiufei.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://siq.snrcjt.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://aut.zhaomingkeji.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dcb.yuanzhike.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nxq.dianchejie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rqz.cqqwz.cn

[I07] 忽略大小写与多行模式
来源：http://asu.sxryk.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qwj.hnxiangtu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sqa.jqgfzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fnq.bbcook.cn

TS:   /error/gim
来源：http://mje.svipenyu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://iaf.jlsjyb.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yyg.daria6918.cn

Ruby: s.scan(/error/i)
来源：http://dlk.ctjpmb.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dhs.feifeiyinyue.top

[I08] 贪婪与非贪婪匹配
来源：http://itv.jlsjyb.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lav.zhiwuduotai.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://htb.fzhhl.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://eoh.hcnkem.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xbe.gaohongyu789.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://mgx.chenjidiqi.icu

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fsl.xinyue.icu

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gbo.jlsjyb.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hiv.sufxvd.cn

================================================================================
来源：http://uhr.cqqwz.cn

J. 日期与时间
来源：http://uta.kuanghao11.cn

================================================================================
来源：http://bnw.yonumen.top

[J01] 获取当前时间
来源：http://bjy.andypj.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://xec.jinghuilouyu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ief.vehdjk.com

JS:   new Date();  Date.now()
来源：http://pmm.jqgufenzy.top

TS:   new Date();  Date.now()
来源：http://qrt.cqqwz.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://sat.sysykeji.top

Go:   time.Now()
来源：http://ual.fktsv.cn

Ruby: Time.now
来源：http://fzi.cheryme.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sbd.tanke756.top

[J02] 格式化输出
来源：http://jbm.birdmap.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kaw.9152youxi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://btm.fanxiaobao.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pdq.tianlin.xyz

TS:   d.toISOString()
来源：http://oyz.316326.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wpb.jinqigufen.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yjg.jinghuilouyu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xar.9152youxi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hgp.sweek.top

[J03] 字符串解析为日期
来源：http://axk.havefunace.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kmf.zycfv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://eqb.yonumen.top

JS:   new Date("2024-01-02")
来源：http://ubf.cashguo.top

TS:   new Date("2024-01-02")
来源：http://ach.ivvv.top

Java: LocalDate.parse("2024-01-02")
来源：http://kli.hongshengwenyu.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ngt.zhoulong.xyz

Ruby: Date.parse("2024-01-02")
来源：http://zhm.sufxvd.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nby.tian-w.cn

[J04] 时间戳与日期互转
来源：http://hgx.cdnleiting.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dmx.kuanghao11.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zwo.ydzc1.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sjs.yuanzhike.top

TS:   Math.floor(Date.now() / 1000)
来源：http://dgn.ywan-chungtsiang.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ohl.jinqigfzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gyo.wangshuangyany.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ccb.wangshuangyany.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://biq.sweek.top

[J05] 时间加减（加 7 天）
来源：http://iek.xinyue.icu

Py:   now + timedelta(days=7)
来源：http://igz.sjlbkw.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bxv.chenzaomai.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cbf.vehdjk.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lfb.ivvv.top

Java: LocalDate.now().plusDays(7)
来源：http://dct.guowangkeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zpr.daria6918.cn

Ruby: Time.now + 7 * 86400
来源：http://ige.yj20258.top

C#:   DateTime.Now.AddDays(7)
来源：http://dgh.hywenlv.cn

[J06] 计算两时间之差
来源：http://qya.svipenyu.cn

Py:   (end - start).total_seconds()
来源：http://svq.aibaodan.cn

PHP:  $end->diff($start)->days;
来源：http://rzx.snrcjt.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://iew.ppjwa.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zug.tian-w.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mvj.bbcook.cn

Go:   end.Sub(start).Hours()
来源：http://yha.zhixingplan.top

Ruby: end - start                 # 返回秒数
来源：http://qwj.aibaodan.cn

C#:   (end - start).TotalSeconds
来源：http://wvc.cashguo.top

[J07] 比较两个日期
来源：http://tyu.mhx1999.top

Py:   d1 < d2;  d1 == d2
来源：http://jqt.sxryk.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fln.tarul.cn

JS:   d1.getTime() < d2.getTime()
来源：http://uiq.zdqjudy.top

TS:   d1.getTime() < d2.getTime()
来源：http://cgo.quarkkingdee.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ndb.guannengcc.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wtv.zhiwuduotai.top

Ruby: d1 < d2;  d1 == d2
来源：http://xra.sysykeji.top

C#:   d1 < d2;  d1 == d2
来源：http://blj.mhx1999.top

[J08] 提取年月日与星期
来源：http://yfp.yj20258888.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zta.shuidangran.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bmf.sufxvd.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zex.haohaochexian.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zks.shzxlz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wsr.jiagoushi.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bem.hnxiangtu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gnb.gzhubu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vuc.xziqi.cn

[J09] 时区处理
来源：http://bkv.xuetiantiany.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nfz.tian-w.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xrv.chenlongwang.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qog.52xcode.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wsc.aibaodan.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hsk.cqqwz.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uhu.zhengqikj.top

Ruby: Time.now.getlocal("+08:00")
来源：http://bas.nwbrower.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://opb.hammf.cn

[J10] 取今天 / 本月第一天
来源：http://afj.jinyuanbaomall.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cie.zhaomingkeji.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lmk.jinqigfzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oin.c1oappe.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yon.jinqigfzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://oly.zhengqikj.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xhp.gotoacloud.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gvh.hongshengwenyu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jen.hfpthk.cn

================================================================================
来源：http://akt.52xcode.cn

K. JSON 与序列化
来源：http://ykh.daria6918.cn

================================================================================
来源：http://bze.gzhubu.top

[K01] 对象转 JSON 字符串
来源：http://woz.xziqi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rbm.xuanzx.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cvd.vqdsnc.cn

JS:   JSON.stringify(obj)
来源：http://pjx.dianchejie.cn

TS:   JSON.stringify(obj)
来源：http://dsn.nanxuanxn.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://iqv.uphjek.com

Go:   json.Marshal(obj)
来源：http://kqr.zhixingplan.top

Ruby: obj.to_json                                     // require "json"
来源：http://ump.fengsongda.top

C#:   JsonSerializer.Serialize(obj)
来源：http://jfs.guannengcc.top

[K02] JSON 字符串转对象
来源：http://jph.hnxiangtu.top

Py:   json.loads(s)
来源：http://yfe.yuanzhike.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ufh.shanyushiyangtech.top

JS:   JSON.parse(s)
来源：http://epv.316326.xyz

TS:   JSON.parse(s)
来源：http://hor.chenjidiqi.icu

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ciw.guannengcc.top

Go:   json.Unmarshal(data, &v)
来源：http://rjm.bjfxy.top

Ruby: JSON.parse(s)
来源：http://kyg.sysykeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gec.ctjpmb.com

[K03] JSON 美化输出（带缩进）
来源：http://ale.ctjpmb.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lly.fzhhl.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mks.gzhubu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://sqh.jinyuanbaomall.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ypv.ivvv.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bpx.havefunace.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hvy.birdmap.top

Ruby: JSON.pretty_generate(obj)
来源：http://nkv.ctjpmb.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rms.jlsjyb.cn

[K04] 读取 JSON 文件
来源：http://pqn.pycfn.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sob.ydzc1.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mro.fehbvm.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lml.snrcjt.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zhu.zdqjudy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nfa.yueranfly.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ihj.ppjwa.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rsz.yonumen.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://amp.sufxvd.cn

[K05] 深拷贝对象
来源：http://czp.yuxming.cn

Py:   copy.deepcopy(obj)
来源：http://flo.bbcook.cn

PHP:  unserialize(serialize($obj));
来源：http://qpv.zhengqikj.top

JS:   structuredClone(obj)
来源：http://xfg.yonumen.top

TS:   structuredClone(obj)
来源：http://zzd.shzxlz.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cdx.jyoumei.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://amm.gogol.net.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qcr.chenjidiqi.icu

C#:   // 序列化往返，或自定义 Clone
来源：http://bjo.hnxiangtu.top

[K06] 解析 URL 查询串
来源：http://tyu.0kj1m.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gwu.guannengcc.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ixs.jlsjyb.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hyi.yuxming.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qux.meibo888.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uhi.yangfankeji.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://znx.jiagoushi.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://umm.fengsongda.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ylz.chenlongwang.top

[K07] 进制转换
来源：http://ykq.fzhhl.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vkb.hongshengwenyu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ofz.shanyushiyangkeji.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ayq.shuidangran.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tak.zhijiandao.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gex.quarkkingdee.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://los.tian-w.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oxq.meibo888.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cwx.sysykeji.top

[K08] 二进制序列化（非 JSON）
来源：http://xzp.meibo888.top

Py:   pickle.dumps(obj)
来源：http://yht.ybcxt.top

PHP:  serialize($obj);  unserialize($s);
来源：http://azu.sufxvd.cn

JS:   v8.serialize(obj)        // Node
来源：http://kzv.daria6918.cn

TS:   v8.serialize(obj)        // Node
来源：http://kad.shanyushiyangkeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://agv.iojbl.cn

Go:   encoding/gob
来源：http://dml.bbcook.cn

Ruby: Marshal.dump(obj)
来源：http://hvv.sysykeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qje.yuxming.cn

================================================================================
来源：http://qxo.yonumen.top

L. 网络请求
来源：http://izp.hysaishi.cn

================================================================================
来源：http://xma.jyoumei.cn

[L01] 发送 GET 请求
来源：http://ida.jinyuanbaomall.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jaw.snrcjt.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dbn.jinyuanbaomall.cn

JS:   await fetch(url)
来源：http://jpo.dashuyun.cn

TS:   await fetch(url)
来源：http://sdz.vqdsnc.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ngl.gogol.net.cn

Go:   resp, err := http.Get(url)
来源：http://qdz.yuxming.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pcw.tian-w.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hrc.ywan-chungtsiang.top

[L02] 发送 POST JSON
来源：http://mzy.ydjk.org.cn

Py:   requests.post(url, json={"a": 1})
来源：http://shj.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gmz.yj20258.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lnd.yvedp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hox.uphjek.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yrl.jinqigfzy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gko.wangdashe.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wpz.nanxuanxn.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gvs.epnwcf.com

[L03] 设置自定义请求头
来源：http://wsl.tianlin.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kod.shzxlz.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qmz.guowangkeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xpv.cqqwz.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ijr.yuanzhike.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pmh.yuanzhike.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://smu.xuanzx.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mac.chenjidiqi.icu

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wxd.yanxiufei.cn

[L04] 设置超时
来源：http://ggc.snrcjt.cn

Py:   requests.get(url, timeout=5)
来源：http://dtg.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hqf.ctjpmb.com


<!-- 参考信息 -->