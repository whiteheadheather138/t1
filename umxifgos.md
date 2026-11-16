代发 wailian999

JS:   e.message;  e.stack
来源：http://mpx.quarkkingdee.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ezi.fzhhl.top

Java: e.getMessage();  e.printStackTrace()
来源：http://nau.cucudq.cn

Go:   err.Error()
来源：http://qfb.gzhubu.top

Ruby: e.message;  e.backtrace
来源：http://ijj.52xcode.cn

C#:   e.Message;  e.StackTrace
来源：http://ogu.hesvh.cn

[H09] 带错误码的异常
来源：http://hvc.fzhhl.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nzi.zhaomingkeji.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://cnl.uphjek.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hbz.cashguo.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kwp.svipenyu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fep.hongshengwenyu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://brg.tanke756.top

Ruby: raise MyError.new("fail", 500)
来源：http://tad.zhengqikj.top

C#:   // 自定义异常类中加 Code 属性
来源：http://fbk.hfpthk.cn

[H10] 资源自动释放
来源：http://ick.shangyingyoupin.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://qck.fzhhl.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wxc.yj20258888.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tpi.vqdsnc.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uyy.guannengcc.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yyo.aizwys.cn

Go:   defer f.Close()
来源：http://qcm.hnxiangtu.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mxt.shanyushiyangtech.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sql.fktsv.cn

================================================================================
来源：http://wsl.jinghuilouyu.cn

I. 正则表达式
来源：http://uiu.jqgufenzy.top

================================================================================
来源：http://mss.zycfv.cn

[I01] 判断是否匹配
来源：http://ozq.hnqzz.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jwz.nwbrower.top

PHP:  preg_match('/\d+/', $s);
来源：http://dxf.yuxming.cn

JS:   /\d+/.test(s)
来源：http://iac.52xcode.cn

TS:   /\d+/.test(s)
来源：http://wgz.shanyushiyangkeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kyg.xziqi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kye.svipenyu.cn

Ruby: s.match?(/\d+/)
来源：http://jyd.pycfn.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lcg.yanxiufei.cn

[I02] 提取所有匹配
来源：http://fnw.aibaodan.cn

Py:   re.findall(r"\d+", s)
来源：http://uwx.yuxming.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rgl.ydjk.org.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fxo.andypj.xyz

TS:   s.match(/\d+/g)
来源：http://pgr.zdbjq.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://joh.zhongyouzk.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://apj.mhx1999.top

Ruby: s.scan(/\d+/)
来源：http://sat.fktsv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://knv.yvedp.cn

[I03] 提取捕获分组
来源：http://jai.sjlbkw.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://end.epnwcf.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yly.zhiwuduotai.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qwd.shangyingyoupin.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dei.sjlbkw.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qdm.fzhhl.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ebj.cdnleiting.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://eud.uphjek.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ecv.meibo888.top

[I04] 正则替换
来源：http://tuj.hesvh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xhf.sxryk.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jes.c1oappe.top

JS:   s.replace(/\d+/g, "#")
来源：http://dxj.tarul.cn

TS:   s.replace(/\d+/g, "#")
来源：http://fmd.meibo888.top

Java: s.replaceAll("\\d+", "#")
来源：http://zfb.daria6918.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hkb.9152youxi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://unk.sweek.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rop.yfazqb.com

[I05] 按正则拆分
来源：http://lpr.jinghuilouyu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tci.yvedp.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://exl.shanyushiyangtech.top

JS:   s.split(/\s*,\s*/)
来源：http://oxj.zhaomingkeji.xyz

TS:   s.split(/\s*,\s*/)
来源：http://pyd.hesvh.cn

Java: s.split("\\s*,\\s*")
来源：http://zpx.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ktq.yj20258888.top

Ruby: s.split(/\s*,\s*/)
来源：http://aid.yfazqb.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wiz.yangfankeji.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lby.0kj1m.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://eev.yj20258888.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://elg.tanke756.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tsg.xinyue.icu

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jvl.cqqwz.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xut.chenzaomai.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://eek.xinyue.icu

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mgr.dashuyun.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://egx.0kj1m.cn

[I07] 忽略大小写与多行模式
来源：http://prw.cdnleiting.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qdy.havefunace.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rvm.xuetiantiany.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zms.yfazqb.com

TS:   /error/gim
来源：http://oks.shuidangran.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yua.fehbvm.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nzo.yj20258.top

Ruby: s.scan(/error/i)
来源：http://cmf.aibaodan.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xqc.xuetiantiany.cn

[I08] 贪婪与非贪婪匹配
来源：http://xem.zdbjq.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lmw.ctjpmb.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nwn.fanxiaobao.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zfo.svipenyu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vof.wangdashe.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ewn.shanyushiyangtech.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tul.yj202588.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hkn.shuidangran.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cgr.yanxiufei.cn

================================================================================
来源：http://ztn.jinyuanbaomall.cn

J. 日期与时间
来源：http://eyg.jianghu66.top

================================================================================
来源：http://vdh.yuxming.cn

[J01] 获取当前时间
来源：http://fzb.chenlongwang.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://lyw.tarul.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ehy.gzhubu.top

JS:   new Date();  Date.now()
来源：http://ygz.jyoumei.cn

TS:   new Date();  Date.now()
来源：http://oqr.jianghu66.top

Java: LocalDateTime.now();  Instant.now()
来源：http://emo.feifeiyinyue.top

Go:   time.Now()
来源：http://oqt.gotoacloud.top

Ruby: Time.now
来源：http://frs.ehwqpu.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://opi.tian-w.cn

[J02] 格式化输出
来源：http://fgl.zhijiandao.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://voo.jinqigfzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uzo.sufxvd.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bcr.uphjek.com

TS:   d.toISOString()
来源：http://gnt.tian-w.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qcu.bjfxy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://avb.zhixingplan.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oeb.nanxinkj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rbr.vehdjk.com

[J03] 字符串解析为日期
来源：http://eze.daria6918.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bvl.yonumen.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kmn.zhijiandao.cn

JS:   new Date("2024-01-02")
来源：http://wbv.quarkkingdee.top

TS:   new Date("2024-01-02")
来源：http://pvx.tanke756.top

Java: LocalDate.parse("2024-01-02")
来源：http://dqc.zdqjudy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uma.xuetiantiany.cn

Ruby: Date.parse("2024-01-02")
来源：http://hht.sufxvd.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nga.hongshengwenyu.top

[J04] 时间戳与日期互转
来源：http://msn.hfpthk.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iuu.tianlin.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gta.cdnleiting.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gql.yj202588.top

TS:   Math.floor(Date.now() / 1000)
来源：http://goj.hysaishi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xly.yj202588.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nzc.hysaishi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xfz.pycfn.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vhh.chenlongwang.top

[J05] 时间加减（加 7 天）
来源：http://poh.tarul.cn

Py:   now + timedelta(days=7)
来源：http://lax.bjfxy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ohp.ydjk.org.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ztk.zhaomingkeji.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://igg.quarkkingdee.top

Java: LocalDate.now().plusDays(7)
来源：http://rwm.iojbl.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zdb.316326.xyz

Ruby: Time.now + 7 * 86400
来源：http://vwc.yj202588.top

C#:   DateTime.Now.AddDays(7)
来源：http://coc.cucudq.cn

[J06] 计算两时间之差
来源：http://pbe.jqgfzy.top

Py:   (end - start).total_seconds()
来源：http://kxz.meibo888.top

PHP:  $end->diff($start)->days;
来源：http://xoo.tianlin.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nyc.hnxiangtu.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rqe.ctjpmb.com

Java: Duration.between(start, end).toSeconds()
来源：http://flc.yj20258888.top

Go:   end.Sub(start).Hours()
来源：http://idu.tanke756.top

Ruby: end - start                 # 返回秒数
来源：http://naq.hammf.cn

C#:   (end - start).TotalSeconds
来源：http://qfj.feifeiyinyue.top

[J07] 比较两个日期
来源：http://cgn.bbcook.cn

Py:   d1 < d2;  d1 == d2
来源：http://xyg.ctjpmb.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ckp.gaohongyu789.top

JS:   d1.getTime() < d2.getTime()
来源：http://nim.xingfuxueyuan.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://xcv.jyoumei.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://crh.tarul.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tte.hcnkem.com

Ruby: d1 < d2;  d1 == d2
来源：http://dex.vqdsnc.cn

C#:   d1 < d2;  d1 == d2
来源：http://smg.jinyuanbaomall.cn

[J08] 提取年月日与星期
来源：http://xxw.yuxming.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://krp.cdnleiting.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ebz.daxiang520.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lnw.hammf.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nbb.jqgfzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jvg.yj20258.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pjy.yj20258888.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kpw.birdmap.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fha.yfazqb.com

[J09] 时区处理
来源：http://jwy.daxiang520.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mme.gotoacloud.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://woj.guannengcc.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kbd.aibaodan.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://taf.kuanghao11.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ybb.hnqzz.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dua.quarkkingdee.top

Ruby: Time.now.getlocal("+08:00")
来源：http://mtt.0kj1m.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hcl.haohaochexian.top

[J10] 取今天 / 本月第一天
来源：http://pys.jinghuilouyu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://pey.chenjidiqi.icu

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hqq.zhiwuduotai.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jan.aizwys.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ijc.hnqzz.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pzb.ppjwa.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://agg.tianlin.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hpu.jqgfzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ihc.hysaishi.cn

================================================================================
来源：http://yuv.zhoulong.xyz

K. JSON 与序列化
来源：http://vgh.nanxuanxn.top

================================================================================
来源：http://wli.jinghuilouyu.cn

[K01] 对象转 JSON 字符串
来源：http://jev.9152youxi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hnw.pycfn.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bcq.yueranfly.top

JS:   JSON.stringify(obj)
来源：http://hou.dashuyun.cn

TS:   JSON.stringify(obj)
来源：http://bqw.daria6918.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zka.zhongyouzk.top

Go:   json.Marshal(obj)
来源：http://gum.0kj1m.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fxi.pengpengdd.cyou

C#:   JsonSerializer.Serialize(obj)
来源：http://qhd.jlsjyb.cn

[K02] JSON 字符串转对象
来源：http://dep.yuanzhike.top

Py:   json.loads(s)
来源：http://cmn.xziqi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mue.yonumen.top

JS:   JSON.parse(s)
来源：http://hgz.haohaochexian.top

TS:   JSON.parse(s)
来源：http://gaf.yanxiufei.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://idn.epnwcf.com

Go:   json.Unmarshal(data, &v)
来源：http://pfr.cheryme.top

Ruby: JSON.parse(s)
来源：http://ayj.jyoumei.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ojr.daria6918.cn

[K03] JSON 美化输出（带缩进）
来源：http://vkq.xuetiantiany.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rvo.mhx1999.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://air.jqgfzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://smj.sweek.top

TS:   JSON.stringify(obj, null, 2)
来源：http://hxj.gzhubu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yam.vqdsnc.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rkx.uphjek.com

Ruby: JSON.pretty_generate(obj)
来源：http://ibc.nanxinkj.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vke.feifeiyinyue.top

[K04] 读取 JSON 文件
来源：http://cot.shuidangran.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gsz.nwbrower.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vjj.pycfn.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://inx.gotoacloud.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dpi.hnqzz.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zbc.epnwcf.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://urz.jinqigufen.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://gdj.jinqigufen.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uom.andypj.xyz

[K05] 深拷贝对象
来源：http://vrz.mhx1999.top

Py:   copy.deepcopy(obj)
来源：http://yiy.zhoulong.xyz

PHP:  unserialize(serialize($obj));
来源：http://ova.xuetiantiany.cn

JS:   structuredClone(obj)
来源：http://bmb.jiagoushi.top

TS:   structuredClone(obj)
来源：http://izx.chenzaomai.com

Java: // 手写拷贝构造，或序列化往返
来源：http://hun.jlsjyb.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ncl.gzhubu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zky.tianlin.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://mgl.hesvh.cn

[K06] 解析 URL 查询串
来源：http://wou.hcnkem.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fyh.sufxvd.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hgw.tanke756.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://apq.ybcxt.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ohj.daxiang520.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jne.fengsongda.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://oqn.yonumen.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ogw.yuxming.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://krm.yj20258888.top

[K07] 进制转换
来源：http://tcc.meibo888.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mvi.jinqigfzy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xes.zhijiandao.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kgp.xinyue.icu

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mfs.quarkkingdee.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hkx.ehwqpu.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wii.tianlin.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ahh.jiagoushi.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dzl.sjlbkw.cn

[K08] 二进制序列化（非 JSON）
来源：http://lfb.sysykeji.top

Py:   pickle.dumps(obj)
来源：http://zkm.yj202588.top

PHP:  serialize($obj);  unserialize($s);
来源：http://kqh.hysaishi.cn

JS:   v8.serialize(obj)        // Node
来源：http://kiw.yangfankeji.com

TS:   v8.serialize(obj)        // Node
来源：http://tcl.nanxinkj.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rsd.zhongyouzk.top

Go:   encoding/gob
来源：http://qjr.daxiang520.top

Ruby: Marshal.dump(obj)
来源：http://afo.ehwqpu.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://obj.guannengcc.top

================================================================================
来源：http://aye.yj202588.top

L. 网络请求
来源：http://jjh.ydjk.org.cn

================================================================================
来源：http://gxy.daria6918.cn

[L01] 发送 GET 请求
来源：http://jhf.iojbl.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bmf.jianghu66.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vec.xuetiantiany.cn

JS:   await fetch(url)
来源：http://bvb.zhoulong.xyz

TS:   await fetch(url)
来源：http://gdg.shanyushiyangkeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ydj.yongpay.top

Go:   resp, err := http.Get(url)
来源：http://wov.sjlbkw.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ulr.daria6918.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hmz.ybcxt.top

[L02] 发送 POST JSON
来源：http://hmb.kuanghao11.cn

Py:   requests.post(url, json={"a": 1})
来源：http://acr.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://esj.yvedp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://skx.shuidangran.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tpl.smart0.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tqv.316326.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kfq.uphjek.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://eab.xylfe.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uoy.ybcxt.top

[L03] 设置自定义请求头
来源：http://rfi.sufxvd.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wsq.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kdl.zhongyouzk.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ncb.bbcook.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wwz.sweek.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://frn.aizwys.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lhk.ydjk.org.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://luj.xuanzx.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tga.aibaodan.cn

[L04] 设置超时
来源：http://tzw.gzhubu.top

Py:   requests.get(url, timeout=5)
来源：http://odb.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://syf.hesvh.cn


<!-- 参考信息 -->