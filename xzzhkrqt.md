代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://dkb.hywenlv.cn

[H08] 获取错误信息与堆栈
来源：http://jav.smart0.xyz

Py:   str(e);  traceback.format_exc()
来源：http://mve.hongshengwenyu.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cvh.jlsjyb.cn

JS:   e.message;  e.stack
来源：http://czh.52xcode.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://uba.vqdsnc.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xak.andypj.xyz

Go:   err.Error()
来源：http://jkx.shuidangran.top

Ruby: e.message;  e.backtrace
来源：http://lbt.jinqigfzy.top

C#:   e.Message;  e.StackTrace
来源：http://vxr.zdqjudy.top

[H09] 带错误码的异常
来源：http://ixn.snrcjt.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://upn.xziqi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gsb.0kj1m.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cxa.hongshengwenyu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hjp.jinghuilouyu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://scb.xuetiantiany.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mci.pengpengdd.cyou

Ruby: raise MyError.new("fail", 500)
来源：http://fww.zhaomingkeji.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://mbc.iojbl.cn

[H10] 资源自动释放
来源：http://rpg.gotoacloud.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://prg.yueranfly.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bng.yonumen.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wmp.nwbrower.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kpy.zdqjudy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://enf.wangshuangyany.cn

Go:   defer f.Close()
来源：http://ucw.ppjwa.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lxn.ctjpmb.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://euk.xuetiantiany.cn

================================================================================
来源：http://jxt.dianchejie.cn

I. 正则表达式
来源：http://wxz.vehdjk.com

================================================================================
来源：http://nmf.mhx1999.top

[I01] 判断是否匹配
来源：http://hwn.zhongyouzk.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://buj.zhixingplan.top

PHP:  preg_match('/\d+/', $s);
来源：http://bsk.nwbrower.top

JS:   /\d+/.test(s)
来源：http://hjt.ydjk.org.cn

TS:   /\d+/.test(s)
来源：http://sou.cashguo.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tts.fktsv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nku.nwbrower.top

Ruby: s.match?(/\d+/)
来源：http://jna.smart0.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ubd.iojbl.cn

[I02] 提取所有匹配
来源：http://ykq.yj20258888.top

Py:   re.findall(r"\d+", s)
来源：http://wro.ehwqpu.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nfp.nanxuanxn.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jqh.yueranfly.top

TS:   s.match(/\d+/g)
来源：http://fiv.pengpengdd.cyou

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://whi.dashuyun.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wcq.cucudq.cn

Ruby: s.scan(/\d+/)
来源：http://nbr.cqqwz.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nqd.shzxlz.cn

[I03] 提取捕获分组
来源：http://ooc.pengpengdd.cyou

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uig.ybcxt.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fyn.52xcode.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://czm.zdqjudy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zgr.jiagoushi.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yuo.ivvv.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qto.0kj1m.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://agt.ehwqpu.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yfa.fktsv.cn

[I04] 正则替换
来源：http://com.mhx1999.top

Py:   re.sub(r"\d+", "#", s)
来源：http://rty.wangshuangyany.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://grb.uphjek.com

JS:   s.replace(/\d+/g, "#")
来源：http://qsq.dianchejie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ctj.jinqigfzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://jaj.yangfankeji.com

Go:   re.ReplaceAllString(s, "#")
来源：http://zcs.nwbrower.top

Ruby: s.gsub(/\d+/, "#")
来源：http://xdo.nanxinkj.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uvb.ctjpmb.com

[I05] 按正则拆分
来源：http://loj.jiagoushi.top

Py:   re.split(r"\s*,\s*", s)
来源：http://qrf.uphjek.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gdk.nwbrower.top

JS:   s.split(/\s*,\s*/)
来源：http://kks.ybcxt.top

TS:   s.split(/\s*,\s*/)
来源：http://uov.yangfankeji.com

Java: s.split("\\s*,\\s*")
来源：http://zns.guowangkeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kxn.feifeiyinyue.top

Ruby: s.split(/\s*,\s*/)
来源：http://ets.fehbvm.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qum.hysaishi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lmu.52xcode.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://azj.sjlbkw.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://iiz.xinyue.icu

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lnd.chenlongwang.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cwu.shanyushiyangtech.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sas.daria6918.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ppo.jinghuilouyu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ysy.pycfn.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://foq.kuanghao11.cn

[I07] 忽略大小写与多行模式
来源：http://sij.chenjidiqi.icu

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lnf.havefunace.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fan.fanxiaobao.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://grk.ivvv.top

TS:   /error/gim
来源：http://csb.316326.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xxu.aizwys.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://une.hysaishi.cn

Ruby: s.scan(/error/i)
来源：http://afe.hnxiangtu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bvh.havefunace.top

[I08] 贪婪与非贪婪匹配
来源：http://egl.shangyingyoupin.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://paj.fzhhl.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dqd.yuxming.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://noj.hongshengwenyu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cjs.0kj1m.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hst.bbcook.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ssv.yonumen.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ozm.tianlin.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://oex.nanxinkj.top

================================================================================
来源：http://coz.guannengcc.top

J. 日期与时间
来源：http://lsz.fanxiaobao.xyz

================================================================================
来源：http://uww.ywan-chungtsiang.top

[J01] 获取当前时间
来源：http://bwi.quarkkingdee.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://mpp.jqgufenzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pgb.guowangkeji.top

JS:   new Date();  Date.now()
来源：http://fks.jinghuilouyu.cn

TS:   new Date();  Date.now()
来源：http://sir.316326.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://psr.ctjpmb.com

Go:   time.Now()
来源：http://tgz.bjfxy.top

Ruby: Time.now
来源：http://wpr.hcnkem.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xiu.xinyue.icu

[J02] 格式化输出
来源：http://izf.vqdsnc.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://svj.fktsv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://age.yangfankeji.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ncr.cucudq.cn

TS:   d.toISOString()
来源：http://zth.jinyuanbaomall.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jkr.daria6918.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lrs.jqgufenzy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pzi.pengpengdd.cyou

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tyy.wangdashe.top

[J03] 字符串解析为日期
来源：http://mru.ywan-chungtsiang.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ugc.jinqigfzy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://akn.zhoulong.xyz

JS:   new Date("2024-01-02")
来源：http://poc.nanxuanxn.top

TS:   new Date("2024-01-02")
来源：http://dgj.cqqwz.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qfi.haohaochexian.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sjy.xingfuxueyuan.xyz

Ruby: Date.parse("2024-01-02")
来源：http://nwo.daria6918.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ilg.zhixingplan.top

[J04] 时间戳与日期互转
来源：http://pko.chenjidiqi.icu

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fut.redwolf501.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://unm.ydjk.org.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sqq.ivvv.top

TS:   Math.floor(Date.now() / 1000)
来源：http://nhb.hywenlv.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tyv.yongpay.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://awj.316326.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://brf.jyoumei.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://flq.xingfuxueyuan.xyz

[J05] 时间加减（加 7 天）
来源：http://hyy.havefunace.top

Py:   now + timedelta(days=7)
来源：http://cbp.yvedp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kji.xziqi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qag.epnwcf.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://old.tarul.cn

Java: LocalDate.now().plusDays(7)
来源：http://drc.mhx1999.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uxy.zhiwuduotai.top

Ruby: Time.now + 7 * 86400
来源：http://bdh.cucudq.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jfm.jinqigufen.top

[J06] 计算两时间之差
来源：http://ven.hcnkem.com

Py:   (end - start).total_seconds()
来源：http://zzm.jianghu66.top

PHP:  $end->diff($start)->days;
来源：http://jzo.tian-w.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wta.meibo888.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ysb.yvedp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wye.sysykeji.top

Go:   end.Sub(start).Hours()
来源：http://ker.yj20258.top

Ruby: end - start                 # 返回秒数
来源：http://eep.zdqjudy.top

C#:   (end - start).TotalSeconds
来源：http://iic.fktsv.cn

[J07] 比较两个日期
来源：http://zgk.hysaishi.cn

Py:   d1 < d2;  d1 == d2
来源：http://thd.redwolf501.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pmd.feifeiyinyue.top

JS:   d1.getTime() < d2.getTime()
来源：http://ulx.xingfuxueyuan.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://xtn.chenlongwang.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fcc.yongpay.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ylg.cashguo.top

Ruby: d1 < d2;  d1 == d2
来源：http://qzu.yfazqb.com

C#:   d1 < d2;  d1 == d2
来源：http://sla.ywan-chungtsiang.top

[J08] 提取年月日与星期
来源：http://nmj.haohaochexian.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ocs.haohaochexian.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://olc.nanxuanxn.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blh.fanxiaobao.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yos.yueranfly.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ujs.c1oappe.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kkc.epnwcf.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ysq.yanxiufei.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tvv.xingfuxueyuan.xyz

[J09] 时区处理
来源：http://jzm.gzhubu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tse.cucudq.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bso.yanxiufei.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jbe.shanyushiyangkeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zut.chenzaomai.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://aee.pengpengdd.cyou

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yxh.shanyushiyangkeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ipa.ydzc1.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ebe.mhx1999.top

[J10] 取今天 / 本月第一天
来源：http://mym.yongpay.top

Py:   date.today();  date.today().replace(day=1)
来源：http://uir.jqgfzy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cvj.zhengqikj.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hke.316326.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rpq.aibaodan.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pnp.gogol.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://eck.hnxiangtu.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vls.nwbrower.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hyi.meibo888.top

================================================================================
来源：http://njd.jianghu66.top

K. JSON 与序列化
来源：http://lgw.zhongyouzk.top

================================================================================
来源：http://ovn.zhengqikj.top

[K01] 对象转 JSON 字符串
来源：http://hip.sweek.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sbe.hnqzz.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fuy.fehbvm.com

JS:   JSON.stringify(obj)
来源：http://rfb.pengpengdd.cyou

TS:   JSON.stringify(obj)
来源：http://etc.fengsongda.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wba.zhoulong.xyz

Go:   json.Marshal(obj)
来源：http://pza.zhaomingkeji.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://atj.chenzaomai.com

C#:   JsonSerializer.Serialize(obj)
来源：http://rrd.zycfv.cn

[K02] JSON 字符串转对象
来源：http://rwn.pycfn.com

Py:   json.loads(s)
来源：http://pug.zhengqikj.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kue.jqgufenzy.top

JS:   JSON.parse(s)
来源：http://xoz.fanxiaobao.xyz

TS:   JSON.parse(s)
来源：http://xiv.epnwcf.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rss.nwbrower.top

Go:   json.Unmarshal(data, &v)
来源：http://sec.ybcxt.top

Ruby: JSON.parse(s)
来源：http://icy.chenjidiqi.icu

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nyr.ehwqpu.com

[K03] JSON 美化输出（带缩进）
来源：http://zhx.yj20258888.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nic.cqqwz.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://juo.hysaishi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ipw.cdnleiting.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ujm.sjlbkw.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yej.sufxvd.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yli.andypj.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://qly.jinqigufen.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tmb.cdnleiting.top

[K04] 读取 JSON 文件
来源：http://eaw.tian-w.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://txh.ybcxt.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lmp.yvedp.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cfg.hongshengwenyu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nnh.vqdsnc.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://krr.yanxiufei.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yym.jinyuanbaomall.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://znp.9152youxi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kai.daxiang520.top

[K05] 深拷贝对象
来源：http://wmc.tianlin.xyz

Py:   copy.deepcopy(obj)
来源：http://uey.yfazqb.com

PHP:  unserialize(serialize($obj));
来源：http://dxz.hnxiangtu.top

JS:   structuredClone(obj)
来源：http://jwr.havefunace.top

TS:   structuredClone(obj)
来源：http://ypz.hysaishi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kjm.daria6918.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wvp.yuanzhike.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://whf.zhoulong.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://bbf.xingfuxueyuan.xyz

[K06] 解析 URL 查询串
来源：http://mxs.hfpthk.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zzo.vehdjk.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zfk.yvedp.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mrw.ydzc1.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zwr.yueranfly.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://szb.hnxiangtu.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://vej.uphjek.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oeh.c1oappe.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yjo.zycfv.cn

[K07] 进制转换
来源：http://mts.smart0.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gmj.xingfuxueyuan.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ivw.tarul.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rwi.yuanzhike.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uvw.zycfv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wky.yangfankeji.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gnn.fehbvm.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ggs.smart0.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://afe.ehwqpu.com

[K08] 二进制序列化（非 JSON）
来源：http://uqk.zhengqikj.top

Py:   pickle.dumps(obj)
来源：http://nab.nwbrower.top

PHP:  serialize($obj);  unserialize($s);
来源：http://goi.kuanghao11.cn

JS:   v8.serialize(obj)        // Node
来源：http://qux.jinyuanbaomall.cn

TS:   v8.serialize(obj)        // Node
来源：http://ouc.ydjk.org.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rqc.jqgufenzy.top

Go:   encoding/gob
来源：http://xnl.zhongyouzk.top

Ruby: Marshal.dump(obj)
来源：http://jyd.iojbl.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yas.zhaomingkeji.xyz

================================================================================
来源：http://hsc.uphjek.com

L. 网络请求
来源：http://zfm.hcnkem.com

================================================================================
来源：http://swf.fktsv.cn

[L01] 发送 GET 请求
来源：http://wfh.sxryk.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xlh.cheryme.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jrl.jinqigfzy.top

JS:   await fetch(url)
来源：http://die.wangshuangyany.cn

TS:   await fetch(url)
来源：http://ibv.wangdashe.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pbz.52xcode.cn

Go:   resp, err := http.Get(url)
来源：http://gzo.yvedp.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://oef.uphjek.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://peq.guannengcc.top

[L02] 发送 POST JSON
来源：http://sbv.nanxinkj.top

Py:   requests.post(url, json={"a": 1})
来源：http://uyh.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://akb.nanxuanxn.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jmz.gotoacloud.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oes.uphjek.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dfn.nanxuanxn.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://eay.sysykeji.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zdm.xuetiantiany.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://aqd.sweek.top

[L03] 设置自定义请求头
来源：http://bjb.cqqwz.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ajy.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zii.sufxvd.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gop.jianghu66.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xhk.jinyuanbaomall.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wyn.gotoacloud.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vbm.hesvh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://iko.jinghuilouyu.cn


<!-- 参考信息 -->