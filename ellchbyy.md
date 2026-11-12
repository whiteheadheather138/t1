代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://rhe.yfazqb.com

C#:   e.Message;  e.StackTrace
来源：http://lgv.andypj.xyz

[H09] 带错误码的异常
来源：http://wbw.meibo888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qix.ivvv.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://pci.jinqigufen.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fno.xylfe.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://uuf.yuanzhike.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mxa.epnwcf.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ywn.mhx1999.top

Ruby: raise MyError.new("fail", 500)
来源：http://fgm.pycfn.com

C#:   // 自定义异常类中加 Code 属性
来源：http://ppg.yangfankeji.com

[H10] 资源自动释放
来源：http://gkk.daria6918.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lyj.ehwqpu.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mrv.hfpthk.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://naz.zdqjudy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xwc.daria6918.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://aww.haohaochexian.top

Go:   defer f.Close()
来源：http://trm.chenlongwang.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ygx.yuxming.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xkh.tian-w.cn

================================================================================
来源：http://tfc.zhengqikj.top

I. 正则表达式
来源：http://wzz.ybcxt.top

================================================================================
来源：http://hkj.wangdashe.top

[I01] 判断是否匹配
来源：http://yfz.yj20258.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://meb.daxiang520.top

PHP:  preg_match('/\d+/', $s);
来源：http://pvd.hnxiangtu.top

JS:   /\d+/.test(s)
来源：http://xlf.cdnleiting.top

TS:   /\d+/.test(s)
来源：http://tsn.chenzaomai.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://saz.yj20258.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ihp.yangfankeji.com

Ruby: s.match?(/\d+/)
来源：http://ezg.chenjidiqi.icu

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hrh.shanyushiyangkeji.top

[I02] 提取所有匹配
来源：http://kue.andypj.xyz

Py:   re.findall(r"\d+", s)
来源：http://alj.shanyushiyangtech.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kst.smart0.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ssj.316326.xyz

TS:   s.match(/\d+/g)
来源：http://uih.chenjidiqi.icu

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://orr.shanyushiyangtech.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ywc.hywenlv.cn

Ruby: s.scan(/\d+/)
来源：http://unu.epnwcf.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tit.cdnleiting.top

[I03] 提取捕获分组
来源：http://myy.cheryme.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://clq.yongpay.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://itt.nanxinkj.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yjh.svipenyu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://awm.kuanghao11.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qlu.xingfuxueyuan.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://myl.fehbvm.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xzs.xuanzx.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://age.zhixingplan.top

[I04] 正则替换
来源：http://apm.smart0.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://kuz.xingfuxueyuan.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qii.jqgfzy.top

JS:   s.replace(/\d+/g, "#")
来源：http://cso.cucudq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vkw.ydjk.org.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hbt.316326.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://tet.jinqigfzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ltu.daria6918.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bqn.fzhhl.top

[I05] 按正则拆分
来源：http://uyd.epnwcf.com

Py:   re.split(r"\s*,\s*", s)
来源：http://att.jinqigfzy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lyq.fehbvm.com

JS:   s.split(/\s*,\s*/)
来源：http://ufk.quarkkingdee.top

TS:   s.split(/\s*,\s*/)
来源：http://ymp.vqdsnc.cn

Java: s.split("\\s*,\\s*")
来源：http://srq.guowangkeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lub.sjlbkw.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ybv.jqgufenzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jci.wangshuangyany.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://upm.yvedp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zdt.tianlin.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mlt.xuetiantiany.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://erp.cucudq.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xzc.xuetiantiany.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uow.cqqwz.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://abe.nanxuanxn.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cwm.yanxiufei.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://epv.yfazqb.com

[I07] 忽略大小写与多行模式
来源：http://cwo.fengsongda.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://poo.jqgufenzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://seb.sjlbkw.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ngq.ydjk.org.cn

TS:   /error/gim
来源：http://hjn.yonumen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qwn.sweek.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wdw.nwbrower.top

Ruby: s.scan(/error/i)
来源：http://uxy.fehbvm.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tiq.nwbrower.top

[I08] 贪婪与非贪婪匹配
来源：http://xvg.sufxvd.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ywj.nwbrower.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tej.sufxvd.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lsg.zycfv.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cnt.tarul.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zym.zhengqikj.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lpd.zhengqikj.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://anp.zdbjq.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tct.quarkkingdee.top

================================================================================
来源：http://bvt.shanyushiyangtech.top

J. 日期与时间
来源：http://usl.xuanzx.com

================================================================================
来源：http://ahw.birdmap.top

[J01] 获取当前时间
来源：http://dio.jqgfzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://kfl.cdnleiting.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kbp.jlsjyb.cn

JS:   new Date();  Date.now()
来源：http://iak.jinqigfzy.top

TS:   new Date();  Date.now()
来源：http://taj.0kj1m.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vyj.bjfxy.top

Go:   time.Now()
来源：http://frx.vehdjk.com

Ruby: Time.now
来源：http://ppm.snrcjt.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rzb.yongpay.top

[J02] 格式化输出
来源：http://unj.dianchejie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://igx.jqgfzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mee.sxryk.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uav.ppjwa.cn

TS:   d.toISOString()
来源：http://pbg.hfpthk.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mjk.nanxuanxn.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://iov.sweek.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wuz.chenlongwang.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ijm.ivvv.top

[J03] 字符串解析为日期
来源：http://ytf.sweek.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://luu.ydzc1.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ohe.jqgfzy.top

JS:   new Date("2024-01-02")
来源：http://ncv.fzhhl.top

TS:   new Date("2024-01-02")
来源：http://cvn.xuanzx.com

Java: LocalDate.parse("2024-01-02")
来源：http://nbo.xuanzx.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cfb.feifeiyinyue.top

Ruby: Date.parse("2024-01-02")
来源：http://hcr.ybcxt.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yue.andypj.xyz

[J04] 时间戳与日期互转
来源：http://npz.fzhhl.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pup.zycfv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nko.zhengqikj.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ief.yueranfly.top

TS:   Math.floor(Date.now() / 1000)
来源：http://xie.iojbl.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xdd.shanyushiyangtech.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://byt.svipenyu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jep.sysykeji.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xlz.aibaodan.cn

[J05] 时间加减（加 7 天）
来源：http://onh.pengpengdd.cyou

Py:   now + timedelta(days=7)
来源：http://mou.zhoulong.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://mlw.sweek.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jeu.nanxuanxn.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uln.jinqigufen.top

Java: LocalDate.now().plusDays(7)
来源：http://kvr.hcnkem.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jmt.ydzc1.top

Ruby: Time.now + 7 * 86400
来源：http://axo.zdqjudy.top

C#:   DateTime.Now.AddDays(7)
来源：http://hva.nwbrower.top

[J06] 计算两时间之差
来源：http://bre.jinqigfzy.top

Py:   (end - start).total_seconds()
来源：http://rme.mhx1999.top

PHP:  $end->diff($start)->days;
来源：http://shj.zhengqikj.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://exu.jiagoushi.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qft.smart0.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://jra.vehdjk.com

Go:   end.Sub(start).Hours()
来源：http://ypd.hesvh.cn

Ruby: end - start                 # 返回秒数
来源：http://mxd.jinyuanbaomall.cn

C#:   (end - start).TotalSeconds
来源：http://vvs.cashguo.top

[J07] 比较两个日期
来源：http://msi.dashuyun.cn

Py:   d1 < d2;  d1 == d2
来源：http://vie.hnxiangtu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fnv.ctjpmb.com

JS:   d1.getTime() < d2.getTime()
来源：http://swo.zhengqikj.top

TS:   d1.getTime() < d2.getTime()
来源：http://kpm.dianchejie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rye.meibo888.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uxa.redwolf501.top

Ruby: d1 < d2;  d1 == d2
来源：http://ymy.daria6918.cn

C#:   d1 < d2;  d1 == d2
来源：http://wym.chenzaomai.com

[J08] 提取年月日与星期
来源：http://qgb.hysaishi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://iux.jinqigufen.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oij.shuidangran.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://noz.316326.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://isx.shanyushiyangkeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bbi.sjlbkw.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gvc.sxryk.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fsi.nwbrower.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gzu.ehwqpu.com

[J09] 时区处理
来源：http://mgg.hammf.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zrq.jiagoushi.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vcb.ctjpmb.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sje.chenjidiqi.icu

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bha.shzxlz.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dgq.ydjk.org.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jrj.yueranfly.top

Ruby: Time.now.getlocal("+08:00")
来源：http://dgc.cucudq.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ozg.xingfuxueyuan.xyz

[J10] 取今天 / 本月第一天
来源：http://rfd.vqdsnc.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://yat.hongshengwenyu.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ctw.gzhubu.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ibf.zhiwuduotai.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://btp.ehwqpu.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ilp.yj20258888.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jak.yj20258.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tom.zhiwuduotai.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xak.jinyuanbaomall.cn

================================================================================
来源：http://hxx.ydjk.org.cn

K. JSON 与序列化
来源：http://azt.yongpay.top

================================================================================
来源：http://ubk.gogol.net.cn

[K01] 对象转 JSON 字符串
来源：http://qdc.yuxming.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zeu.zhixingplan.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oph.svipenyu.cn

JS:   JSON.stringify(obj)
来源：http://goo.zdqjudy.top

TS:   JSON.stringify(obj)
来源：http://qcj.gotoacloud.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cyg.cheryme.top

Go:   json.Marshal(obj)
来源：http://bru.jinqigufen.top

Ruby: obj.to_json                                     // require "json"
来源：http://bsr.kuanghao11.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://efm.andypj.xyz

[K02] JSON 字符串转对象
来源：http://efc.zhaomingkeji.xyz

Py:   json.loads(s)
来源：http://bal.iojbl.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ada.yfazqb.com

JS:   JSON.parse(s)
来源：http://chn.hysaishi.cn

TS:   JSON.parse(s)
来源：http://pwj.hcnkem.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rwp.meibo888.top

Go:   json.Unmarshal(data, &v)
来源：http://vzf.cheryme.top

Ruby: JSON.parse(s)
来源：http://vnr.ehwqpu.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zui.chenlongwang.top

[K03] JSON 美化输出（带缩进）
来源：http://msk.snrcjt.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kny.mhx1999.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bqw.cdnleiting.top

JS:   JSON.stringify(obj, null, 2)
来源：http://oud.fengsongda.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ihk.jinyuanbaomall.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qbe.yonumen.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://euh.cqqwz.cn

Ruby: JSON.pretty_generate(obj)
来源：http://izw.zhijiandao.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ldf.sjlbkw.cn

[K04] 读取 JSON 文件
来源：http://sxh.yanxiufei.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://apy.zhixingplan.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bkf.sjlbkw.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gkk.shanyushiyangtech.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jjk.hammf.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xng.kuanghao11.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uue.zhijiandao.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://nsw.epnwcf.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lwi.tianlin.xyz

[K05] 深拷贝对象
来源：http://ovl.yj20258888.top

Py:   copy.deepcopy(obj)
来源：http://lop.jianghu66.top

PHP:  unserialize(serialize($obj));
来源：http://nsc.aizwys.cn

JS:   structuredClone(obj)
来源：http://qos.guannengcc.top

TS:   structuredClone(obj)
来源：http://eio.aibaodan.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kmo.cheryme.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yjj.0kj1m.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sbh.sufxvd.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mha.yongpay.top

[K06] 解析 URL 查询串
来源：http://cwn.daxiang520.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://eub.chenjidiqi.icu

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dos.jlsjyb.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pws.ppjwa.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://etd.9152youxi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bfl.havefunace.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://kkb.vehdjk.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hkr.ydzc1.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wis.chenzaomai.com

[K07] 进制转换
来源：http://ocg.gotoacloud.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pft.jqgfzy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hiw.yvedp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qqg.haohaochexian.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lfi.havefunace.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wvn.chenlongwang.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mof.jqgufenzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qkr.birdmap.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mdw.dashuyun.cn

[K08] 二进制序列化（非 JSON）
来源：http://gjs.shangyingyoupin.top

Py:   pickle.dumps(obj)
来源：http://bff.gzhubu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://fys.mhx1999.top

JS:   v8.serialize(obj)        // Node
来源：http://pns.gogol.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://tfo.jiagoushi.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://alw.meibo888.top

Go:   encoding/gob
来源：http://tbu.wangdashe.top

Ruby: Marshal.dump(obj)
来源：http://hij.ywan-chungtsiang.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vxt.redwolf501.top

================================================================================
来源：http://lxb.shzxlz.cn

L. 网络请求
来源：http://upe.snrcjt.cn

================================================================================
来源：http://yym.xuetiantiany.cn

[L01] 发送 GET 请求
来源：http://keo.hnqzz.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://iih.hnqzz.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://put.cucudq.cn

JS:   await fetch(url)
来源：http://nuz.pengpengdd.cyou

TS:   await fetch(url)
来源：http://ajm.aibaodan.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wkc.zhoulong.xyz

Go:   resp, err := http.Get(url)
来源：http://hmm.nwbrower.top

Ruby: Net::HTTP.get(URI(url))
来源：http://lcy.shuidangran.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qpo.cucudq.cn

[L02] 发送 POST JSON
来源：http://isy.bbcook.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hae.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lmn.jinqigfzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kzs.zhixingplan.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wqm.sysykeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gpn.wangshuangyany.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zwn.sweek.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uxx.shanyushiyangtech.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yma.quarkkingdee.top

[L03] 设置自定义请求头
来源：http://wcb.vehdjk.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xpb.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://foh.fktsv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qgg.iojbl.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nud.cdnleiting.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://iyi.xuanzx.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qvy.havefunace.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tdb.quarkkingdee.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kqa.nanxuanxn.top

[L04] 设置超时
来源：http://fzr.0kj1m.cn

Py:   requests.get(url, timeout=5)
来源：http://gxd.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lig.wangdashe.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ffh.fanxiaobao.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ozd.hcnkem.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xim.yonumen.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://txq.xylfe.cn


<!-- 参考信息 -->