代发 wailian999

JS:   e.message;  e.stack
来源：http://uea.ehwqpu.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://evh.hysaishi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nng.hesvh.cn

Go:   err.Error()
来源：http://hfq.hcnkem.com

Ruby: e.message;  e.backtrace
来源：http://gor.ivvv.top

C#:   e.Message;  e.StackTrace
来源：http://sbs.cqqwz.cn

[H09] 带错误码的异常
来源：http://jba.sweek.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fjn.316326.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://nlp.jinyuanbaomall.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mwa.fzhhl.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ijk.feifeiyinyue.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ujl.yfazqb.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gyj.svipenyu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vth.shanyushiyangtech.top

C#:   // 自定义异常类中加 Code 属性
来源：http://khn.yj20258.top

[H10] 资源自动释放
来源：http://giu.hysaishi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vdy.daria6918.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bvp.shzxlz.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bpn.fzhhl.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kbx.havefunace.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ibh.bjfxy.top

Go:   defer f.Close()
来源：http://efh.feifeiyinyue.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cqy.yanxiufei.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ymr.fanxiaobao.xyz

================================================================================
来源：http://nce.jyoumei.cn

I. 正则表达式
来源：http://hlo.dianchejie.cn

================================================================================
来源：http://xyx.sjlbkw.cn

[I01] 判断是否匹配
来源：http://oyv.zdbjq.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mrb.9152youxi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ffv.jlsjyb.cn

JS:   /\d+/.test(s)
来源：http://lii.ybcxt.top

TS:   /\d+/.test(s)
来源：http://zge.daria6918.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nus.meibo888.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vtj.yj202588.top

Ruby: s.match?(/\d+/)
来源：http://aml.chenjidiqi.icu

C#:   Regex.IsMatch(s, @"\d+")
来源：http://iup.yonumen.top

[I02] 提取所有匹配
来源：http://kae.bbcook.cn

Py:   re.findall(r"\d+", s)
来源：http://vph.yj202588.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ctk.ctjpmb.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pzn.guannengcc.top

TS:   s.match(/\d+/g)
来源：http://piu.epnwcf.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yfr.gotoacloud.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://onu.zhixingplan.top

Ruby: s.scan(/\d+/)
来源：http://cya.sweek.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nwl.yj20258888.top

[I03] 提取捕获分组
来源：http://wwi.xuanzx.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pgs.jinghuilouyu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rlo.snrcjt.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://oxz.shanyushiyangtech.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ixr.yvedp.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://smd.ywan-chungtsiang.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ksx.xuetiantiany.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ojf.zhoulong.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xom.hnqzz.top

[I04] 正则替换
来源：http://pnr.hesvh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ooi.yvedp.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mhd.quarkkingdee.top

JS:   s.replace(/\d+/g, "#")
来源：http://fxr.xingfuxueyuan.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://yyj.wangdashe.top

Java: s.replaceAll("\\d+", "#")
来源：http://tjh.nanxinkj.top

Go:   re.ReplaceAllString(s, "#")
来源：http://qea.tian-w.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zrz.nanxinkj.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xxn.c1oappe.top

[I05] 按正则拆分
来源：http://ctf.guannengcc.top

Py:   re.split(r"\s*,\s*", s)
来源：http://vof.shuidangran.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mjn.jiagoushi.top

JS:   s.split(/\s*,\s*/)
来源：http://fyc.hnxiangtu.top

TS:   s.split(/\s*,\s*/)
来源：http://trp.cashguo.top

Java: s.split("\\s*,\\s*")
来源：http://xmg.epnwcf.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://egv.zdqjudy.top

Ruby: s.split(/\s*,\s*/)
来源：http://sxs.cucudq.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bvk.hysaishi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gfu.haohaochexian.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hko.guowangkeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pin.52xcode.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lij.guowangkeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gdq.tian-w.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bpa.tianlin.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tgm.vqdsnc.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mmb.shanyushiyangtech.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gfa.hfpthk.cn

[I07] 忽略大小写与多行模式
来源：http://eel.nanxinkj.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xfl.52xcode.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lmk.yangfankeji.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bnn.ivvv.top

TS:   /error/gim
来源：http://ieb.jianghu66.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://elx.yuanzhike.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lfs.yangfankeji.com

Ruby: s.scan(/error/i)
来源：http://nbj.sysykeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dsu.cashguo.top

[I08] 贪婪与非贪婪匹配
来源：http://gfy.ydzc1.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tng.smart0.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tih.svipenyu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fsl.xuetiantiany.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ecv.andypj.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://wes.andypj.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://agm.hnxiangtu.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fpx.cqqwz.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pts.epnwcf.com

================================================================================
来源：http://qad.havefunace.top

J. 日期与时间
来源：http://wsw.jqgufenzy.top

================================================================================
来源：http://wbz.xziqi.cn

[J01] 获取当前时间
来源：http://qpa.smart0.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://ydk.vehdjk.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rkp.zhoulong.xyz

JS:   new Date();  Date.now()
来源：http://ysw.chenjidiqi.icu

TS:   new Date();  Date.now()
来源：http://udt.jlsjyb.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kco.daria6918.cn

Go:   time.Now()
来源：http://btw.svipenyu.cn

Ruby: Time.now
来源：http://hkj.daria6918.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vju.yuxming.cn

[J02] 格式化输出
来源：http://xhl.hesvh.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uqi.ydzc1.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wrf.xuanzx.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zoi.shanyushiyangkeji.top

TS:   d.toISOString()
来源：http://afz.shanyushiyangtech.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tqz.yfazqb.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nvv.guannengcc.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qnt.c1oappe.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pcs.ehwqpu.com

[J03] 字符串解析为日期
来源：http://tmx.shuidangran.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zqz.wangshuangyany.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ded.fktsv.cn

JS:   new Date("2024-01-02")
来源：http://ljq.zhaomingkeji.xyz

TS:   new Date("2024-01-02")
来源：http://mat.yanxiufei.cn

Java: LocalDate.parse("2024-01-02")
来源：http://eoc.yfazqb.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://psw.fzhhl.top

Ruby: Date.parse("2024-01-02")
来源：http://yod.cucudq.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vfy.smart0.xyz

[J04] 时间戳与日期互转
来源：http://ybt.nanxuanxn.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://you.vqdsnc.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://odn.shuidangran.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rlu.sysykeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://gnx.hcnkem.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ueb.sjlbkw.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://euk.jinqigufen.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://eyi.ivvv.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://idq.ppjwa.cn

[J05] 时间加减（加 7 天）
来源：http://qpi.hongshengwenyu.top

Py:   now + timedelta(days=7)
来源：http://kev.uphjek.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://duw.hnqzz.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cmb.yj202588.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nzs.sysykeji.top

Java: LocalDate.now().plusDays(7)
来源：http://kwh.xziqi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://whu.snrcjt.cn

Ruby: Time.now + 7 * 86400
来源：http://teg.jlsjyb.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ioa.cheryme.top

[J06] 计算两时间之差
来源：http://hgi.ctjpmb.com

Py:   (end - start).total_seconds()
来源：http://agm.gogol.net.cn

PHP:  $end->diff($start)->days;
来源：http://iee.yonumen.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tgm.jlsjyb.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rod.gzhubu.top

Java: Duration.between(start, end).toSeconds()
来源：http://hvp.zycfv.cn

Go:   end.Sub(start).Hours()
来源：http://tiw.ivvv.top

Ruby: end - start                 # 返回秒数
来源：http://oqp.yonumen.top

C#:   (end - start).TotalSeconds
来源：http://ice.fanxiaobao.xyz

[J07] 比较两个日期
来源：http://emr.yueranfly.top

Py:   d1 < d2;  d1 == d2
来源：http://eeu.jiagoushi.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tdp.haohaochexian.top

JS:   d1.getTime() < d2.getTime()
来源：http://fci.ybcxt.top

TS:   d1.getTime() < d2.getTime()
来源：http://tuk.jiagoushi.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rnc.svipenyu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mfk.hnqzz.top

Ruby: d1 < d2;  d1 == d2
来源：http://qvw.ehwqpu.com

C#:   d1 < d2;  d1 == d2
来源：http://kca.zdqjudy.top

[J08] 提取年月日与星期
来源：http://iio.xinyue.icu

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ndc.hywenlv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fpy.gotoacloud.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xbq.yangfankeji.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rfn.chenlongwang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tkt.xingfuxueyuan.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cfa.zhiwuduotai.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dha.xuetiantiany.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vll.tarul.cn

[J09] 时区处理
来源：http://ssd.havefunace.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://duw.shuidangran.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://szq.zhixingplan.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tcs.guannengcc.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://npz.shzxlz.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rkh.ehwqpu.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cgr.chenjidiqi.icu

Ruby: Time.now.getlocal("+08:00")
来源：http://kvw.cashguo.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lcu.hnqzz.top

[J10] 取今天 / 本月第一天
来源：http://vic.tarul.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bpj.ctjpmb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://enf.ydjk.org.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ajn.ywan-chungtsiang.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xxq.dianchejie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pwd.yuxming.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://noo.pengpengdd.cyou

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://khj.yvedp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://whn.nanxinkj.top

================================================================================
来源：http://dwk.dianchejie.cn

K. JSON 与序列化
来源：http://wse.tian-w.cn

================================================================================
来源：http://fbo.havefunace.top

[K01] 对象转 JSON 字符串
来源：http://tgj.jinqigufen.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://spz.jianghu66.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dqr.fengsongda.top

JS:   JSON.stringify(obj)
来源：http://twr.daxiang520.top

TS:   JSON.stringify(obj)
来源：http://iuy.svipenyu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xcd.yangfankeji.com

Go:   json.Marshal(obj)
来源：http://pvs.yangfankeji.com

Ruby: obj.to_json                                     // require "json"
来源：http://axp.daxiang520.top

C#:   JsonSerializer.Serialize(obj)
来源：http://vam.nwbrower.top

[K02] JSON 字符串转对象
来源：http://vyi.zdqjudy.top

Py:   json.loads(s)
来源：http://rti.sysykeji.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pzy.dashuyun.cn

JS:   JSON.parse(s)
来源：http://nyr.xuetiantiany.cn

TS:   JSON.parse(s)
来源：http://kgk.dashuyun.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xiq.gaohongyu789.top

Go:   json.Unmarshal(data, &v)
来源：http://vko.hnxiangtu.top

Ruby: JSON.parse(s)
来源：http://ffz.cheryme.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mkh.xuetiantiany.cn

[K03] JSON 美化输出（带缩进）
来源：http://otk.c1oappe.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hjz.tian-w.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qji.vqdsnc.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pel.tianlin.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://kut.birdmap.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://eae.zhixingplan.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qbd.hesvh.cn

Ruby: JSON.pretty_generate(obj)
来源：http://lzv.tian-w.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lkf.tianlin.xyz

[K04] 读取 JSON 文件
来源：http://xtr.jinyuanbaomall.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cgb.cashguo.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sjy.zhengqikj.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jew.cashguo.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dez.shanyushiyangtech.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mld.yongpay.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://flk.shuidangran.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://dim.fzhhl.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jfr.hesvh.cn

[K05] 深拷贝对象
来源：http://are.zhiwuduotai.top

Py:   copy.deepcopy(obj)
来源：http://qhp.zhixingplan.top

PHP:  unserialize(serialize($obj));
来源：http://cht.tarul.cn

JS:   structuredClone(obj)
来源：http://srf.gaohongyu789.top

TS:   structuredClone(obj)
来源：http://bxx.gzhubu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://qul.nanxinkj.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pic.zhongyouzk.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://onh.hysaishi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ahx.chenjidiqi.icu

[K06] 解析 URL 查询串
来源：http://oes.yj20258888.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kln.xuetiantiany.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://prr.ydzc1.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kdb.ctjpmb.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jtu.yj202588.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://iba.hammf.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://nui.gzhubu.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yew.andypj.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://piy.ctjpmb.com

[K07] 进制转换
来源：http://hum.316326.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nzg.zhoulong.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ggp.yfazqb.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://smr.fanxiaobao.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tir.9152youxi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mun.zhoulong.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ycd.zhijiandao.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ryl.yuanzhike.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zyi.wangshuangyany.cn

[K08] 二进制序列化（非 JSON）
来源：http://mfv.dashuyun.cn

Py:   pickle.dumps(obj)
来源：http://ukf.daria6918.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ypo.wangdashe.top

JS:   v8.serialize(obj)        // Node
来源：http://tee.yueranfly.top

TS:   v8.serialize(obj)        // Node
来源：http://maw.zhixingplan.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qbe.dianchejie.cn

Go:   encoding/gob
来源：http://pzr.jinqigufen.top

Ruby: Marshal.dump(obj)
来源：http://zdf.tianlin.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xjt.svipenyu.cn

================================================================================
来源：http://hpg.hfpthk.cn

L. 网络请求
来源：http://szj.fzhhl.top

================================================================================
来源：http://tog.snrcjt.cn

[L01] 发送 GET 请求
来源：http://zwk.zycfv.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yoa.ybcxt.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lme.fanxiaobao.xyz

JS:   await fetch(url)
来源：http://dat.c1oappe.top

TS:   await fetch(url)
来源：http://pzw.yonumen.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ggn.pycfn.com

Go:   resp, err := http.Get(url)
来源：http://ufx.jiagoushi.top

Ruby: Net::HTTP.get(URI(url))
来源：http://nzj.jqgfzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wcb.sufxvd.cn

[L02] 发送 POST JSON
来源：http://zqg.tanke756.top

Py:   requests.post(url, json={"a": 1})
来源：http://lon.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tdk.dianchejie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ore.tarul.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zdv.daria6918.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zfx.xziqi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://axh.gzhubu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qxd.chenjidiqi.icu

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gth.nwbrower.top

[L03] 设置自定义请求头
来源：http://kxr.gzhubu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://oqf.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rmt.yuanzhike.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zeg.hnxiangtu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rgz.sxryk.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://eut.pengpengdd.cyou

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pqd.chenzaomai.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://evh.jinqigfzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lxb.sufxvd.cn

[L04] 设置超时
来源：http://myl.yj202588.top

Py:   requests.get(url, timeout=5)
来源：http://mmw.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mcd.zdqjudy.top


<!-- 参考信息 -->