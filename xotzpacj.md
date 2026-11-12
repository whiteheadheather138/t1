代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://dir.hesvh.cn

[H08] 获取错误信息与堆栈
来源：http://noz.fehbvm.com

Py:   str(e);  traceback.format_exc()
来源：http://jys.fanxiaobao.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://iqm.jinqigfzy.top

JS:   e.message;  e.stack
来源：http://dzi.fengsongda.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://jfy.hongshengwenyu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://vxc.xuetiantiany.cn

Go:   err.Error()
来源：http://ebe.ivvv.top

Ruby: e.message;  e.backtrace
来源：http://muz.shangyingyoupin.top

C#:   e.Message;  e.StackTrace
来源：http://tbk.hesvh.cn

[H09] 带错误码的异常
来源：http://wly.hysaishi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tvz.epnwcf.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://czq.meibo888.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pdi.guowangkeji.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pdg.yj20258.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gop.birdmap.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dbx.svipenyu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://dwr.xingfuxueyuan.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://csn.yvedp.cn

[H10] 资源自动释放
来源：http://mza.nanxuanxn.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://vme.shzxlz.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hlf.jinqigfzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ulv.vehdjk.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tfb.52xcode.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zjv.andypj.xyz

Go:   defer f.Close()
来源：http://rqo.cqqwz.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mwj.daria6918.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xqz.cqqwz.cn

================================================================================
来源：http://hmf.vehdjk.com

I. 正则表达式
来源：http://qss.xylfe.cn

================================================================================
来源：http://gof.jqgfzy.top

[I01] 判断是否匹配
来源：http://rtp.shangyingyoupin.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gao.hfpthk.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ynj.uphjek.com

JS:   /\d+/.test(s)
来源：http://woe.shzxlz.cn

TS:   /\d+/.test(s)
来源：http://dex.fktsv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jce.yangfankeji.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gly.zdbjq.cn

Ruby: s.match?(/\d+/)
来源：http://cva.hammf.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qsm.316326.xyz

[I02] 提取所有匹配
来源：http://vmc.hnxiangtu.top

Py:   re.findall(r"\d+", s)
来源：http://gsu.jqgfzy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ajt.sufxvd.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://uhz.zdqjudy.top

TS:   s.match(/\d+/g)
来源：http://ijz.ydjk.org.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ifi.kuanghao11.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uzj.fehbvm.com

Ruby: s.scan(/\d+/)
来源：http://ydc.fengsongda.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://drz.jqgufenzy.top

[I03] 提取捕获分组
来源：http://zse.guannengcc.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://don.jinqigufen.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yig.tian-w.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tdm.bjfxy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wbp.chenlongwang.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nvn.vehdjk.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uxo.jiagoushi.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uiq.meibo888.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mpy.ctjpmb.com

[I04] 正则替换
来源：http://eov.yanxiufei.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qlq.smart0.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wxs.feifeiyinyue.top

JS:   s.replace(/\d+/g, "#")
来源：http://get.jiagoushi.top

TS:   s.replace(/\d+/g, "#")
来源：http://hsn.hesvh.cn

Java: s.replaceAll("\\d+", "#")
来源：http://lfs.yfazqb.com

Go:   re.ReplaceAllString(s, "#")
来源：http://vvj.haohaochexian.top

Ruby: s.gsub(/\d+/, "#")
来源：http://itd.hysaishi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bbb.vqdsnc.cn

[I05] 按正则拆分
来源：http://fif.daxiang520.top

Py:   re.split(r"\s*,\s*", s)
来源：http://zch.andypj.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uvb.jinqigufen.top

JS:   s.split(/\s*,\s*/)
来源：http://xzd.jinqigfzy.top

TS:   s.split(/\s*,\s*/)
来源：http://fbk.9152youxi.cn

Java: s.split("\\s*,\\s*")
来源：http://zjc.tanke756.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://aue.yj202588.top

Ruby: s.split(/\s*,\s*/)
来源：http://dzk.jinqigufen.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://faf.yangfankeji.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hlb.guowangkeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dfg.xuanzx.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hsl.zdbjq.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rtp.sufxvd.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ksi.jyoumei.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kla.chenlongwang.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ari.tanke756.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ugz.zhengqikj.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sgn.wangdashe.top

[I07] 忽略大小写与多行模式
来源：http://cxt.dashuyun.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gio.tarul.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jzi.cashguo.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oyw.9152youxi.cn

TS:   /error/gim
来源：http://ztm.birdmap.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ngp.gaohongyu789.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nzo.yongpay.top

Ruby: s.scan(/error/i)
来源：http://ktk.chenzaomai.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://imx.guowangkeji.top

[I08] 贪婪与非贪婪匹配
来源：http://nlr.ydzc1.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vdv.vehdjk.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pxh.xziqi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gwy.xinyue.icu

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://unn.svipenyu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xuu.xuetiantiany.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cgu.sysykeji.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://skj.fktsv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ngo.aibaodan.cn

================================================================================
来源：http://zgy.gaohongyu789.top

J. 日期与时间
来源：http://eny.0kj1m.cn

================================================================================
来源：http://tdz.aizwys.cn

[J01] 获取当前时间
来源：http://pnv.jinqigfzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://lqn.shzxlz.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jss.hammf.cn

JS:   new Date();  Date.now()
来源：http://ozr.jqgfzy.top

TS:   new Date();  Date.now()
来源：http://pml.yuanzhike.top

Java: LocalDateTime.now();  Instant.now()
来源：http://uif.hnxiangtu.top

Go:   time.Now()
来源：http://ebz.hysaishi.cn

Ruby: Time.now
来源：http://rzu.ywan-chungtsiang.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://iol.hcnkem.com

[J02] 格式化输出
来源：http://ggy.sjlbkw.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mea.hcnkem.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ory.jinqigufen.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ina.snrcjt.cn

TS:   d.toISOString()
来源：http://dwl.xinyue.icu

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rqe.hysaishi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kfd.aizwys.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xiv.0kj1m.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nay.hnxiangtu.top

[J03] 字符串解析为日期
来源：http://pnn.xuanzx.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bbh.c1oappe.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wss.mhx1999.top

JS:   new Date("2024-01-02")
来源：http://hje.0kj1m.cn

TS:   new Date("2024-01-02")
来源：http://hzh.pycfn.com

Java: LocalDate.parse("2024-01-02")
来源：http://rsi.cdnleiting.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yup.chenzaomai.com

Ruby: Date.parse("2024-01-02")
来源：http://khf.cqqwz.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ich.jyoumei.cn

[J04] 时间戳与日期互转
来源：http://rtl.feifeiyinyue.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://znn.ppjwa.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baz.jinqigufen.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ftr.epnwcf.com

TS:   Math.floor(Date.now() / 1000)
来源：http://dzl.ydzc1.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xsv.tanke756.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qgg.tian-w.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://viy.guowangkeji.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hel.ywan-chungtsiang.top

[J05] 时间加减（加 7 天）
来源：http://mna.c1oappe.top

Py:   now + timedelta(days=7)
来源：http://ajs.fehbvm.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://lep.c1oappe.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wuk.ivvv.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vof.ctjpmb.com

Java: LocalDate.now().plusDays(7)
来源：http://dwi.ppjwa.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tlf.hesvh.cn

Ruby: Time.now + 7 * 86400
来源：http://skc.chenjidiqi.icu

C#:   DateTime.Now.AddDays(7)
来源：http://uvz.hywenlv.cn

[J06] 计算两时间之差
来源：http://irx.jinyuanbaomall.cn

Py:   (end - start).total_seconds()
来源：http://mdb.jyoumei.cn

PHP:  $end->diff($start)->days;
来源：http://wpg.chenlongwang.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bvd.yonumen.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ssz.sysykeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://ttd.ehwqpu.com

Go:   end.Sub(start).Hours()
来源：http://tjk.yuxming.cn

Ruby: end - start                 # 返回秒数
来源：http://zkf.svipenyu.cn

C#:   (end - start).TotalSeconds
来源：http://aif.quarkkingdee.top

[J07] 比较两个日期
来源：http://frm.dashuyun.cn

Py:   d1 < d2;  d1 == d2
来源：http://tiw.fehbvm.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xdt.jqgufenzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://hif.chenzaomai.com

TS:   d1.getTime() < d2.getTime()
来源：http://gcp.chenjidiqi.icu

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://itc.aizwys.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ejp.andypj.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://xej.jyoumei.cn

C#:   d1 < d2;  d1 == d2
来源：http://qoh.yuanzhike.top

[J08] 提取年月日与星期
来源：http://nem.vqdsnc.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bqy.316326.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qsc.snrcjt.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xbx.daxiang520.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sbt.aizwys.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wbe.smart0.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qcg.ctjpmb.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zcf.yonumen.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://liy.gotoacloud.top

[J09] 时区处理
来源：http://jqw.jianghu66.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uao.shzxlz.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ize.havefunace.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tro.sufxvd.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zbq.vqdsnc.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qkq.yanxiufei.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mjy.chenjidiqi.icu

Ruby: Time.now.getlocal("+08:00")
来源：http://pwp.vehdjk.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rru.shanyushiyangtech.top

[J10] 取今天 / 本月第一天
来源：http://xsw.tanke756.top

Py:   date.today();  date.today().replace(day=1)
来源：http://wvk.hywenlv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jcy.chenzaomai.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://caq.jinghuilouyu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qdm.meibo888.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kqt.nwbrower.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://piw.zhengqikj.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cvx.uphjek.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jsv.cheryme.top

================================================================================
来源：http://mlg.tarul.cn

K. JSON 与序列化
来源：http://trf.316326.xyz

================================================================================
来源：http://fzg.birdmap.top

[K01] 对象转 JSON 字符串
来源：http://iux.yongpay.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fjb.chenzaomai.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vut.andypj.xyz

JS:   JSON.stringify(obj)
来源：http://apk.cdnleiting.top

TS:   JSON.stringify(obj)
来源：http://yfh.wangshuangyany.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nlk.cashguo.top

Go:   json.Marshal(obj)
来源：http://sfw.jqgfzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://usz.shanyushiyangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://jup.fanxiaobao.xyz

[K02] JSON 字符串转对象
来源：http://whh.xziqi.cn

Py:   json.loads(s)
来源：http://pwk.fehbvm.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ads.jqgufenzy.top

JS:   JSON.parse(s)
来源：http://kxx.sysykeji.top

TS:   JSON.parse(s)
来源：http://ptf.snrcjt.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vky.sjlbkw.cn

Go:   json.Unmarshal(data, &v)
来源：http://ggy.ppjwa.cn

Ruby: JSON.parse(s)
来源：http://icw.52xcode.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uwy.guowangkeji.top

[K03] JSON 美化输出（带缩进）
来源：http://eey.hcnkem.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fta.ybcxt.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yaz.wangshuangyany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dfs.kuanghao11.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://lrs.zhoulong.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://izl.hcnkem.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vku.hysaishi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ooc.chenzaomai.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wqq.cheryme.top

[K04] 读取 JSON 文件
来源：http://mzw.jinqigfzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lzv.bjfxy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rai.smart0.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uwj.nwbrower.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pox.chenlongwang.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lmg.bjfxy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jjx.jqgfzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://gjp.xinyue.icu

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xsg.snrcjt.cn

[K05] 深拷贝对象
来源：http://dcw.jinqigufen.top

Py:   copy.deepcopy(obj)
来源：http://gdv.0kj1m.cn

PHP:  unserialize(serialize($obj));
来源：http://xmk.mhx1999.top

JS:   structuredClone(obj)
来源：http://kow.fzhhl.top

TS:   structuredClone(obj)
来源：http://eft.bjfxy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://run.zdbjq.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gln.tarul.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://eav.yj20258888.top

C#:   // 序列化往返，或自定义 Clone
来源：http://qzy.gzhubu.top

[K06] 解析 URL 查询串
来源：http://oec.sysykeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gsx.sufxvd.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wgl.snrcjt.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xsq.shanyushiyangkeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://knz.iojbl.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bwj.shzxlz.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sxv.havefunace.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jdb.hongshengwenyu.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rgj.yanxiufei.cn

[K07] 进制转换
来源：http://xoj.havefunace.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bzo.shangyingyoupin.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uao.birdmap.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://msf.zhijiandao.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://toc.quarkkingdee.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://elu.cucudq.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lve.tarul.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ybs.xylfe.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uoe.yuanzhike.top

[K08] 二进制序列化（非 JSON）
来源：http://rev.gaohongyu789.top

Py:   pickle.dumps(obj)
来源：http://ykd.sjlbkw.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://olw.shanyushiyangtech.top

JS:   v8.serialize(obj)        // Node
来源：http://nft.hnxiangtu.top

TS:   v8.serialize(obj)        // Node
来源：http://ynl.ppjwa.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ymu.sysykeji.top

Go:   encoding/gob
来源：http://box.yangfankeji.com

Ruby: Marshal.dump(obj)
来源：http://ntb.c1oappe.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bqp.zhiwuduotai.top

================================================================================
来源：http://sor.yangfankeji.com

L. 网络请求
来源：http://lyd.iojbl.cn

================================================================================
来源：http://dlx.sjlbkw.cn

[L01] 发送 GET 请求
来源：http://rbb.smart0.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sjt.cheryme.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cwt.havefunace.top

JS:   await fetch(url)
来源：http://skn.tanke756.top

TS:   await fetch(url)
来源：http://jpn.chenlongwang.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cdj.meibo888.top

Go:   resp, err := http.Get(url)
来源：http://ouu.jianghu66.top

Ruby: Net::HTTP.get(URI(url))
来源：http://woh.jlsjyb.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ovz.chenzaomai.com

[L02] 发送 POST JSON
来源：http://cie.pycfn.com

Py:   requests.post(url, json={"a": 1})
来源：http://pwl.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ged.dianchejie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://inf.xinyue.icu

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pxd.zhiwuduotai.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://edu.52xcode.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jvj.redwolf501.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://few.fktsv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nqb.zhijiandao.cn

[L03] 设置自定义请求头
来源：http://fjk.yj20258888.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ope.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://njs.redwolf501.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cof.snrcjt.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dqj.daria6918.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://iyv.52xcode.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gre.epnwcf.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ozo.kuanghao11.cn


<!-- 参考信息 -->