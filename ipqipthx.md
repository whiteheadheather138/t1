代发 wailian999

TS:   console.assert(x > 0);
来源：http://qdg.0kj1m.cn

Java: assert x > 0 : "必须为正";
来源：http://fyi.ydzc1.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xpe.zhaomingkeji.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://nrr.hcnkem.com

C#:   Debug.Assert(x > 0);
来源：http://kpf.hcnkem.com

[H08] 获取错误信息与堆栈
来源：http://jpw.hongshengwenyu.top

Py:   str(e);  traceback.format_exc()
来源：http://yzk.uphjek.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xrj.cqqwz.cn

JS:   e.message;  e.stack
来源：http://tvg.svipenyu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://txb.jiagoushi.top

Java: e.getMessage();  e.printStackTrace()
来源：http://lnc.tarul.cn

Go:   err.Error()
来源：http://fme.svipenyu.cn

Ruby: e.message;  e.backtrace
来源：http://bee.wangdashe.top

C#:   e.Message;  e.StackTrace
来源：http://vqi.guannengcc.top

[H09] 带错误码的异常
来源：http://fol.sysykeji.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pss.tianlin.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://jzm.chenzaomai.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kft.shanyushiyangkeji.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pao.daxiang520.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rmn.redwolf501.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lym.sweek.top

Ruby: raise MyError.new("fail", 500)
来源：http://buf.quarkkingdee.top

C#:   // 自定义异常类中加 Code 属性
来源：http://koj.cashguo.top

[H10] 资源自动释放
来源：http://qnr.tianlin.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://rwh.guowangkeji.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://slq.zdqjudy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zvc.zhongyouzk.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mfg.hcnkem.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gkc.cqqwz.cn

Go:   defer f.Close()
来源：http://ljw.aizwys.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://icd.ehwqpu.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sof.sufxvd.cn

================================================================================
来源：http://pmg.aizwys.cn

I. 正则表达式
来源：http://rfs.ivvv.top

================================================================================
来源：http://ngt.yfazqb.com

[I01] 判断是否匹配
来源：http://keb.iojbl.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qwk.xingfuxueyuan.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://zzk.jiagoushi.top

JS:   /\d+/.test(s)
来源：http://pyh.havefunace.top

TS:   /\d+/.test(s)
来源：http://tcs.cucudq.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wrj.haohaochexian.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ijw.sysykeji.top

Ruby: s.match?(/\d+/)
来源：http://vyn.yj20258.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xzc.nanxuanxn.top

[I02] 提取所有匹配
来源：http://dmn.yj20258888.top

Py:   re.findall(r"\d+", s)
来源：http://kpg.xingfuxueyuan.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://eyf.yanxiufei.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://iou.jinqigfzy.top

TS:   s.match(/\d+/g)
来源：http://pxr.shanyushiyangtech.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gbw.cashguo.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pue.vehdjk.com

Ruby: s.scan(/\d+/)
来源：http://rip.hywenlv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://acz.feifeiyinyue.top

[I03] 提取捕获分组
来源：http://wmg.tanke756.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hxw.jqgufenzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jto.snrcjt.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zim.jinyuanbaomall.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jvr.hnqzz.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bkd.cheryme.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fcu.wangdashe.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dqg.9152youxi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nqi.nwbrower.top

[I04] 正则替换
来源：http://zxq.hongshengwenyu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://kvj.chenlongwang.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jjr.yj202588.top

JS:   s.replace(/\d+/g, "#")
来源：http://ebs.ydzc1.top

TS:   s.replace(/\d+/g, "#")
来源：http://erl.shuidangran.top

Java: s.replaceAll("\\d+", "#")
来源：http://cfn.zdqjudy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://tdz.uphjek.com

Ruby: s.gsub(/\d+/, "#")
来源：http://tew.yj20258.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://iav.pycfn.com

[I05] 按正则拆分
来源：http://wzo.smart0.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://ksw.fktsv.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pvf.xuetiantiany.cn

JS:   s.split(/\s*,\s*/)
来源：http://ecb.c1oappe.top

TS:   s.split(/\s*,\s*/)
来源：http://lnc.ydjk.org.cn

Java: s.split("\\s*,\\s*")
来源：http://zbe.zhiwuduotai.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://onu.feifeiyinyue.top

Ruby: s.split(/\s*,\s*/)
来源：http://uur.feifeiyinyue.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qea.shzxlz.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kzk.52xcode.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zdt.wangdashe.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ldv.xylfe.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yfq.gogol.net.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jcj.wangshuangyany.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gdv.fanxiaobao.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://iws.fanxiaobao.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hwr.xingfuxueyuan.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lfj.gogol.net.cn

[I07] 忽略大小写与多行模式
来源：http://sws.xuetiantiany.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://oem.zhaomingkeji.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://iem.zhaomingkeji.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://eml.hfpthk.cn

TS:   /error/gim
来源：http://smn.feifeiyinyue.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kfl.shanyushiyangtech.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nvo.ydjk.org.cn

Ruby: s.scan(/error/i)
来源：http://lnj.smart0.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kve.fzhhl.top

[I08] 贪婪与非贪婪匹配
来源：http://hez.jlsjyb.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://akl.zhiwuduotai.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ruv.hesvh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ouh.yuanzhike.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://moa.ivvv.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://dru.shanyushiyangkeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ovq.fengsongda.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mid.yongpay.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mxp.fktsv.cn

================================================================================
来源：http://vjn.chenjidiqi.icu

J. 日期与时间
来源：http://phh.tianlin.xyz

================================================================================
来源：http://aez.cqqwz.cn

[J01] 获取当前时间
来源：http://keq.xylfe.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://nkh.c1oappe.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gqo.zdqjudy.top

JS:   new Date();  Date.now()
来源：http://hmh.zdqjudy.top

TS:   new Date();  Date.now()
来源：http://lcw.aizwys.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rzd.quarkkingdee.top

Go:   time.Now()
来源：http://eqo.cucudq.cn

Ruby: Time.now
来源：http://vne.nwbrower.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mmd.fktsv.cn

[J02] 格式化输出
来源：http://ycj.aibaodan.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ogn.pycfn.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ilx.sxryk.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cok.shzxlz.cn

TS:   d.toISOString()
来源：http://grp.ybcxt.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://akz.andypj.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sss.jianghu66.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vpn.zhoulong.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bpe.jinghuilouyu.cn

[J03] 字符串解析为日期
来源：http://ira.wangshuangyany.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bzz.zhengqikj.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://aqx.fktsv.cn

JS:   new Date("2024-01-02")
来源：http://qfr.havefunace.top

TS:   new Date("2024-01-02")
来源：http://mih.ywan-chungtsiang.top

Java: LocalDate.parse("2024-01-02")
来源：http://vmd.snrcjt.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dbr.chenjidiqi.icu

Ruby: Date.parse("2024-01-02")
来源：http://rbi.cdnleiting.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://shc.fehbvm.com

[J04] 时间戳与日期互转
来源：http://zos.hywenlv.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lsv.jyoumei.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pjx.cucudq.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nrg.zhaomingkeji.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://ilg.daria6918.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kpv.zdbjq.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uvl.hongshengwenyu.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vem.zhongyouzk.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lgq.tianlin.xyz

[J05] 时间加减（加 7 天）
来源：http://iro.ehwqpu.com

Py:   now + timedelta(days=7)
来源：http://gaa.andypj.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://hrb.snrcjt.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ezv.cashguo.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://juz.fehbvm.com

Java: LocalDate.now().plusDays(7)
来源：http://agd.chenzaomai.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://oui.ydjk.org.cn

Ruby: Time.now + 7 * 86400
来源：http://gus.nanxinkj.top

C#:   DateTime.Now.AddDays(7)
来源：http://jvo.havefunace.top

[J06] 计算两时间之差
来源：http://hpg.guowangkeji.top

Py:   (end - start).total_seconds()
来源：http://abh.shangyingyoupin.top

PHP:  $end->diff($start)->days;
来源：http://tqa.haohaochexian.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vtl.chenjidiqi.icu

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uxg.zhaomingkeji.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://hoy.jinyuanbaomall.cn

Go:   end.Sub(start).Hours()
来源：http://pqi.xingfuxueyuan.xyz

Ruby: end - start                 # 返回秒数
来源：http://cei.hesvh.cn

C#:   (end - start).TotalSeconds
来源：http://tro.hcnkem.com

[J07] 比较两个日期
来源：http://quu.fehbvm.com

Py:   d1 < d2;  d1 == d2
来源：http://hsv.iojbl.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://khg.hcnkem.com

JS:   d1.getTime() < d2.getTime()
来源：http://hoy.wangshuangyany.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pdm.yuxming.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tcz.shangyingyoupin.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qwd.guowangkeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://nis.pengpengdd.cyou

C#:   d1 < d2;  d1 == d2
来源：http://jlu.ppjwa.cn

[J08] 提取年月日与星期
来源：http://nuv.epnwcf.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jnx.hammf.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xch.hesvh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gdu.ctjpmb.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qak.iojbl.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sfh.xuetiantiany.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kfb.9152youxi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rri.xziqi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hyp.haohaochexian.top

[J09] 时区处理
来源：http://tfg.mhx1999.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rwo.hongshengwenyu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xiu.yangfankeji.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dyd.tarul.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pwo.ivvv.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sdv.fengsongda.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://oxu.yangfankeji.com

Ruby: Time.now.getlocal("+08:00")
来源：http://ufi.zhoulong.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zzz.yj20258888.top

[J10] 取今天 / 本月第一天
来源：http://dez.xinyue.icu

Py:   date.today();  date.today().replace(day=1)
来源：http://gku.316326.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hry.quarkkingdee.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xbk.zdqjudy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jrl.xziqi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://eqi.gogol.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://day.havefunace.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ihj.316326.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rlz.uphjek.com

================================================================================
来源：http://pta.hcnkem.com

K. JSON 与序列化
来源：http://kmq.yuanzhike.top

================================================================================
来源：http://onl.hcnkem.com

[K01] 对象转 JSON 字符串
来源：http://urc.yvedp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mhd.cqqwz.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uxy.yfazqb.com

JS:   JSON.stringify(obj)
来源：http://isg.zhongyouzk.top

TS:   JSON.stringify(obj)
来源：http://oaw.svipenyu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nzz.aizwys.cn

Go:   json.Marshal(obj)
来源：http://ssk.pengpengdd.cyou

Ruby: obj.to_json                                     // require "json"
来源：http://sga.sjlbkw.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nyv.cheryme.top

[K02] JSON 字符串转对象
来源：http://esh.andypj.xyz

Py:   json.loads(s)
来源：http://orq.52xcode.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hof.fktsv.cn

JS:   JSON.parse(s)
来源：http://vbj.yongpay.top

TS:   JSON.parse(s)
来源：http://vqn.zhoulong.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jfp.nwbrower.top

Go:   json.Unmarshal(data, &v)
来源：http://kex.yj20258.top

Ruby: JSON.parse(s)
来源：http://ahc.epnwcf.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://umb.jyoumei.cn

[K03] JSON 美化输出（带缩进）
来源：http://rjp.nanxuanxn.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xlb.ppjwa.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nsu.cashguo.top

JS:   JSON.stringify(obj, null, 2)
来源：http://tsr.cdnleiting.top

TS:   JSON.stringify(obj, null, 2)
来源：http://bfm.gzhubu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qai.aibaodan.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gkb.yj202588.top

Ruby: JSON.pretty_generate(obj)
来源：http://xgd.havefunace.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hra.gzhubu.top

[K04] 读取 JSON 文件
来源：http://gxo.shangyingyoupin.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rgv.bbcook.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rwn.zdqjudy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://adq.zhixingplan.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ann.chenlongwang.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wvk.jinqigfzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uko.svipenyu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://enl.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bju.yueranfly.top

[K05] 深拷贝对象
来源：http://jpn.cucudq.cn

Py:   copy.deepcopy(obj)
来源：http://ffp.yueranfly.top

PHP:  unserialize(serialize($obj));
来源：http://ufb.vqdsnc.cn

JS:   structuredClone(obj)
来源：http://kev.ctjpmb.com

TS:   structuredClone(obj)
来源：http://mby.yj20258888.top

Java: // 手写拷贝构造，或序列化往返
来源：http://nvb.jiagoushi.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mjv.bjfxy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lri.pengpengdd.cyou

C#:   // 序列化往返，或自定义 Clone
来源：http://hrs.daria6918.cn

[K06] 解析 URL 查询串
来源：http://dys.redwolf501.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rba.andypj.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wwd.feifeiyinyue.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mro.c1oappe.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pfp.zhengqikj.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ffa.yuanzhike.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://npi.jinqigfzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://eon.fanxiaobao.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://byw.wangshuangyany.cn

[K07] 进制转换
来源：http://cls.shanyushiyangtech.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qbt.epnwcf.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://eaf.yuanzhike.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://srt.svipenyu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qmg.shanyushiyangtech.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hyf.wangdashe.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kaw.pengpengdd.cyou

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://our.yongpay.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gxd.tian-w.cn

[K08] 二进制序列化（非 JSON）
来源：http://qsd.hnxiangtu.top

Py:   pickle.dumps(obj)
来源：http://low.zdqjudy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://nav.hesvh.cn

JS:   v8.serialize(obj)        // Node
来源：http://sbb.zhijiandao.cn

TS:   v8.serialize(obj)        // Node
来源：http://cck.quarkkingdee.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://eea.jqgufenzy.top

Go:   encoding/gob
来源：http://wcy.ywan-chungtsiang.top

Ruby: Marshal.dump(obj)
来源：http://hif.jyoumei.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qjk.jinqigfzy.top

================================================================================
来源：http://vsw.andypj.xyz

L. 网络请求
来源：http://lbc.meibo888.top

================================================================================
来源：http://xpk.fanxiaobao.xyz

[L01] 发送 GET 请求
来源：http://ntm.ppjwa.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://okq.52xcode.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tfn.cashguo.top

JS:   await fetch(url)
来源：http://fvu.pengpengdd.cyou

TS:   await fetch(url)
来源：http://ibb.bjfxy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://auj.jinyuanbaomall.cn

Go:   resp, err := http.Get(url)
来源：http://plh.havefunace.top

Ruby: Net::HTTP.get(URI(url))
来源：http://sgk.ctjpmb.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rcz.cqqwz.cn

[L02] 发送 POST JSON
来源：http://pfb.yanxiufei.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nfi.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ixa.52xcode.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wwx.jqgufenzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hko.zhixingplan.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://oyi.yuanzhike.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://svd.chenzaomai.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://exi.zhiwuduotai.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://heh.cdnleiting.top

[L03] 设置自定义请求头
来源：http://ghy.yj20258.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hxn.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://oaa.zhiwuduotai.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qjo.zhaomingkeji.xyz


<!-- 参考信息 -->