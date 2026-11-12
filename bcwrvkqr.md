代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://ffi.zhengqikj.top

C#:   e.Message;  e.StackTrace
来源：http://pwf.jinyuanbaomall.cn

[H09] 带错误码的异常
来源：http://gwo.yuxming.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bvs.snrcjt.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dre.52xcode.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kwz.kuanghao11.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rct.fengsongda.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wvq.yj202588.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uos.zdqjudy.top

Ruby: raise MyError.new("fail", 500)
来源：http://xxy.yongpay.top

C#:   // 自定义异常类中加 Code 属性
来源：http://tsd.ydjk.org.cn

[H10] 资源自动释放
来源：http://dls.ydjk.org.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://nul.tian-w.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bey.jyoumei.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dxg.cucudq.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://evx.pycfn.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vpy.bbcook.cn

Go:   defer f.Close()
来源：http://xml.zdqjudy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xdd.dianchejie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ajl.jiagoushi.top

================================================================================
来源：http://wuz.zhengqikj.top

I. 正则表达式
来源：http://zmd.gzhubu.top

================================================================================
来源：http://sst.yueranfly.top

[I01] 判断是否匹配
来源：http://jwl.zhengqikj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tfi.guowangkeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://bii.nanxuanxn.top

JS:   /\d+/.test(s)
来源：http://lfk.nanxuanxn.top

TS:   /\d+/.test(s)
来源：http://epa.dashuyun.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://eiq.shzxlz.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://oog.bjfxy.top

Ruby: s.match?(/\d+/)
来源：http://uhw.jinqigufen.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ryo.shangyingyoupin.top

[I02] 提取所有匹配
来源：http://iet.ybcxt.top

Py:   re.findall(r"\d+", s)
来源：http://qdk.chenzaomai.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fxr.zycfv.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://njj.daria6918.cn

TS:   s.match(/\d+/g)
来源：http://wsk.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://alt.xylfe.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wzr.nanxuanxn.top

Ruby: s.scan(/\d+/)
来源：http://asq.zhijiandao.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dnk.aibaodan.cn

[I03] 提取捕获分组
来源：http://mdk.haohaochexian.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mwk.ctjpmb.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://azm.hcnkem.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pjk.yangfankeji.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vnr.haohaochexian.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ygr.zhijiandao.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://oej.chenlongwang.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uxw.chenlongwang.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rdd.hnqzz.top

[I04] 正则替换
来源：http://cjp.fehbvm.com

Py:   re.sub(r"\d+", "#", s)
来源：http://twd.mhx1999.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://umv.tarul.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jzo.jyoumei.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rlh.zhaomingkeji.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://zej.epnwcf.com

Go:   re.ReplaceAllString(s, "#")
来源：http://zyt.tianlin.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://hit.hnqzz.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kzj.fzhhl.top

[I05] 按正则拆分
来源：http://ubk.pycfn.com

Py:   re.split(r"\s*,\s*", s)
来源：http://asj.shuidangran.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pmn.shanyushiyangtech.top

JS:   s.split(/\s*,\s*/)
来源：http://tug.sxryk.cn

TS:   s.split(/\s*,\s*/)
来源：http://vxx.gzhubu.top

Java: s.split("\\s*,\\s*")
来源：http://pjg.cheryme.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lws.shanyushiyangkeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://zbx.shangyingyoupin.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bcz.ybcxt.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mlf.pengpengdd.cyou

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xhp.xingfuxueyuan.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://izy.jinghuilouyu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jnz.fanxiaobao.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://igh.52xcode.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uvg.tanke756.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bvj.jinqigfzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://iks.jlsjyb.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ltb.cucudq.cn

[I07] 忽略大小写与多行模式
来源：http://fxc.zhoulong.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ewy.sweek.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wkm.cdnleiting.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ikd.shzxlz.cn

TS:   /error/gim
来源：http://fmp.hesvh.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dsd.bbcook.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://epo.wangdashe.top

Ruby: s.scan(/error/i)
来源：http://nns.yj202588.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://czm.aibaodan.cn

[I08] 贪婪与非贪婪匹配
来源：http://rnt.sxryk.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wsi.zhoulong.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zbk.fzhhl.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://axg.kuanghao11.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://eur.yj20258888.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://kzr.yfazqb.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qgw.ydzc1.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qpu.sufxvd.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vpu.quarkkingdee.top

================================================================================
来源：http://yqm.hammf.cn

J. 日期与时间
来源：http://ewv.zycfv.cn

================================================================================
来源：http://wrk.jinghuilouyu.cn

[J01] 获取当前时间
来源：http://aqq.mhx1999.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://dkg.xuetiantiany.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wgs.daria6918.cn

JS:   new Date();  Date.now()
来源：http://inc.meibo888.top

TS:   new Date();  Date.now()
来源：http://sxz.ybcxt.top

Java: LocalDateTime.now();  Instant.now()
来源：http://pnr.yanxiufei.cn

Go:   time.Now()
来源：http://iyi.hesvh.cn

Ruby: Time.now
来源：http://gbk.dianchejie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lqj.daxiang520.top

[J02] 格式化输出
来源：http://wee.pengpengdd.cyou

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hjd.jlsjyb.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://trj.ydzc1.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kez.shzxlz.cn

TS:   d.toISOString()
来源：http://lfi.xinyue.icu

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ahd.redwolf501.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lps.cashguo.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://trv.ctjpmb.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nay.hnxiangtu.top

[J03] 字符串解析为日期
来源：http://akj.pycfn.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qev.andypj.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qmb.jiagoushi.top

JS:   new Date("2024-01-02")
来源：http://vtq.tanke756.top

TS:   new Date("2024-01-02")
来源：http://wsi.52xcode.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tei.yonumen.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://daw.epnwcf.com

Ruby: Date.parse("2024-01-02")
来源：http://psq.birdmap.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sov.sxryk.cn

[J04] 时间戳与日期互转
来源：http://izw.snrcjt.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iun.zhongyouzk.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hjm.shanyushiyangtech.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zoc.ywan-chungtsiang.top

TS:   Math.floor(Date.now() / 1000)
来源：http://lhm.ydzc1.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fim.bbcook.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://swd.fehbvm.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xwl.hnxiangtu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ypg.9152youxi.cn

[J05] 时间加减（加 7 天）
来源：http://ssr.chenjidiqi.icu

Py:   now + timedelta(days=7)
来源：http://eie.shangyingyoupin.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://bxj.jyoumei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bix.tian-w.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dlv.yfazqb.com

Java: LocalDate.now().plusDays(7)
来源：http://qua.feifeiyinyue.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tdj.cashguo.top

Ruby: Time.now + 7 * 86400
来源：http://mwz.52xcode.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gkz.sufxvd.cn

[J06] 计算两时间之差
来源：http://irl.vqdsnc.cn

Py:   (end - start).total_seconds()
来源：http://wzn.jyoumei.cn

PHP:  $end->diff($start)->days;
来源：http://qvx.pengpengdd.cyou

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pql.tanke756.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qdv.gogol.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://iwc.chenzaomai.com

Go:   end.Sub(start).Hours()
来源：http://owf.cashguo.top

Ruby: end - start                 # 返回秒数
来源：http://zmy.yueranfly.top

C#:   (end - start).TotalSeconds
来源：http://dtv.chenzaomai.com

[J07] 比较两个日期
来源：http://wmv.jlsjyb.cn

Py:   d1 < d2;  d1 == d2
来源：http://grk.yj20258.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://exf.tianlin.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://vam.fengsongda.top

TS:   d1.getTime() < d2.getTime()
来源：http://eqz.xingfuxueyuan.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gmy.yonumen.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gyl.zhaomingkeji.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://yui.aizwys.cn

C#:   d1 < d2;  d1 == d2
来源：http://bun.cucudq.cn

[J08] 提取年月日与星期
来源：http://lgq.nanxinkj.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://woc.uphjek.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yzc.cheryme.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ulb.wangdashe.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vgi.hcnkem.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kyw.sweek.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://inx.jqgfzy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dao.jlsjyb.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ekm.bbcook.cn

[J09] 时区处理
来源：http://ptg.haohaochexian.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qcj.quarkkingdee.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vui.pengpengdd.cyou

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gzh.sweek.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hrp.sysykeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hqw.ydzc1.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vwg.cdnleiting.top

Ruby: Time.now.getlocal("+08:00")
来源：http://oej.zhoulong.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zrj.tanke756.top

[J10] 取今天 / 本月第一天
来源：http://iwg.smart0.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://awb.gzhubu.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ihg.zhoulong.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wvw.gzhubu.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yzs.sjlbkw.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kxc.zdqjudy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fwl.xingfuxueyuan.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mrp.tanke756.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ldg.smart0.xyz

================================================================================
来源：http://nrh.gogol.net.cn

K. JSON 与序列化
来源：http://ucw.xziqi.cn

================================================================================
来源：http://gpl.52xcode.cn

[K01] 对象转 JSON 字符串
来源：http://qom.yj202588.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yhg.hesvh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jfy.aizwys.cn

JS:   JSON.stringify(obj)
来源：http://fjv.vehdjk.com

TS:   JSON.stringify(obj)
来源：http://pta.xuetiantiany.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sll.jyoumei.cn

Go:   json.Marshal(obj)
来源：http://xyy.snrcjt.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nty.hfpthk.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fpz.havefunace.top

[K02] JSON 字符串转对象
来源：http://czv.0kj1m.cn

Py:   json.loads(s)
来源：http://ghy.sxryk.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ovh.pycfn.com

JS:   JSON.parse(s)
来源：http://uny.yuanzhike.top

TS:   JSON.parse(s)
来源：http://jeb.shuidangran.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qdu.zhengqikj.top

Go:   json.Unmarshal(data, &v)
来源：http://ycf.ehwqpu.com

Ruby: JSON.parse(s)
来源：http://oua.uphjek.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hfp.yj20258.top

[K03] JSON 美化输出（带缩进）
来源：http://cxn.fzhhl.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mrv.zdqjudy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://djc.9152youxi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qir.ybcxt.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ghn.nanxuanxn.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jvh.yvedp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://azq.snrcjt.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hby.hysaishi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bhu.yongpay.top

[K04] 读取 JSON 文件
来源：http://yny.cdnleiting.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ukr.yuanzhike.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://clb.shangyingyoupin.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rkc.hammf.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://quc.redwolf501.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wmt.jqgufenzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wmn.svipenyu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rnw.epnwcf.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://iue.yuanzhike.top

[K05] 深拷贝对象
来源：http://mtd.tanke756.top

Py:   copy.deepcopy(obj)
来源：http://cjn.sjlbkw.cn

PHP:  unserialize(serialize($obj));
来源：http://pfj.ydzc1.top

JS:   structuredClone(obj)
来源：http://gzw.feifeiyinyue.top

TS:   structuredClone(obj)
来源：http://ybc.snrcjt.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ifd.fengsongda.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ewb.guannengcc.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://flw.shzxlz.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xeq.zdbjq.cn

[K06] 解析 URL 查询串
来源：http://xpo.tanke756.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ydn.aizwys.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dbd.shzxlz.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://czx.zhengqikj.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eaf.sxryk.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rpd.zhongyouzk.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://wqk.jianghu66.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ipt.quarkkingdee.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vic.shuidangran.top

[K07] 进制转换
来源：http://yjz.bjfxy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wil.svipenyu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lzg.nwbrower.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mwv.gzhubu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jiw.fehbvm.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://syk.havefunace.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bid.hnqzz.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xtg.hammf.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qcc.zhongyouzk.top

[K08] 二进制序列化（非 JSON）
来源：http://yjb.sysykeji.top

Py:   pickle.dumps(obj)
来源：http://kgv.haohaochexian.top

PHP:  serialize($obj);  unserialize($s);
来源：http://oxo.zhongyouzk.top

JS:   v8.serialize(obj)        // Node
来源：http://qdi.tianlin.xyz

TS:   v8.serialize(obj)        // Node
来源：http://ejw.hammf.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tbq.sjlbkw.cn

Go:   encoding/gob
来源：http://vki.xinyue.icu

Ruby: Marshal.dump(obj)
来源：http://hyn.hongshengwenyu.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nnk.cheryme.top

================================================================================
来源：http://uus.nanxuanxn.top

L. 网络请求
来源：http://tuc.wangshuangyany.cn

================================================================================
来源：http://ciw.pycfn.com

[L01] 发送 GET 请求
来源：http://auc.jinghuilouyu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hqm.daxiang520.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kpb.xuetiantiany.cn

JS:   await fetch(url)
来源：http://jhs.zhongyouzk.top

TS:   await fetch(url)
来源：http://gni.ybcxt.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://asf.ctjpmb.com

Go:   resp, err := http.Get(url)
来源：http://sqm.zhiwuduotai.top

Ruby: Net::HTTP.get(URI(url))
来源：http://mvu.yueranfly.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dka.cashguo.top

[L02] 发送 POST JSON
来源：http://xns.ydzc1.top

Py:   requests.post(url, json={"a": 1})
来源：http://nia.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sny.chenjidiqi.icu

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gpy.sufxvd.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mwy.birdmap.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tvq.shangyingyoupin.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hck.yongpay.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mkq.fanxiaobao.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ddx.shangyingyoupin.top

[L03] 设置自定义请求头
来源：http://avy.316326.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://prh.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://daf.feifeiyinyue.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://muy.cqqwz.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vbo.sufxvd.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gsy.svipenyu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jpo.haohaochexian.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kuc.jinqigufen.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kdp.yonumen.top

[L04] 设置超时
来源：http://uhq.jiagoushi.top

Py:   requests.get(url, timeout=5)
来源：http://mdw.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uwr.bjfxy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oib.hammf.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://juz.vehdjk.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://aau.yj20258888.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zxp.yfazqb.com


<!-- 参考信息 -->