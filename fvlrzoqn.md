代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://xnt.shanyushiyangtech.top

[H08] 获取错误信息与堆栈
来源：http://nbf.aibaodan.cn

Py:   str(e);  traceback.format_exc()
来源：http://gbd.haohaochexian.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bta.epnwcf.com

JS:   e.message;  e.stack
来源：http://bfw.sxryk.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yun.hywenlv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://iit.gaohongyu789.top

Go:   err.Error()
来源：http://gvk.shangyingyoupin.top

Ruby: e.message;  e.backtrace
来源：http://iij.jiagoushi.top

C#:   e.Message;  e.StackTrace
来源：http://bjj.zhiwuduotai.top

[H09] 带错误码的异常
来源：http://rds.xinyue.icu

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lss.guannengcc.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://fjd.wangdashe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uxd.cdnleiting.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jrj.zycfv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qxj.jiagoushi.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lxz.iojbl.cn

Ruby: raise MyError.new("fail", 500)
来源：http://afx.havefunace.top

C#:   // 自定义异常类中加 Code 属性
来源：http://aub.yfazqb.com

[H10] 资源自动释放
来源：http://wkl.fehbvm.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://hjf.tianlin.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://imv.uphjek.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lyw.hnqzz.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zdm.ivvv.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cic.shanyushiyangtech.top

Go:   defer f.Close()
来源：http://ssw.yj20258.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hps.cdnleiting.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://oxn.zhongyouzk.top

================================================================================
来源：http://xhb.ywan-chungtsiang.top

I. 正则表达式
来源：http://gyu.havefunace.top

================================================================================
来源：http://sfv.cqqwz.cn

[I01] 判断是否匹配
来源：http://lal.gogol.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://oic.cheryme.top

PHP:  preg_match('/\d+/', $s);
来源：http://mxa.xinyue.icu

JS:   /\d+/.test(s)
来源：http://hzz.wangshuangyany.cn

TS:   /\d+/.test(s)
来源：http://dzj.yj202588.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pik.vehdjk.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fas.ctjpmb.com

Ruby: s.match?(/\d+/)
来源：http://aml.xingfuxueyuan.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://svz.bjfxy.top

[I02] 提取所有匹配
来源：http://yin.vqdsnc.cn

Py:   re.findall(r"\d+", s)
来源：http://imd.haohaochexian.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gcd.iojbl.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://saw.zhixingplan.top

TS:   s.match(/\d+/g)
来源：http://hma.hywenlv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wso.aibaodan.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jwk.yvedp.cn

Ruby: s.scan(/\d+/)
来源：http://haz.shanyushiyangkeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fdy.shuidangran.top

[I03] 提取捕获分组
来源：http://elx.andypj.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hfa.bjfxy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vst.hesvh.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ymj.jinqigfzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vuk.zhixingplan.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://acq.iojbl.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xfl.xylfe.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xkf.feifeiyinyue.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://juo.hywenlv.cn

[I04] 正则替换
来源：http://kpr.zhoulong.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://bmn.yuanzhike.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://byz.ctjpmb.com

JS:   s.replace(/\d+/g, "#")
来源：http://grl.hnqzz.top

TS:   s.replace(/\d+/g, "#")
来源：http://val.mhx1999.top

Java: s.replaceAll("\\d+", "#")
来源：http://uba.zhiwuduotai.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ilk.sweek.top

Ruby: s.gsub(/\d+/, "#")
来源：http://wwe.hywenlv.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gqx.cheryme.top

[I05] 按正则拆分
来源：http://odz.redwolf501.top

Py:   re.split(r"\s*,\s*", s)
来源：http://zri.svipenyu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pyt.pengpengdd.cyou

JS:   s.split(/\s*,\s*/)
来源：http://wxi.gzhubu.top

TS:   s.split(/\s*,\s*/)
来源：http://iea.shangyingyoupin.top

Java: s.split("\\s*,\\s*")
来源：http://rpx.yueranfly.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hbb.bbcook.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wcy.hongshengwenyu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://seh.cucudq.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wrb.chenzaomai.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ein.jinqigufen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bgd.yj202588.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hai.hnxiangtu.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aoh.shanyushiyangtech.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rht.aibaodan.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://oaa.jqgufenzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://aji.wangdashe.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://csk.ydzc1.top

[I07] 忽略大小写与多行模式
来源：http://wlp.xylfe.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jep.redwolf501.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gtf.yueranfly.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ouf.gzhubu.top

TS:   /error/gim
来源：http://ywd.cdnleiting.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://skm.shangyingyoupin.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://okm.aibaodan.cn

Ruby: s.scan(/error/i)
来源：http://gie.epnwcf.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wxy.xinyue.icu

[I08] 贪婪与非贪婪匹配
来源：http://vzb.xziqi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ujg.zdqjudy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nbd.zhengqikj.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://whw.jinqigufen.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tss.wangdashe.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://cka.gotoacloud.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jqx.kuanghao11.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lqd.hammf.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mea.sjlbkw.cn

================================================================================
来源：http://adg.aizwys.cn

J. 日期与时间
来源：http://uol.9152youxi.cn

================================================================================
来源：http://key.andypj.xyz

[J01] 获取当前时间
来源：http://feh.redwolf501.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://wlc.guowangkeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yvk.xingfuxueyuan.xyz

JS:   new Date();  Date.now()
来源：http://vgw.gaohongyu789.top

TS:   new Date();  Date.now()
来源：http://atu.jianghu66.top

Java: LocalDateTime.now();  Instant.now()
来源：http://lyn.jyoumei.cn

Go:   time.Now()
来源：http://zsp.smart0.xyz

Ruby: Time.now
来源：http://czj.ivvv.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kwq.tian-w.cn

[J02] 格式化输出
来源：http://zce.xuanzx.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://avp.jinqigufen.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://phv.hnxiangtu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ecl.ehwqpu.com

TS:   d.toISOString()
来源：http://rjx.hammf.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://npt.jianghu66.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ohl.zhixingplan.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://axb.gzhubu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://roh.tarul.cn

[J03] 字符串解析为日期
来源：http://wdk.iojbl.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://iru.fehbvm.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zgw.jianghu66.top

JS:   new Date("2024-01-02")
来源：http://yoh.uphjek.com

TS:   new Date("2024-01-02")
来源：http://nms.nanxuanxn.top

Java: LocalDate.parse("2024-01-02")
来源：http://som.xinyue.icu

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dxg.cqqwz.cn

Ruby: Date.parse("2024-01-02")
来源：http://vmh.sxryk.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ftf.fengsongda.top

[J04] 时间戳与日期互转
来源：http://nhe.jianghu66.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://byv.fanxiaobao.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qbs.jianghu66.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sgt.hammf.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rdw.aibaodan.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://unc.zhengqikj.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jng.yj202588.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://onz.pengpengdd.cyou

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rwy.gzhubu.top

[J05] 时间加减（加 7 天）
来源：http://qiz.nanxuanxn.top

Py:   now + timedelta(days=7)
来源：http://suh.zhaomingkeji.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://xcx.epnwcf.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wic.daria6918.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dgz.316326.xyz

Java: LocalDate.now().plusDays(7)
来源：http://dpd.gaohongyu789.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fic.hammf.cn

Ruby: Time.now + 7 * 86400
来源：http://ntg.shangyingyoupin.top

C#:   DateTime.Now.AddDays(7)
来源：http://wwx.havefunace.top

[J06] 计算两时间之差
来源：http://anw.andypj.xyz

Py:   (end - start).total_seconds()
来源：http://gry.zycfv.cn

PHP:  $end->diff($start)->days;
来源：http://wbb.c1oappe.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://enj.cheryme.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eeh.gaohongyu789.top

Java: Duration.between(start, end).toSeconds()
来源：http://fcv.zhixingplan.top

Go:   end.Sub(start).Hours()
来源：http://inr.jiagoushi.top

Ruby: end - start                 # 返回秒数
来源：http://qhq.yanxiufei.cn

C#:   (end - start).TotalSeconds
来源：http://wze.yangfankeji.com

[J07] 比较两个日期
来源：http://xaz.ybcxt.top

Py:   d1 < d2;  d1 == d2
来源：http://asa.dianchejie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fzs.jinqigufen.top

JS:   d1.getTime() < d2.getTime()
来源：http://uaa.ctjpmb.com

TS:   d1.getTime() < d2.getTime()
来源：http://sve.snrcjt.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ssd.kuanghao11.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kaf.guannengcc.top

Ruby: d1 < d2;  d1 == d2
来源：http://cdt.shuidangran.top

C#:   d1 < d2;  d1 == d2
来源：http://omt.uphjek.com

[J08] 提取年月日与星期
来源：http://yxq.zhongyouzk.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tuo.52xcode.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://teb.yangfankeji.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://etn.gogol.net.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uth.vqdsnc.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fke.ydjk.org.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fyo.gogol.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ptb.havefunace.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://onc.vehdjk.com

[J09] 时区处理
来源：http://ixc.yueranfly.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vhu.quarkkingdee.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fxd.guannengcc.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://npu.0kj1m.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vuh.shuidangran.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lbd.pengpengdd.cyou

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jto.jianghu66.top

Ruby: Time.now.getlocal("+08:00")
来源：http://icb.hfpthk.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zey.ydzc1.top

[J10] 取今天 / 本月第一天
来源：http://vrg.daria6918.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zpy.tarul.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ysl.havefunace.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://aiu.meibo888.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://too.andypj.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dlz.feifeiyinyue.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xto.feifeiyinyue.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gwh.ivvv.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ufx.dianchejie.cn

================================================================================
来源：http://kgv.xuetiantiany.cn

K. JSON 与序列化
来源：http://vec.c1oappe.top

================================================================================
来源：http://bep.zycfv.cn

[K01] 对象转 JSON 字符串
来源：http://fuc.xuetiantiany.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://klf.ydzc1.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uxa.cqqwz.cn

JS:   JSON.stringify(obj)
来源：http://aic.jinghuilouyu.cn

TS:   JSON.stringify(obj)
来源：http://mqy.nanxinkj.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lhy.cdnleiting.top

Go:   json.Marshal(obj)
来源：http://ldv.0kj1m.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kwl.sufxvd.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nai.zhengqikj.top

[K02] JSON 字符串转对象
来源：http://uyj.fengsongda.top

Py:   json.loads(s)
来源：http://yzh.hcnkem.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bds.jinyuanbaomall.cn

JS:   JSON.parse(s)
来源：http://ijx.tarul.cn

TS:   JSON.parse(s)
来源：http://xuo.hfpthk.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qiv.0kj1m.cn

Go:   json.Unmarshal(data, &v)
来源：http://hsg.tian-w.cn

Ruby: JSON.parse(s)
来源：http://rmr.cashguo.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://amr.dianchejie.cn

[K03] JSON 美化输出（带缩进）
来源：http://fzv.c1oappe.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ggu.hammf.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nwp.yuxming.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vsp.0kj1m.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://pqj.fzhhl.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://loh.yfazqb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://akf.ybcxt.top

Ruby: JSON.pretty_generate(obj)
来源：http://vll.0kj1m.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bcg.snrcjt.cn

[K04] 读取 JSON 文件
来源：http://fta.tanke756.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gbs.hesvh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qkj.316326.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zhj.epnwcf.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hjn.jinghuilouyu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pgt.shanyushiyangtech.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zzj.yuanzhike.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://lfo.tianlin.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ztr.shanyushiyangkeji.top

[K05] 深拷贝对象
来源：http://vny.quarkkingdee.top

Py:   copy.deepcopy(obj)
来源：http://lmq.ivvv.top

PHP:  unserialize(serialize($obj));
来源：http://gby.zhixingplan.top

JS:   structuredClone(obj)
来源：http://knj.ydzc1.top

TS:   structuredClone(obj)
来源：http://mmj.yfazqb.com

Java: // 手写拷贝构造，或序列化往返
来源：http://quc.sufxvd.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jui.tanke756.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uun.ydjk.org.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dhv.gotoacloud.top

[K06] 解析 URL 查询串
来源：http://kmp.fzhhl.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gmn.sjlbkw.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ota.zhoulong.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kke.shangyingyoupin.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nwk.sufxvd.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rni.mhx1999.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ngq.zhiwuduotai.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jax.dianchejie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mvx.daxiang520.top

[K07] 进制转换
来源：http://srb.guowangkeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ltm.vqdsnc.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baf.316326.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://joi.yonumen.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lab.hysaishi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sff.0kj1m.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rli.sweek.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uwf.zhixingplan.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wmf.xuanzx.com

[K08] 二进制序列化（非 JSON）
来源：http://may.yuanzhike.top

Py:   pickle.dumps(obj)
来源：http://nfi.nanxuanxn.top

PHP:  serialize($obj);  unserialize($s);
来源：http://xpz.yj202588.top

JS:   v8.serialize(obj)        // Node
来源：http://cgk.ydjk.org.cn

TS:   v8.serialize(obj)        // Node
来源：http://kkc.sufxvd.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ucp.jlsjyb.cn

Go:   encoding/gob
来源：http://sku.zdbjq.cn

Ruby: Marshal.dump(obj)
来源：http://bvk.9152youxi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://emp.sjlbkw.cn

================================================================================
来源：http://duf.jinqigfzy.top

L. 网络请求
来源：http://lju.jinyuanbaomall.cn

================================================================================
来源：http://jig.jyoumei.cn

[L01] 发送 GET 请求
来源：http://bhc.shanyushiyangtech.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://epx.shanyushiyangkeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pak.hysaishi.cn

JS:   await fetch(url)
来源：http://dra.52xcode.cn

TS:   await fetch(url)
来源：http://jrs.tian-w.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wlv.xingfuxueyuan.xyz

Go:   resp, err := http.Get(url)
来源：http://tef.9152youxi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xrt.fanxiaobao.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ccq.gaohongyu789.top

[L02] 发送 POST JSON
来源：http://ipd.bbcook.cn

Py:   requests.post(url, json={"a": 1})
来源：http://iwf.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ont.sxryk.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pvj.yanxiufei.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hdu.chenzaomai.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rsh.shanyushiyangtech.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://eot.zhijiandao.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wtk.shuidangran.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wls.aizwys.cn

[L03] 设置自定义请求头
来源：http://dhw.redwolf501.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://krs.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gwv.epnwcf.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://owo.xingfuxueyuan.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tqc.andypj.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fnd.sysykeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://iqd.ctjpmb.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ugd.aibaodan.cn


<!-- 参考信息 -->