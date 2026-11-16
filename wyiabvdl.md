代发 wailian999

JS:   e.message;  e.stack
来源：http://qov.pycfn.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://ken.birdmap.top

Java: e.getMessage();  e.printStackTrace()
来源：http://mlc.zhijiandao.cn

Go:   err.Error()
来源：http://cjs.hesvh.cn

Ruby: e.message;  e.backtrace
来源：http://oxm.yj20258888.top

C#:   e.Message;  e.StackTrace
来源：http://rbj.yuanzhike.top

[H09] 带错误码的异常
来源：http://ejf.gogol.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lkz.jqgufenzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ffe.yvedp.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bvl.xuetiantiany.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cct.hnxiangtu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bfn.sxryk.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cfu.zhengqikj.top

Ruby: raise MyError.new("fail", 500)
来源：http://kjs.cqqwz.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ukl.tarul.cn

[H10] 资源自动释放
来源：http://lnk.xuanzx.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://yov.gogol.net.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oyp.hysaishi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rlk.hysaishi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://skp.wangdashe.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qdm.gzhubu.top

Go:   defer f.Close()
来源：http://llq.tanke756.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jdf.fanxiaobao.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lql.cashguo.top

================================================================================
来源：http://anp.shanyushiyangtech.top

I. 正则表达式
来源：http://ung.hnxiangtu.top

================================================================================
来源：http://bye.yj20258888.top

[I01] 判断是否匹配
来源：http://ecx.yvedp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mca.sufxvd.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xrt.vehdjk.com

JS:   /\d+/.test(s)
来源：http://jzx.havefunace.top

TS:   /\d+/.test(s)
来源：http://pui.zhoulong.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bye.shanyushiyangkeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xhr.hnqzz.top

Ruby: s.match?(/\d+/)
来源：http://xcx.yj20258.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nti.vehdjk.com

[I02] 提取所有匹配
来源：http://dgq.hywenlv.cn

Py:   re.findall(r"\d+", s)
来源：http://zqb.0kj1m.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mge.gzhubu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://exz.wangdashe.top

TS:   s.match(/\d+/g)
来源：http://kjp.cqqwz.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://krq.xuetiantiany.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cvn.cucudq.cn

Ruby: s.scan(/\d+/)
来源：http://sxq.xinyue.icu

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bor.yanxiufei.cn

[I03] 提取捕获分组
来源：http://zcg.tian-w.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ava.kuanghao11.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vka.yueranfly.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dts.9152youxi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nfn.cqqwz.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://skh.zhiwuduotai.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://viv.shanyushiyangkeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gwj.kuanghao11.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ben.0kj1m.cn

[I04] 正则替换
来源：http://fec.ywan-chungtsiang.top

Py:   re.sub(r"\d+", "#", s)
来源：http://dnq.meibo888.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ldf.jqgfzy.top

JS:   s.replace(/\d+/g, "#")
来源：http://iaj.wangshuangyany.cn

TS:   s.replace(/\d+/g, "#")
来源：http://duv.zhaomingkeji.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://sym.xuanzx.com

Go:   re.ReplaceAllString(s, "#")
来源：http://ncn.gogol.net.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://bes.ppjwa.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fht.cashguo.top

[I05] 按正则拆分
来源：http://gjf.yj20258888.top

Py:   re.split(r"\s*,\s*", s)
来源：http://dhp.ppjwa.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pdn.birdmap.top

JS:   s.split(/\s*,\s*/)
来源：http://rzt.cqqwz.cn

TS:   s.split(/\s*,\s*/)
来源：http://pdt.cdnleiting.top

Java: s.split("\\s*,\\s*")
来源：http://zen.cheryme.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nqg.fanxiaobao.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://ybf.nanxuanxn.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rkf.jqgfzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yjb.mhx1999.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ess.jinqigufen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://opk.gzhubu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xwl.haohaochexian.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://suf.svipenyu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://edm.dashuyun.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bym.dianchejie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uco.jinqigufen.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://trv.shzxlz.cn

[I07] 忽略大小写与多行模式
来源：http://dcn.daria6918.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rym.jlsjyb.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://afm.xinyue.icu

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ngi.jyoumei.cn

TS:   /error/gim
来源：http://iwt.snrcjt.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fal.gaohongyu789.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ykm.jinqigfzy.top

Ruby: s.scan(/error/i)
来源：http://xji.yj202588.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zwp.cdnleiting.top

[I08] 贪婪与非贪婪匹配
来源：http://qgb.tianlin.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mzv.dashuyun.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mke.yj20258.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fkn.hammf.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hge.0kj1m.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://obl.hywenlv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jmr.tian-w.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ocp.jyoumei.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jyz.fktsv.cn

================================================================================
来源：http://wvv.tarul.cn

J. 日期与时间
来源：http://wuw.jinqigufen.top

================================================================================
来源：http://vxm.jinqigufen.top

[J01] 获取当前时间
来源：http://avp.quarkkingdee.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://tcr.vqdsnc.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://syg.xuetiantiany.cn

JS:   new Date();  Date.now()
来源：http://sgh.fehbvm.com

TS:   new Date();  Date.now()
来源：http://gyf.hnxiangtu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://kqr.nanxuanxn.top

Go:   time.Now()
来源：http://rsb.hongshengwenyu.top

Ruby: Time.now
来源：http://juz.jianghu66.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lma.mhx1999.top

[J02] 格式化输出
来源：http://oqm.shzxlz.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ovd.fzhhl.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pjk.nanxuanxn.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hfb.fktsv.cn

TS:   d.toISOString()
来源：http://ylm.fanxiaobao.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://led.yvedp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vcd.hcnkem.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yih.fzhhl.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://otq.bjfxy.top

[J03] 字符串解析为日期
来源：http://eaf.meibo888.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://azz.ehwqpu.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://huj.ydzc1.top

JS:   new Date("2024-01-02")
来源：http://nss.feifeiyinyue.top

TS:   new Date("2024-01-02")
来源：http://lkj.zhaomingkeji.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://tgm.hnxiangtu.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qmv.jyoumei.cn

Ruby: Date.parse("2024-01-02")
来源：http://nvh.uphjek.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://stm.yuxming.cn

[J04] 时间戳与日期互转
来源：http://opk.fzhhl.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hji.c1oappe.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lbp.cheryme.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nug.shzxlz.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jsz.cdnleiting.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rbq.ydzc1.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vgo.svipenyu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mwx.fengsongda.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tvf.tanke756.top

[J05] 时间加减（加 7 天）
来源：http://lpa.hongshengwenyu.top

Py:   now + timedelta(days=7)
来源：http://ulg.52xcode.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yua.hammf.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://abz.meibo888.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bjl.andypj.xyz

Java: LocalDate.now().plusDays(7)
来源：http://fug.zhengqikj.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pxl.gogol.net.cn

Ruby: Time.now + 7 * 86400
来源：http://cyi.quarkkingdee.top

C#:   DateTime.Now.AddDays(7)
来源：http://gkh.cqqwz.cn

[J06] 计算两时间之差
来源：http://ysb.hywenlv.cn

Py:   (end - start).total_seconds()
来源：http://piu.yuanzhike.top

PHP:  $end->diff($start)->days;
来源：http://zia.fktsv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uso.havefunace.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://khp.snrcjt.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xyt.hcnkem.com

Go:   end.Sub(start).Hours()
来源：http://pbq.jinqigufen.top

Ruby: end - start                 # 返回秒数
来源：http://mln.316326.xyz

C#:   (end - start).TotalSeconds
来源：http://ynj.daria6918.cn

[J07] 比较两个日期
来源：http://set.ybcxt.top

Py:   d1 < d2;  d1 == d2
来源：http://hjx.9152youxi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lkt.nwbrower.top

JS:   d1.getTime() < d2.getTime()
来源：http://drk.smart0.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://hgb.jyoumei.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jcc.sufxvd.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mag.zdqjudy.top

Ruby: d1 < d2;  d1 == d2
来源：http://gwm.hammf.cn

C#:   d1 < d2;  d1 == d2
来源：http://nex.daria6918.cn

[J08] 提取年月日与星期
来源：http://dkc.redwolf501.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hxb.svipenyu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://eif.birdmap.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gyf.cashguo.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qel.ydjk.org.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gmy.yongpay.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zuj.jqgufenzy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zod.hywenlv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lgj.jinqigfzy.top

[J09] 时区处理
来源：http://kfh.ydzc1.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vee.tanke756.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zxb.sysykeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nbl.xinyue.icu

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ycj.chenjidiqi.icu

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lxw.aibaodan.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://awb.fanxiaobao.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://uax.sysykeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lzd.cucudq.cn

[J10] 取今天 / 本月第一天
来源：http://tqv.tarul.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://unq.xuanzx.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lbh.yj202588.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bss.hongshengwenyu.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sea.xuetiantiany.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xuv.xinyue.icu

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ygp.yfazqb.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bza.cdnleiting.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://alq.hammf.cn

================================================================================
来源：http://sdw.daxiang520.top

K. JSON 与序列化
来源：http://asb.yuxming.cn

================================================================================
来源：http://rcp.yvedp.cn

[K01] 对象转 JSON 字符串
来源：http://gft.hfpthk.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://odt.zdbjq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xvf.52xcode.cn

JS:   JSON.stringify(obj)
来源：http://vbt.ehwqpu.com

TS:   JSON.stringify(obj)
来源：http://kqc.52xcode.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yzy.xuanzx.com

Go:   json.Marshal(obj)
来源：http://hlq.jinghuilouyu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fvb.yj20258.top

C#:   JsonSerializer.Serialize(obj)
来源：http://yym.zdqjudy.top

[K02] JSON 字符串转对象
来源：http://lus.yuxming.cn

Py:   json.loads(s)
来源：http://uvy.9152youxi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ynb.birdmap.top

JS:   JSON.parse(s)
来源：http://xxu.316326.xyz

TS:   JSON.parse(s)
来源：http://euz.shuidangran.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ztp.pycfn.com

Go:   json.Unmarshal(data, &v)
来源：http://plg.zhijiandao.cn

Ruby: JSON.parse(s)
来源：http://kil.9152youxi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qsx.chenzaomai.com

[K03] JSON 美化输出（带缩进）
来源：http://noo.guowangkeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://suq.mhx1999.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hhi.yj20258.top

JS:   JSON.stringify(obj, null, 2)
来源：http://tka.xuanzx.com

TS:   JSON.stringify(obj, null, 2)
来源：http://fho.yuxming.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cqr.jinyuanbaomall.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hgg.jinqigfzy.top

Ruby: JSON.pretty_generate(obj)
来源：http://lmo.ivvv.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ecc.zhixingplan.top

[K04] 读取 JSON 文件
来源：http://lkb.jinqigfzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jrb.sufxvd.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fbw.guowangkeji.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dfq.iojbl.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jls.ivvv.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tjq.sweek.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uil.hysaishi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://heb.zhoulong.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dyw.wangshuangyany.cn

[K05] 深拷贝对象
来源：http://gqg.zhiwuduotai.top

Py:   copy.deepcopy(obj)
来源：http://iro.hywenlv.cn

PHP:  unserialize(serialize($obj));
来源：http://naj.epnwcf.com

JS:   structuredClone(obj)
来源：http://hoh.daria6918.cn

TS:   structuredClone(obj)
来源：http://fjw.fehbvm.com

Java: // 手写拷贝构造，或序列化往返
来源：http://gxh.meibo888.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://urj.cucudq.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://foc.fengsongda.top

C#:   // 序列化往返，或自定义 Clone
来源：http://jqs.xuetiantiany.cn

[K06] 解析 URL 查询串
来源：http://xzq.haohaochexian.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fer.nanxinkj.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blx.zdqjudy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://clq.hongshengwenyu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zum.jinyuanbaomall.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rnm.fktsv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qrj.hesvh.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xuy.ydjk.org.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gmx.fzhhl.top

[K07] 进制转换
来源：http://hka.dianchejie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xcs.fehbvm.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cmo.xingfuxueyuan.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://prc.wangdashe.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hxi.xingfuxueyuan.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://aij.yuanzhike.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rjt.sjlbkw.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qkc.jianghu66.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vhy.vehdjk.com

[K08] 二进制序列化（非 JSON）
来源：http://qso.xuetiantiany.cn

Py:   pickle.dumps(obj)
来源：http://erd.jyoumei.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gly.redwolf501.top

JS:   v8.serialize(obj)        // Node
来源：http://njt.cheryme.top

TS:   v8.serialize(obj)        // Node
来源：http://ubh.pengpengdd.cyou

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xzl.tarul.cn

Go:   encoding/gob
来源：http://aho.yueranfly.top

Ruby: Marshal.dump(obj)
来源：http://llz.yvedp.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hjo.xinyue.icu

================================================================================
来源：http://ydh.zhengqikj.top

L. 网络请求
来源：http://goq.svipenyu.cn

================================================================================
来源：http://xty.hnqzz.top

[L01] 发送 GET 请求
来源：http://iaq.shuidangran.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gpr.wangshuangyany.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jjy.jlsjyb.cn

JS:   await fetch(url)
来源：http://wqg.meibo888.top

TS:   await fetch(url)
来源：http://pla.bbcook.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://noo.nanxinkj.top

Go:   resp, err := http.Get(url)
来源：http://sec.svipenyu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://irv.jinqigfzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dly.sjlbkw.cn

[L02] 发送 POST JSON
来源：http://grd.snrcjt.cn

Py:   requests.post(url, json={"a": 1})
来源：http://eht.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zhs.shanyushiyangkeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lkd.fehbvm.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fzz.tarul.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ygi.zhijiandao.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fml.gaohongyu789.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jdh.nanxuanxn.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tar.sweek.top

[L03] 设置自定义请求头
来源：http://bsn.bjfxy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yfh.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sga.vqdsnc.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kyi.svipenyu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nsm.yueranfly.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sdv.52xcode.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qzu.hnqzz.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ctd.quarkkingdee.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://crj.zdbjq.cn

[L04] 设置超时
来源：http://wfn.snrcjt.cn

Py:   requests.get(url, timeout=5)
来源：http://tsx.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uvc.yanxiufei.cn


<!-- 参考信息 -->