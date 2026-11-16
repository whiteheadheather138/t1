代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://rxf.fengsongda.top

[H08] 获取错误信息与堆栈
来源：http://rzs.hongshengwenyu.top

Py:   str(e);  traceback.format_exc()
来源：http://njd.fktsv.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rdu.tanke756.top

JS:   e.message;  e.stack
来源：http://jwn.hysaishi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://sie.nanxinkj.top

Java: e.getMessage();  e.printStackTrace()
来源：http://znj.hnqzz.top

Go:   err.Error()
来源：http://epq.guowangkeji.top

Ruby: e.message;  e.backtrace
来源：http://env.feifeiyinyue.top

C#:   e.Message;  e.StackTrace
来源：http://edo.daxiang520.top

[H09] 带错误码的异常
来源：http://rum.hnxiangtu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yap.ydjk.org.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xmz.hywenlv.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://iyf.guannengcc.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ool.wangshuangyany.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pgs.aibaodan.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ejg.guannengcc.top

Ruby: raise MyError.new("fail", 500)
来源：http://bfe.ivvv.top

C#:   // 自定义异常类中加 Code 属性
来源：http://azn.xylfe.cn

[H10] 资源自动释放
来源：http://vii.hongshengwenyu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://qdc.yonumen.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://plo.shzxlz.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://plk.xylfe.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ich.yongpay.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ppa.hesvh.cn

Go:   defer f.Close()
来源：http://law.snrcjt.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qvf.meibo888.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gdf.aibaodan.cn

================================================================================
来源：http://quz.cdnleiting.top

I. 正则表达式
来源：http://zhx.jianghu66.top

================================================================================
来源：http://rub.tianlin.xyz

[I01] 判断是否匹配
来源：http://vrc.yj202588.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mrf.hysaishi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zqv.fehbvm.com

JS:   /\d+/.test(s)
来源：http://jsu.wangdashe.top

TS:   /\d+/.test(s)
来源：http://msi.snrcjt.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ykw.hcnkem.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uah.hnxiangtu.top

Ruby: s.match?(/\d+/)
来源：http://nos.jinghuilouyu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mpj.c1oappe.top

[I02] 提取所有匹配
来源：http://rds.xziqi.cn

Py:   re.findall(r"\d+", s)
来源：http://gmb.nwbrower.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mmo.mhx1999.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cyv.ydjk.org.cn

TS:   s.match(/\d+/g)
来源：http://hud.nwbrower.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sop.ctjpmb.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qec.ydzc1.top

Ruby: s.scan(/\d+/)
来源：http://phw.snrcjt.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yfo.wangdashe.top

[I03] 提取捕获分组
来源：http://yax.vqdsnc.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bty.chenlongwang.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kyf.svipenyu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bxn.hammf.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kpq.daxiang520.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ilc.zhengqikj.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wjt.hammf.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gjd.sysykeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ryn.wangdashe.top

[I04] 正则替换
来源：http://brd.bbcook.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gcy.mhx1999.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pvz.hcnkem.com

JS:   s.replace(/\d+/g, "#")
来源：http://zce.vqdsnc.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ane.c1oappe.top

Java: s.replaceAll("\\d+", "#")
来源：http://gfr.nwbrower.top

Go:   re.ReplaceAllString(s, "#")
来源：http://lue.hnxiangtu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://kix.yvedp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mxd.yongpay.top

[I05] 按正则拆分
来源：http://frp.zhongyouzk.top

Py:   re.split(r"\s*,\s*", s)
来源：http://vuv.hfpthk.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jsi.zhijiandao.cn

JS:   s.split(/\s*,\s*/)
来源：http://unm.gaohongyu789.top

TS:   s.split(/\s*,\s*/)
来源：http://uxt.c1oappe.top

Java: s.split("\\s*,\\s*")
来源：http://wtg.sweek.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mak.yj202588.top

Ruby: s.split(/\s*,\s*/)
来源：http://efj.wangshuangyany.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pys.shzxlz.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nau.fengsongda.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vmz.zhaomingkeji.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ziy.yfazqb.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jgg.hywenlv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://llp.fanxiaobao.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xky.cashguo.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ffw.gogol.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rzo.zhengqikj.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jsr.hnqzz.top

[I07] 忽略大小写与多行模式
来源：http://vat.yuanzhike.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fff.zhoulong.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://taf.pengpengdd.cyou

JS:   /error/gim；new RegExp("error", "gim")
来源：http://guk.zhoulong.xyz

TS:   /error/gim
来源：http://dbh.jinyuanbaomall.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kqd.zycfv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yjs.hywenlv.cn

Ruby: s.scan(/error/i)
来源：http://wjk.xinyue.icu

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tiz.guowangkeji.top

[I08] 贪婪与非贪婪匹配
来源：http://pou.52xcode.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://osg.jyoumei.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vip.zhengqikj.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tcz.hnxiangtu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tnn.yangfankeji.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://usj.zhengqikj.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ahy.andypj.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fvq.jinqigfzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lgi.zhijiandao.cn

================================================================================
来源：http://mpz.quarkkingdee.top

J. 日期与时间
来源：http://pft.nwbrower.top

================================================================================
来源：http://zfw.ydzc1.top

[J01] 获取当前时间
来源：http://sqd.guannengcc.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://flq.guowangkeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wzz.iojbl.cn

JS:   new Date();  Date.now()
来源：http://crh.kuanghao11.cn

TS:   new Date();  Date.now()
来源：http://pai.chenlongwang.top

Java: LocalDateTime.now();  Instant.now()
来源：http://edw.shanyushiyangtech.top

Go:   time.Now()
来源：http://tdh.pengpengdd.cyou

Ruby: Time.now
来源：http://owq.316326.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dyc.aizwys.cn

[J02] 格式化输出
来源：http://evp.tian-w.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://okg.nanxuanxn.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vqc.tian-w.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wsw.ydzc1.top

TS:   d.toISOString()
来源：http://ddl.cucudq.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vjx.c1oappe.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://osc.yuanzhike.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sxo.snrcjt.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ulq.tian-w.cn

[J03] 字符串解析为日期
来源：http://szf.ywan-chungtsiang.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://onp.ydjk.org.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://oog.fzhhl.top

JS:   new Date("2024-01-02")
来源：http://lzl.ywan-chungtsiang.top

TS:   new Date("2024-01-02")
来源：http://ynb.zdbjq.cn

Java: LocalDate.parse("2024-01-02")
来源：http://epm.xuanzx.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nmp.havefunace.top

Ruby: Date.parse("2024-01-02")
来源：http://sew.uphjek.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vzy.dashuyun.cn

[J04] 时间戳与日期互转
来源：http://rmc.fanxiaobao.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://beo.nwbrower.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zmt.daxiang520.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gmo.52xcode.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qgg.ehwqpu.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://itn.guannengcc.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://amb.nwbrower.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rgm.meibo888.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gxk.chenlongwang.top

[J05] 时间加减（加 7 天）
来源：http://kvc.shzxlz.cn

Py:   now + timedelta(days=7)
来源：http://tat.bjfxy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://wpg.guowangkeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yhc.havefunace.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kdn.jinqigufen.top

Java: LocalDate.now().plusDays(7)
来源：http://hpl.jinqigfzy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vxg.nanxinkj.top

Ruby: Time.now + 7 * 86400
来源：http://exi.cucudq.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kjj.c1oappe.top

[J06] 计算两时间之差
来源：http://jic.yongpay.top

Py:   (end - start).total_seconds()
来源：http://dih.yueranfly.top

PHP:  $end->diff($start)->days;
来源：http://hit.vqdsnc.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://csk.yangfankeji.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vfh.0kj1m.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xcg.chenlongwang.top

Go:   end.Sub(start).Hours()
来源：http://ahp.bjfxy.top

Ruby: end - start                 # 返回秒数
来源：http://olg.sweek.top

C#:   (end - start).TotalSeconds
来源：http://isr.jqgufenzy.top

[J07] 比较两个日期
来源：http://idm.bjfxy.top

Py:   d1 < d2;  d1 == d2
来源：http://may.zhoulong.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kfb.jiagoushi.top

JS:   d1.getTime() < d2.getTime()
来源：http://qwp.gaohongyu789.top

TS:   d1.getTime() < d2.getTime()
来源：http://pzn.fanxiaobao.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jfq.gzhubu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dsx.andypj.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://kjj.yj20258.top

C#:   d1 < d2;  d1 == d2
来源：http://lah.haohaochexian.top

[J08] 提取年月日与星期
来源：http://bmb.zdbjq.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dzm.yj202588.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xhd.guannengcc.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://scx.haohaochexian.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mni.cqqwz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dym.hammf.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hrb.quarkkingdee.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tvt.hfpthk.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xge.feifeiyinyue.top

[J09] 时区处理
来源：http://hnn.epnwcf.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://spv.xuetiantiany.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sob.tian-w.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oix.aizwys.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kyn.pengpengdd.cyou

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tiq.yuanzhike.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pfh.fanxiaobao.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://ivd.dashuyun.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xqy.shanyushiyangkeji.top

[J10] 取今天 / 本月第一天
来源：http://dok.zdbjq.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://asn.fehbvm.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pan.yonumen.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://byc.yueranfly.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://eai.svipenyu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uqw.daria6918.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nfi.guannengcc.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sap.jqgufenzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ccc.ydjk.org.cn

================================================================================
来源：http://dms.hywenlv.cn

K. JSON 与序列化
来源：http://puq.cucudq.cn

================================================================================
来源：http://nby.fehbvm.com

[K01] 对象转 JSON 字符串
来源：http://gsk.birdmap.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nut.hnqzz.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bza.chenzaomai.com

JS:   JSON.stringify(obj)
来源：http://yye.gaohongyu789.top

TS:   JSON.stringify(obj)
来源：http://idr.jinyuanbaomall.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wqc.chenzaomai.com

Go:   json.Marshal(obj)
来源：http://eec.wangshuangyany.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mzc.gotoacloud.top

C#:   JsonSerializer.Serialize(obj)
来源：http://lyk.zdqjudy.top

[K02] JSON 字符串转对象
来源：http://ihp.fanxiaobao.xyz

Py:   json.loads(s)
来源：http://bhx.cqqwz.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://akf.yfazqb.com

JS:   JSON.parse(s)
来源：http://zzj.yj202588.top

TS:   JSON.parse(s)
来源：http://nla.kuanghao11.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://srm.hongshengwenyu.top

Go:   json.Unmarshal(data, &v)
来源：http://gic.cashguo.top

Ruby: JSON.parse(s)
来源：http://skk.daxiang520.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ezi.birdmap.top

[K03] JSON 美化输出（带缩进）
来源：http://lkc.tanke756.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xxb.yvedp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dhc.zycfv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cpq.pengpengdd.cyou

TS:   JSON.stringify(obj, null, 2)
来源：http://ezs.zhoulong.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zov.zhixingplan.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sgg.pengpengdd.cyou

Ruby: JSON.pretty_generate(obj)
来源：http://iby.daxiang520.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rza.bbcook.cn

[K04] 读取 JSON 文件
来源：http://xii.tian-w.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bps.chenjidiqi.icu

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tis.hongshengwenyu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pyq.0kj1m.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zms.guowangkeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qeb.chenjidiqi.icu

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://iqb.ydjk.org.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dft.meibo888.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xop.pycfn.com

[K05] 深拷贝对象
来源：http://gfb.mhx1999.top

Py:   copy.deepcopy(obj)
来源：http://nzj.chenzaomai.com

PHP:  unserialize(serialize($obj));
来源：http://qdr.xziqi.cn

JS:   structuredClone(obj)
来源：http://iql.cqqwz.cn

TS:   structuredClone(obj)
来源：http://egs.andypj.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://ely.daxiang520.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dpm.andypj.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://smp.aizwys.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://uct.yangfankeji.com

[K06] 解析 URL 查询串
来源：http://lif.havefunace.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zln.yonumen.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zvd.sufxvd.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fpv.gzhubu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cbx.zdbjq.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://peu.hysaishi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ugl.redwolf501.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://keq.jqgufenzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jrh.yonumen.top

[K07] 进制转换
来源：http://ssl.dashuyun.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mnv.jinqigufen.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fnf.shanyushiyangtech.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lqr.aibaodan.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sgy.fehbvm.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gew.hesvh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://afp.hysaishi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mtq.jinqigufen.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lzi.ydzc1.top

[K08] 二进制序列化（非 JSON）
来源：http://eui.ppjwa.cn

Py:   pickle.dumps(obj)
来源：http://gfy.birdmap.top

PHP:  serialize($obj);  unserialize($s);
来源：http://nhp.ivvv.top

JS:   v8.serialize(obj)        // Node
来源：http://tqe.cqqwz.cn

TS:   v8.serialize(obj)        // Node
来源：http://ulm.epnwcf.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wqh.ydzc1.top

Go:   encoding/gob
来源：http://gyd.zdbjq.cn

Ruby: Marshal.dump(obj)
来源：http://lfm.daxiang520.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xrk.xinyue.icu

================================================================================
来源：http://lrs.zhiwuduotai.top

L. 网络请求
来源：http://mxf.hongshengwenyu.top

================================================================================
来源：http://lcv.svipenyu.cn

[L01] 发送 GET 请求
来源：http://oud.cashguo.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://coq.tian-w.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://iul.yanxiufei.cn

JS:   await fetch(url)
来源：http://uav.tanke756.top

TS:   await fetch(url)
来源：http://qxo.52xcode.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pyv.cqqwz.cn

Go:   resp, err := http.Get(url)
来源：http://aec.jinghuilouyu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ywy.zhoulong.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nap.wangdashe.top

[L02] 发送 POST JSON
来源：http://csa.zhiwuduotai.top

Py:   requests.post(url, json={"a": 1})
来源：http://chr.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tuk.jiagoushi.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hdn.yangfankeji.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bby.xziqi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jum.zhijiandao.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tii.sxryk.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nix.cashguo.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bjk.xuetiantiany.cn

[L03] 设置自定义请求头
来源：http://acd.gaohongyu789.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://doq.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ipb.gogol.net.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rql.iojbl.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kcf.iojbl.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cwv.andypj.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tmv.fengsongda.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ycd.hnqzz.top


<!-- 参考信息 -->