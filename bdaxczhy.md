代发 wailian999

JS:   e.message;  e.stack
来源：http://nsr.andypj.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://axn.zhoulong.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://nps.pengpengdd.cyou

Go:   err.Error()
来源：http://jeh.0kj1m.cn

Ruby: e.message;  e.backtrace
来源：http://die.birdmap.top

C#:   e.Message;  e.StackTrace
来源：http://sqb.xylfe.cn

[H09] 带错误码的异常
来源：http://vab.sweek.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://opr.nanxuanxn.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://hah.jqgufenzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://crm.xziqi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pkg.xuetiantiany.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fvt.shanyushiyangkeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yxg.yangfankeji.com

Ruby: raise MyError.new("fail", 500)
来源：http://jud.tian-w.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hor.jinghuilouyu.cn

[H10] 资源自动释放
来源：http://hoq.tianlin.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://mdg.svipenyu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rko.ywan-chungtsiang.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xov.xziqi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kur.kuanghao11.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://roj.cashguo.top

Go:   defer f.Close()
来源：http://xec.dashuyun.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://olk.sweek.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jfy.hammf.cn

================================================================================
来源：http://bbz.yvedp.cn

I. 正则表达式
来源：http://ias.shuidangran.top

================================================================================
来源：http://ruc.zhengqikj.top

[I01] 判断是否匹配
来源：http://rbd.316326.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jtn.hammf.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xdf.sufxvd.cn

JS:   /\d+/.test(s)
来源：http://ate.hongshengwenyu.top

TS:   /\d+/.test(s)
来源：http://dki.hywenlv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rtq.bjfxy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zau.yj20258888.top

Ruby: s.match?(/\d+/)
来源：http://lmy.hysaishi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wld.jinqigfzy.top

[I02] 提取所有匹配
来源：http://jdz.chenjidiqi.icu

Py:   re.findall(r"\d+", s)
来源：http://gse.ctjpmb.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bqz.nanxinkj.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lrt.yfazqb.com

TS:   s.match(/\d+/g)
来源：http://ctu.zhaomingkeji.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yqu.shanyushiyangtech.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lsd.yj20258888.top

Ruby: s.scan(/\d+/)
来源：http://vtz.316326.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bzv.hnxiangtu.top

[I03] 提取捕获分组
来源：http://ddo.quarkkingdee.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qrb.jyoumei.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rwb.fanxiaobao.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tfa.gzhubu.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fct.ydjk.org.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://swu.zhaomingkeji.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wzo.cqqwz.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ylw.ctjpmb.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://thl.chenlongwang.top

[I04] 正则替换
来源：http://zsf.gzhubu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://gnf.ppjwa.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uei.ydjk.org.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ybj.yj20258888.top

TS:   s.replace(/\d+/g, "#")
来源：http://pes.shuidangran.top

Java: s.replaceAll("\\d+", "#")
来源：http://maw.hfpthk.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bae.chenjidiqi.icu

Ruby: s.gsub(/\d+/, "#")
来源：http://iuw.ctjpmb.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://klp.yvedp.cn

[I05] 按正则拆分
来源：http://zze.cqqwz.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xrd.bbcook.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://epm.shzxlz.cn

JS:   s.split(/\s*,\s*/)
来源：http://wok.zhongyouzk.top

TS:   s.split(/\s*,\s*/)
来源：http://bps.fzhhl.top

Java: s.split("\\s*,\\s*")
来源：http://bvv.vqdsnc.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zmi.zhiwuduotai.top

Ruby: s.split(/\s*,\s*/)
来源：http://uax.zdbjq.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pww.zycfv.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xmw.pengpengdd.cyou

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uho.aizwys.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ybf.havefunace.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://urv.nanxinkj.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tzo.zhongyouzk.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://foj.hongshengwenyu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rnn.epnwcf.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tvf.zhixingplan.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ehh.hywenlv.cn

[I07] 忽略大小写与多行模式
来源：http://ooo.jinqigfzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://awv.smart0.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cgy.tian-w.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://axj.aibaodan.cn

TS:   /error/gim
来源：http://ang.dianchejie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rqz.epnwcf.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dye.zhoulong.xyz

Ruby: s.scan(/error/i)
来源：http://iud.guannengcc.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dms.zhijiandao.cn

[I08] 贪婪与非贪婪匹配
来源：http://clz.iojbl.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ajg.shuidangran.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wmx.gzhubu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uad.pengpengdd.cyou

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yqv.cucudq.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://iua.mhx1999.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://idd.quarkkingdee.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dxw.nanxuanxn.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jxd.guowangkeji.top

================================================================================
来源：http://acc.chenjidiqi.icu

J. 日期与时间
来源：http://cud.meibo888.top

================================================================================
来源：http://tba.cashguo.top

[J01] 获取当前时间
来源：http://ans.yj202588.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://tsn.zhoulong.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://brm.gzhubu.top

JS:   new Date();  Date.now()
来源：http://lcm.bbcook.cn

TS:   new Date();  Date.now()
来源：http://esw.zdbjq.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://egs.yj20258.top

Go:   time.Now()
来源：http://ruu.cqqwz.cn

Ruby: Time.now
来源：http://srr.nanxinkj.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hob.zhoulong.xyz

[J02] 格式化输出
来源：http://lim.daria6918.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wqg.ppjwa.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qwo.zhengqikj.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ast.uphjek.com

TS:   d.toISOString()
来源：http://hzu.xingfuxueyuan.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sjh.316326.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yzf.havefunace.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oyb.yangfankeji.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://efh.shuidangran.top

[J03] 字符串解析为日期
来源：http://ucc.nwbrower.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ziq.52xcode.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tsi.cashguo.top

JS:   new Date("2024-01-02")
来源：http://dqc.birdmap.top

TS:   new Date("2024-01-02")
来源：http://tme.hywenlv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yea.ppjwa.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nzc.andypj.xyz

Ruby: Date.parse("2024-01-02")
来源：http://qxq.mhx1999.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://emc.yongpay.top

[J04] 时间戳与日期互转
来源：http://rgm.fehbvm.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pcv.shanyushiyangkeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://oqu.hesvh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://skc.ivvv.top

TS:   Math.floor(Date.now() / 1000)
来源：http://scg.yj20258888.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kvj.zdqjudy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cdt.daxiang520.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qov.havefunace.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zmk.gogol.net.cn

[J05] 时间加减（加 7 天）
来源：http://oqg.fehbvm.com

Py:   now + timedelta(days=7)
来源：http://ayz.jqgfzy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://att.tanke756.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zof.sjlbkw.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gyz.yfazqb.com

Java: LocalDate.now().plusDays(7)
来源：http://yly.uphjek.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bht.xylfe.cn

Ruby: Time.now + 7 * 86400
来源：http://hbc.pengpengdd.cyou

C#:   DateTime.Now.AddDays(7)
来源：http://wnc.ivvv.top

[J06] 计算两时间之差
来源：http://ees.snrcjt.cn

Py:   (end - start).total_seconds()
来源：http://hfn.pengpengdd.cyou

PHP:  $end->diff($start)->days;
来源：http://tym.ybcxt.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tty.gotoacloud.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hds.fzhhl.top

Java: Duration.between(start, end).toSeconds()
来源：http://aka.aizwys.cn

Go:   end.Sub(start).Hours()
来源：http://yii.chenjidiqi.icu

Ruby: end - start                 # 返回秒数
来源：http://jgi.fanxiaobao.xyz

C#:   (end - start).TotalSeconds
来源：http://xit.gaohongyu789.top

[J07] 比较两个日期
来源：http://gmi.yanxiufei.cn

Py:   d1 < d2;  d1 == d2
来源：http://mjm.gotoacloud.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lus.ydzc1.top

JS:   d1.getTime() < d2.getTime()
来源：http://lui.daria6918.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fyc.yongpay.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vfa.zhijiandao.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xuo.yuanzhike.top

Ruby: d1 < d2;  d1 == d2
来源：http://cbq.0kj1m.cn

C#:   d1 < d2;  d1 == d2
来源：http://ctt.ehwqpu.com

[J08] 提取年月日与星期
来源：http://gxr.yvedp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rcj.cheryme.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://beh.svipenyu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kqg.kuanghao11.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jeu.hnqzz.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sph.quarkkingdee.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xkp.cheryme.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zxj.epnwcf.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lui.fengsongda.top

[J09] 时区处理
来源：http://vex.cashguo.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wbz.yj20258.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pnd.316326.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wvo.snrcjt.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zqo.shanyushiyangtech.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lzf.jlsjyb.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://haj.shanyushiyangtech.top

Ruby: Time.now.getlocal("+08:00")
来源：http://hgk.cucudq.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hqe.jinqigfzy.top

[J10] 取今天 / 本月第一天
来源：http://yji.yueranfly.top

Py:   date.today();  date.today().replace(day=1)
来源：http://sqd.ctjpmb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xbe.feifeiyinyue.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pno.cheryme.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wvk.bjfxy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://oqa.hysaishi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yup.xuanzx.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mtu.chenjidiqi.icu

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zmv.vqdsnc.cn

================================================================================
来源：http://rjm.svipenyu.cn

K. JSON 与序列化
来源：http://zcd.yongpay.top

================================================================================
来源：http://ebh.guowangkeji.top

[K01] 对象转 JSON 字符串
来源：http://byp.9152youxi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yhn.sxryk.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hho.fzhhl.top

JS:   JSON.stringify(obj)
来源：http://kxr.hfpthk.cn

TS:   JSON.stringify(obj)
来源：http://ggj.hcnkem.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dzl.yonumen.top

Go:   json.Marshal(obj)
来源：http://onp.zhongyouzk.top

Ruby: obj.to_json                                     // require "json"
来源：http://ttf.yongpay.top

C#:   JsonSerializer.Serialize(obj)
来源：http://hwp.xingfuxueyuan.xyz

[K02] JSON 字符串转对象
来源：http://atu.daria6918.cn

Py:   json.loads(s)
来源：http://wwq.jyoumei.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nxv.tian-w.cn

JS:   JSON.parse(s)
来源：http://lvj.quarkkingdee.top

TS:   JSON.parse(s)
来源：http://hfw.gogol.net.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jqe.zhixingplan.top

Go:   json.Unmarshal(data, &v)
来源：http://bys.guannengcc.top

Ruby: JSON.parse(s)
来源：http://usl.wangdashe.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dxz.ybcxt.top

[K03] JSON 美化输出（带缩进）
来源：http://vjq.guowangkeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wfe.gotoacloud.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://coj.guannengcc.top

JS:   JSON.stringify(obj, null, 2)
来源：http://zbr.ydjk.org.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vsn.nanxinkj.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jse.pengpengdd.cyou

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rpz.yj20258888.top

Ruby: JSON.pretty_generate(obj)
来源：http://nte.zdbjq.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sgt.andypj.xyz

[K04] 读取 JSON 文件
来源：http://ehi.zhoulong.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mkm.hcnkem.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wdt.zhengqikj.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qvp.zhengqikj.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bhi.zhixingplan.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bxf.fzhhl.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rwk.chenlongwang.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://coo.guowangkeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fbv.fengsongda.top

[K05] 深拷贝对象
来源：http://jxr.nanxinkj.top

Py:   copy.deepcopy(obj)
来源：http://vsw.cashguo.top

PHP:  unserialize(serialize($obj));
来源：http://nyu.andypj.xyz

JS:   structuredClone(obj)
来源：http://kwc.zdqjudy.top

TS:   structuredClone(obj)
来源：http://ydg.gogol.net.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gdx.tian-w.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lmu.guannengcc.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://toj.zhongyouzk.top

C#:   // 序列化往返，或自定义 Clone
来源：http://yjd.kuanghao11.cn

[K06] 解析 URL 查询串
来源：http://xht.zhijiandao.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dlb.sjlbkw.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fzw.hesvh.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uqp.haohaochexian.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dix.hcnkem.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dhl.hfpthk.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://kxl.iojbl.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fzn.chenjidiqi.icu

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qdo.fzhhl.top

[K07] 进制转换
来源：http://alz.jqgufenzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://exp.ywan-chungtsiang.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jyv.jinghuilouyu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qww.9152youxi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gxc.smart0.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zcx.jqgfzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zna.ydjk.org.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tec.hywenlv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xbj.yangfankeji.com

[K08] 二进制序列化（非 JSON）
来源：http://mmm.pengpengdd.cyou

Py:   pickle.dumps(obj)
来源：http://sqm.cdnleiting.top

PHP:  serialize($obj);  unserialize($s);
来源：http://opw.cqqwz.cn

JS:   v8.serialize(obj)        // Node
来源：http://atz.dashuyun.cn

TS:   v8.serialize(obj)        // Node
来源：http://bbl.yonumen.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jrb.daxiang520.top

Go:   encoding/gob
来源：http://exv.yfazqb.com

Ruby: Marshal.dump(obj)
来源：http://cfd.tianlin.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ttu.shangyingyoupin.top

================================================================================
来源：http://kbz.yj20258888.top

L. 网络请求
来源：http://obr.snrcjt.cn

================================================================================
来源：http://gww.daria6918.cn

[L01] 发送 GET 请求
来源：http://jai.fktsv.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://aov.uphjek.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nks.iojbl.cn

JS:   await fetch(url)
来源：http://mjw.zhengqikj.top

TS:   await fetch(url)
来源：http://fsz.ivvv.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zsa.vehdjk.com

Go:   resp, err := http.Get(url)
来源：http://wdf.sysykeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://uuk.jinyuanbaomall.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wtn.epnwcf.com

[L02] 发送 POST JSON
来源：http://mac.aibaodan.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gze.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ycm.pycfn.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://znh.hfpthk.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aeh.hammf.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zen.nanxuanxn.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mmu.yangfankeji.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lfq.hongshengwenyu.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hbz.ybcxt.top

[L03] 设置自定义请求头
来源：http://dtr.tian-w.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wvf.sweek.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xgr.ctjpmb.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hxt.cqqwz.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vxw.pycfn.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kha.hywenlv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qdn.ybcxt.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zjh.xziqi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cva.hongshengwenyu.top

[L04] 设置超时
来源：http://doa.quarkkingdee.top

Py:   requests.get(url, timeout=5)
来源：http://wnl.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mvv.fktsv.cn


<!-- 参考信息 -->