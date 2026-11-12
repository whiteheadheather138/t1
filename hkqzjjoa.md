代发 wailian999

JS:   e.message;  e.stack
来源：http://lvl.hfpthk.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rlj.mhx1999.top

Java: e.getMessage();  e.printStackTrace()
来源：http://zmm.0kj1m.cn

Go:   err.Error()
来源：http://kvf.gogol.net.cn

Ruby: e.message;  e.backtrace
来源：http://jhg.chenlongwang.top

C#:   e.Message;  e.StackTrace
来源：http://kaf.shangyingyoupin.top

[H09] 带错误码的异常
来源：http://nvj.hongshengwenyu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mnz.hammf.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dka.hammf.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vka.jinqigufen.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xhe.quarkkingdee.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ppp.hammf.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ziw.guowangkeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://rsb.jiagoushi.top

C#:   // 自定义异常类中加 Code 属性
来源：http://eey.gotoacloud.top

[H10] 资源自动释放
来源：http://bsv.zhaomingkeji.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://juu.xinyue.icu

PHP:  // 无 with：在 finally 里 fclose()
来源：http://iqj.jinyuanbaomall.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://isf.daxiang520.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tsv.jianghu66.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qtz.jinyuanbaomall.cn

Go:   defer f.Close()
来源：http://stt.yfazqb.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uyw.nanxuanxn.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://eyw.xuetiantiany.cn

================================================================================
来源：http://afr.nwbrower.top

I. 正则表达式
来源：http://mvm.xingfuxueyuan.xyz

================================================================================
来源：http://clv.hongshengwenyu.top

[I01] 判断是否匹配
来源：http://avr.feifeiyinyue.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ham.hcnkem.com

PHP:  preg_match('/\d+/', $s);
来源：http://ygh.yfazqb.com

JS:   /\d+/.test(s)
来源：http://huh.yuxming.cn

TS:   /\d+/.test(s)
来源：http://ilb.zdqjudy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vyb.quarkkingdee.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rpg.nanxuanxn.top

Ruby: s.match?(/\d+/)
来源：http://bhh.yonumen.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://biz.hammf.cn

[I02] 提取所有匹配
来源：http://vfb.yonumen.top

Py:   re.findall(r"\d+", s)
来源：http://bev.fanxiaobao.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hjk.daria6918.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pqx.ivvv.top

TS:   s.match(/\d+/g)
来源：http://fox.gaohongyu789.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://znt.vehdjk.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rqa.jinyuanbaomall.cn

Ruby: s.scan(/\d+/)
来源：http://whs.jyoumei.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://aiv.haohaochexian.top

[I03] 提取捕获分组
来源：http://evc.wangshuangyany.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yus.ydjk.org.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rqf.sysykeji.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://koy.smart0.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fdx.haohaochexian.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://oex.zdqjudy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kgv.chenlongwang.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kit.gaohongyu789.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jkf.c1oappe.top

[I04] 正则替换
来源：http://xkt.jinghuilouyu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://nor.hesvh.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://byc.cqqwz.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nsu.ydzc1.top

TS:   s.replace(/\d+/g, "#")
来源：http://idv.yueranfly.top

Java: s.replaceAll("\\d+", "#")
来源：http://qyc.zdbjq.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pqf.uphjek.com

Ruby: s.gsub(/\d+/, "#")
来源：http://yro.guannengcc.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bpt.redwolf501.top

[I05] 按正则拆分
来源：http://aot.cashguo.top

Py:   re.split(r"\s*,\s*", s)
来源：http://hnf.sxryk.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cmh.shuidangran.top

JS:   s.split(/\s*,\s*/)
来源：http://ddv.bbcook.cn

TS:   s.split(/\s*,\s*/)
来源：http://erg.zhixingplan.top

Java: s.split("\\s*,\\s*")
来源：http://ysx.haohaochexian.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wam.jiagoushi.top

Ruby: s.split(/\s*,\s*/)
来源：http://bbe.zhoulong.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://slr.gaohongyu789.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uvh.ydjk.org.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gmh.0kj1m.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lwq.cqqwz.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lvt.c1oappe.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nkj.hcnkem.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://doj.zhaomingkeji.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mkr.hongshengwenyu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://igr.guannengcc.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vhu.fehbvm.com

[I07] 忽略大小写与多行模式
来源：http://eyt.zycfv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cxf.guowangkeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lxn.zhixingplan.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://itc.tianlin.xyz

TS:   /error/gim
来源：http://bia.nanxuanxn.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://erg.yj202588.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yon.yfazqb.com

Ruby: s.scan(/error/i)
来源：http://wbw.yj20258.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ulj.yueranfly.top

[I08] 贪婪与非贪婪匹配
来源：http://pag.yvedp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jfu.zhiwuduotai.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hbh.ydzc1.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ode.hysaishi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vkc.nanxuanxn.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://pir.sysykeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cnj.cucudq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://axn.fzhhl.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zvh.ydzc1.top

================================================================================
来源：http://kxp.aizwys.cn

J. 日期与时间
来源：http://mqy.dashuyun.cn

================================================================================
来源：http://krv.zycfv.cn

[J01] 获取当前时间
来源：http://jsp.daxiang520.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://uah.ybcxt.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wli.ehwqpu.com

JS:   new Date();  Date.now()
来源：http://ttx.guowangkeji.top

TS:   new Date();  Date.now()
来源：http://dkf.sxryk.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://coy.xinyue.icu

Go:   time.Now()
来源：http://wsa.jqgufenzy.top

Ruby: Time.now
来源：http://qkj.cucudq.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qhg.ydzc1.top

[J02] 格式化输出
来源：http://dkj.sysykeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://izx.yongpay.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vzy.yj202588.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://klw.gogol.net.cn

TS:   d.toISOString()
来源：http://gjz.guowangkeji.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yai.yj20258.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blu.birdmap.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ovt.havefunace.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yai.zycfv.cn

[J03] 字符串解析为日期
来源：http://scy.vehdjk.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cke.zycfv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://glk.haohaochexian.top

JS:   new Date("2024-01-02")
来源：http://cgd.zhaomingkeji.xyz

TS:   new Date("2024-01-02")
来源：http://dlt.hysaishi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qnj.fengsongda.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cus.gogol.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://jhp.jinyuanbaomall.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ezy.fehbvm.com

[J04] 时间戳与日期互转
来源：http://sbz.jinyuanbaomall.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hek.zhixingplan.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pmd.feifeiyinyue.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lqo.bbcook.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xxh.jqgfzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rjo.hcnkem.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://txi.feifeiyinyue.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lut.wangshuangyany.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nej.hcnkem.com

[J05] 时间加减（加 7 天）
来源：http://uju.snrcjt.cn

Py:   now + timedelta(days=7)
来源：http://pjl.hongshengwenyu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://phf.sxryk.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ebv.sysykeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ozg.guowangkeji.top

Java: LocalDate.now().plusDays(7)
来源：http://xjz.wangdashe.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gic.hnqzz.top

Ruby: Time.now + 7 * 86400
来源：http://uvd.nanxinkj.top

C#:   DateTime.Now.AddDays(7)
来源：http://ujf.aibaodan.cn

[J06] 计算两时间之差
来源：http://ixd.jinyuanbaomall.cn

Py:   (end - start).total_seconds()
来源：http://fsh.gzhubu.top

PHP:  $end->diff($start)->days;
来源：http://rln.jlsjyb.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cti.snrcjt.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nyc.yangfankeji.com

Java: Duration.between(start, end).toSeconds()
来源：http://oqn.tanke756.top

Go:   end.Sub(start).Hours()
来源：http://kfa.ywan-chungtsiang.top

Ruby: end - start                 # 返回秒数
来源：http://hvc.yj20258888.top

C#:   (end - start).TotalSeconds
来源：http://ddy.yj20258888.top

[J07] 比较两个日期
来源：http://sgi.52xcode.cn

Py:   d1 < d2;  d1 == d2
来源：http://lyn.jinqigufen.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nsd.jyoumei.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wdr.0kj1m.cn

TS:   d1.getTime() < d2.getTime()
来源：http://eqk.havefunace.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hxi.gotoacloud.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://smy.yonumen.top

Ruby: d1 < d2;  d1 == d2
来源：http://nog.gzhubu.top

C#:   d1 < d2;  d1 == d2
来源：http://del.ywan-chungtsiang.top

[J08] 提取年月日与星期
来源：http://tzi.fanxiaobao.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://myv.quarkkingdee.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zny.andypj.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://upg.yj202588.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jme.zdqjudy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wui.chenjidiqi.icu

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vxq.bbcook.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://eda.meibo888.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xha.jyoumei.cn

[J09] 时区处理
来源：http://rkj.bbcook.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jvk.cqqwz.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ktj.aizwys.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dzy.sysykeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rwq.aibaodan.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tdf.daxiang520.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://whp.kuanghao11.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://uxl.chenzaomai.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fxr.gotoacloud.top

[J10] 取今天 / 本月第一天
来源：http://zvf.zdbjq.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ajc.guowangkeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rzq.jinghuilouyu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://knb.sysykeji.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://moo.yongpay.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gra.shangyingyoupin.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ffi.yanxiufei.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vjk.dashuyun.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cld.epnwcf.com

================================================================================
来源：http://xcu.jiagoushi.top

K. JSON 与序列化
来源：http://irj.wangshuangyany.cn

================================================================================
来源：http://znq.feifeiyinyue.top

[K01] 对象转 JSON 字符串
来源：http://qkb.aizwys.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rrl.nanxinkj.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ree.fengsongda.top

JS:   JSON.stringify(obj)
来源：http://win.52xcode.cn

TS:   JSON.stringify(obj)
来源：http://qwo.nwbrower.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oba.316326.xyz

Go:   json.Marshal(obj)
来源：http://wnf.iojbl.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ebb.yueranfly.top

C#:   JsonSerializer.Serialize(obj)
来源：http://wbe.yj20258888.top

[K02] JSON 字符串转对象
来源：http://ljj.316326.xyz

Py:   json.loads(s)
来源：http://fav.chenjidiqi.icu

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://oyp.hammf.cn

JS:   JSON.parse(s)
来源：http://hal.sufxvd.cn

TS:   JSON.parse(s)
来源：http://gzy.jianghu66.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qto.kuanghao11.cn

Go:   json.Unmarshal(data, &v)
来源：http://ikn.bbcook.cn

Ruby: JSON.parse(s)
来源：http://gms.andypj.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lbw.shangyingyoupin.top

[K03] JSON 美化输出（带缩进）
来源：http://bkq.chenlongwang.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ypg.ywan-chungtsiang.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ink.0kj1m.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://khv.dashuyun.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://aun.jinqigufen.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ros.iojbl.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qyv.xylfe.cn

Ruby: JSON.pretty_generate(obj)
来源：http://iyw.fktsv.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zvc.chenlongwang.top

[K04] 读取 JSON 文件
来源：http://ojb.xziqi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lln.ywan-chungtsiang.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qxc.jiagoushi.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cmm.cqqwz.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uwm.ppjwa.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rpr.havefunace.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xdy.zhengqikj.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://zbu.fanxiaobao.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ihb.aibaodan.cn

[K05] 深拷贝对象
来源：http://jyi.fktsv.cn

Py:   copy.deepcopy(obj)
来源：http://ooc.hesvh.cn

PHP:  unserialize(serialize($obj));
来源：http://lrg.jinyuanbaomall.cn

JS:   structuredClone(obj)
来源：http://udy.shanyushiyangkeji.top

TS:   structuredClone(obj)
来源：http://sdw.ivvv.top

Java: // 手写拷贝构造，或序列化往返
来源：http://mpp.xziqi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sua.hnxiangtu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ill.nanxinkj.top

C#:   // 序列化往返，或自定义 Clone
来源：http://yfq.gogol.net.cn

[K06] 解析 URL 查询串
来源：http://hwj.ydzc1.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pus.316326.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tlg.pycfn.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kcd.jinghuilouyu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lls.nanxuanxn.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://neo.cqqwz.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pac.iojbl.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gwt.zdqjudy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hzc.mhx1999.top

[K07] 进制转换
来源：http://exl.sufxvd.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ozq.kuanghao11.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nmw.aibaodan.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dtj.jinqigfzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lua.iojbl.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fto.shuidangran.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dhg.jinqigufen.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bld.gotoacloud.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hae.kuanghao11.cn

[K08] 二进制序列化（非 JSON）
来源：http://bol.guowangkeji.top

Py:   pickle.dumps(obj)
来源：http://plr.quarkkingdee.top

PHP:  serialize($obj);  unserialize($s);
来源：http://kbl.jlsjyb.cn

JS:   v8.serialize(obj)        // Node
来源：http://ktq.haohaochexian.top

TS:   v8.serialize(obj)        // Node
来源：http://vqc.shangyingyoupin.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uok.guowangkeji.top

Go:   encoding/gob
来源：http://cqu.cqqwz.cn

Ruby: Marshal.dump(obj)
来源：http://tlr.redwolf501.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lvy.zhaomingkeji.xyz

================================================================================
来源：http://xpp.0kj1m.cn

L. 网络请求
来源：http://fsp.bjfxy.top

================================================================================
来源：http://tlw.hcnkem.com

[L01] 发送 GET 请求
来源：http://bfu.ydzc1.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ach.fanxiaobao.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bwe.zhijiandao.cn

JS:   await fetch(url)
来源：http://gpg.daria6918.cn

TS:   await fetch(url)
来源：http://xvy.feifeiyinyue.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ijp.aibaodan.cn

Go:   resp, err := http.Get(url)
来源：http://get.yonumen.top

Ruby: Net::HTTP.get(URI(url))
来源：http://lvl.xylfe.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vsh.ctjpmb.com

[L02] 发送 POST JSON
来源：http://zud.hcnkem.com

Py:   requests.post(url, json={"a": 1})
来源：http://twc.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fpo.shanyushiyangtech.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xyf.yvedp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aqk.tanke756.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kgo.haohaochexian.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zcb.quarkkingdee.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ahd.gogol.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://knk.yuanzhike.top

[L03] 设置自定义请求头
来源：http://glg.xylfe.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fif.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://edq.uphjek.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wyo.zdbjq.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://otu.dianchejie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jsq.hysaishi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nbu.yanxiufei.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ppc.fktsv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mdv.yanxiufei.cn

[L04] 设置超时
来源：http://zqj.nanxuanxn.top

Py:   requests.get(url, timeout=5)
来源：http://ooq.9152youxi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sgz.jinghuilouyu.cn


<!-- 参考信息 -->