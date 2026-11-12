代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://nna.feifeiyinyue.top

C#:   e.Message;  e.StackTrace
来源：http://fhg.aizwys.cn

[H09] 带错误码的异常
来源：http://pix.dashuyun.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lnx.iojbl.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cec.nanxuanxn.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hxe.fengsongda.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jql.tian-w.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qhm.zycfv.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rdw.aizwys.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xkt.yongpay.top

C#:   // 自定义异常类中加 Code 属性
来源：http://gda.ehwqpu.com

[H10] 资源自动释放
来源：http://uhe.yj20258888.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://gzf.zhoulong.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://woh.cqqwz.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kpk.cqqwz.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rah.9152youxi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tvd.mhx1999.top

Go:   defer f.Close()
来源：http://vrm.havefunace.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://afe.yongpay.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://isz.hesvh.cn

================================================================================
来源：http://sna.gzhubu.top

I. 正则表达式
来源：http://xse.xylfe.cn

================================================================================
来源：http://mje.jianghu66.top

[I01] 判断是否匹配
来源：http://acr.yongpay.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nlk.bbcook.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vft.pycfn.com

JS:   /\d+/.test(s)
来源：http://una.bjfxy.top

TS:   /\d+/.test(s)
来源：http://zys.xingfuxueyuan.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://otq.gaohongyu789.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lzb.vqdsnc.cn

Ruby: s.match?(/\d+/)
来源：http://djy.chenjidiqi.icu

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gtz.xuanzx.com

[I02] 提取所有匹配
来源：http://lrv.9152youxi.cn

Py:   re.findall(r"\d+", s)
来源：http://veg.aibaodan.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://usu.cucudq.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zsc.tarul.cn

TS:   s.match(/\d+/g)
来源：http://jwd.yonumen.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wrr.yj20258888.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://krj.tanke756.top

Ruby: s.scan(/\d+/)
来源：http://rjp.ybcxt.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wmv.kuanghao11.cn

[I03] 提取捕获分组
来源：http://amg.nanxinkj.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vcl.zycfv.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kfy.hfpthk.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://var.iojbl.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ehu.smart0.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wzr.shzxlz.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://eol.zhongyouzk.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://myk.tianlin.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://iqd.nwbrower.top

[I04] 正则替换
来源：http://cul.haohaochexian.top

Py:   re.sub(r"\d+", "#", s)
来源：http://oky.pycfn.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://grv.yvedp.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jzu.yj202588.top

TS:   s.replace(/\d+/g, "#")
来源：http://bpm.zhijiandao.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ujy.yj20258888.top

Go:   re.ReplaceAllString(s, "#")
来源：http://zjm.yfazqb.com

Ruby: s.gsub(/\d+/, "#")
来源：http://dki.yj20258.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://oei.guannengcc.top

[I05] 按正则拆分
来源：http://lkt.shanyushiyangtech.top

Py:   re.split(r"\s*,\s*", s)
来源：http://cch.gzhubu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nho.0kj1m.cn

JS:   s.split(/\s*,\s*/)
来源：http://aob.fzhhl.top

TS:   s.split(/\s*,\s*/)
来源：http://cvw.ybcxt.top

Java: s.split("\\s*,\\s*")
来源：http://rtk.zhengqikj.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ejw.jinqigfzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://hqj.yj20258.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://icp.zhengqikj.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mbe.yfazqb.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fhq.chenlongwang.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jnk.cucudq.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cqe.birdmap.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yjy.cdnleiting.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ahp.aizwys.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zgh.svipenyu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hhu.hysaishi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sul.gaohongyu789.top

[I07] 忽略大小写与多行模式
来源：http://byy.zhongyouzk.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rmz.daxiang520.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nix.9152youxi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://eyt.aibaodan.cn

TS:   /error/gim
来源：http://dds.gogol.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zdn.c1oappe.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xkd.zycfv.cn

Ruby: s.scan(/error/i)
来源：http://qll.zhoulong.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yjo.feifeiyinyue.top

[I08] 贪婪与非贪婪匹配
来源：http://tis.nanxuanxn.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zab.quarkkingdee.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xtw.ywan-chungtsiang.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://llk.chenlongwang.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://eyi.hfpthk.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://urb.chenzaomai.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dqh.fzhhl.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xhx.shangyingyoupin.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bpc.daxiang520.top

================================================================================
来源：http://fql.ehwqpu.com

J. 日期与时间
来源：http://ssk.guowangkeji.top

================================================================================
来源：http://ctd.jyoumei.cn

[J01] 获取当前时间
来源：http://vlm.cdnleiting.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://gew.hcnkem.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hjq.jinghuilouyu.cn

JS:   new Date();  Date.now()
来源：http://pmx.tian-w.cn

TS:   new Date();  Date.now()
来源：http://xwz.yonumen.top

Java: LocalDateTime.now();  Instant.now()
来源：http://aml.hfpthk.cn

Go:   time.Now()
来源：http://why.yongpay.top

Ruby: Time.now
来源：http://ckd.zhongyouzk.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xcb.tian-w.cn

[J02] 格式化输出
来源：http://jqn.jyoumei.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://chw.ywan-chungtsiang.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kps.tarul.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://imw.andypj.xyz

TS:   d.toISOString()
来源：http://osb.jinyuanbaomall.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jnl.fanxiaobao.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jun.sufxvd.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sag.shanyushiyangkeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tmm.dianchejie.cn

[J03] 字符串解析为日期
来源：http://dcm.316326.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jgx.aibaodan.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wmd.gzhubu.top

JS:   new Date("2024-01-02")
来源：http://awn.yongpay.top

TS:   new Date("2024-01-02")
来源：http://jwb.fanxiaobao.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://okl.yongpay.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xcw.ppjwa.cn

Ruby: Date.parse("2024-01-02")
来源：http://foo.gogol.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://eho.ydzc1.top

[J04] 时间戳与日期互转
来源：http://qua.shuidangran.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zch.nanxinkj.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dxe.hnxiangtu.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kqt.gzhubu.top

TS:   Math.floor(Date.now() / 1000)
来源：http://pkn.vqdsnc.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dtv.svipenyu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nwr.xziqi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://idq.redwolf501.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rcw.0kj1m.cn

[J05] 时间加减（加 7 天）
来源：http://ghb.chenlongwang.top

Py:   now + timedelta(days=7)
来源：http://eoz.nanxinkj.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://pbq.meibo888.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vhe.yvedp.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bld.yfazqb.com

Java: LocalDate.now().plusDays(7)
来源：http://jkv.xuetiantiany.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mjv.yonumen.top

Ruby: Time.now + 7 * 86400
来源：http://vjq.nanxuanxn.top

C#:   DateTime.Now.AddDays(7)
来源：http://zvh.hysaishi.cn

[J06] 计算两时间之差
来源：http://mei.gotoacloud.top

Py:   (end - start).total_seconds()
来源：http://lrv.cashguo.top

PHP:  $end->diff($start)->days;
来源：http://tkh.bjfxy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://crt.jyoumei.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rsy.quarkkingdee.top

Java: Duration.between(start, end).toSeconds()
来源：http://bdi.hywenlv.cn

Go:   end.Sub(start).Hours()
来源：http://ozq.zdqjudy.top

Ruby: end - start                 # 返回秒数
来源：http://jrw.zdqjudy.top

C#:   (end - start).TotalSeconds
来源：http://xaf.bbcook.cn

[J07] 比较两个日期
来源：http://eqn.cheryme.top

Py:   d1 < d2;  d1 == d2
来源：http://tty.yvedp.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://oxn.xziqi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dxg.jqgfzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://psn.ydjk.org.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gau.zhijiandao.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://oiu.0kj1m.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kni.yvedp.cn

C#:   d1 < d2;  d1 == d2
来源：http://yqp.zhengqikj.top

[J08] 提取年月日与星期
来源：http://cll.yj202588.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cjd.pycfn.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zcu.vehdjk.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ybg.hesvh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://psx.zdqjudy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tio.zhiwuduotai.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mna.bbcook.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vcn.jinghuilouyu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ewm.chenlongwang.top

[J09] 时区处理
来源：http://qws.yuanzhike.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kug.xuetiantiany.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://iba.hfpthk.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mcw.sweek.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kre.zhaomingkeji.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sao.yueranfly.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ovn.jqgufenzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://dga.redwolf501.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sac.xinyue.icu

[J10] 取今天 / 本月第一天
来源：http://kem.cucudq.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://iea.nanxinkj.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rcg.sxryk.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sti.havefunace.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gsv.zhengqikj.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rrk.tianlin.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ryf.havefunace.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ium.yangfankeji.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lsq.wangdashe.top

================================================================================
来源：http://lsa.zdqjudy.top

K. JSON 与序列化
来源：http://jdq.hesvh.cn

================================================================================
来源：http://hbx.yongpay.top

[K01] 对象转 JSON 字符串
来源：http://rvl.jiagoushi.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dfj.yj20258.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xvh.yongpay.top

JS:   JSON.stringify(obj)
来源：http://fyt.nwbrower.top

TS:   JSON.stringify(obj)
来源：http://oix.bbcook.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gam.sjlbkw.cn

Go:   json.Marshal(obj)
来源：http://dmx.quarkkingdee.top

Ruby: obj.to_json                                     // require "json"
来源：http://mgj.nanxinkj.top

C#:   JsonSerializer.Serialize(obj)
来源：http://hyh.zhaomingkeji.xyz

[K02] JSON 字符串转对象
来源：http://xrx.gotoacloud.top

Py:   json.loads(s)
来源：http://npn.yanxiufei.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://aah.vehdjk.com

JS:   JSON.parse(s)
来源：http://tcm.sufxvd.cn

TS:   JSON.parse(s)
来源：http://zdg.hongshengwenyu.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lmn.iojbl.cn

Go:   json.Unmarshal(data, &v)
来源：http://veq.yj202588.top

Ruby: JSON.parse(s)
来源：http://hyi.mhx1999.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://esx.cqqwz.cn

[K03] JSON 美化输出（带缩进）
来源：http://gkn.shzxlz.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cry.hywenlv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://uig.xylfe.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gjb.jinghuilouyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nxr.xziqi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mta.ctjpmb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://evy.zhiwuduotai.top

Ruby: JSON.pretty_generate(obj)
来源：http://hsh.xinyue.icu

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jai.gzhubu.top

[K04] 读取 JSON 文件
来源：http://ovx.hcnkem.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lzw.chenzaomai.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yar.fehbvm.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hhx.chenzaomai.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ajg.jqgufenzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fej.zhaomingkeji.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dsl.c1oappe.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://lbp.redwolf501.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://env.bjfxy.top

[K05] 深拷贝对象
来源：http://glx.jiagoushi.top

Py:   copy.deepcopy(obj)
来源：http://ove.pengpengdd.cyou

PHP:  unserialize(serialize($obj));
来源：http://mqv.0kj1m.cn

JS:   structuredClone(obj)
来源：http://uwm.shangyingyoupin.top

TS:   structuredClone(obj)
来源：http://jtz.jlsjyb.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qdw.dianchejie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://twa.shangyingyoupin.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mlb.zhaomingkeji.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://vkx.vqdsnc.cn

[K06] 解析 URL 查询串
来源：http://vtv.daria6918.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qtf.316326.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://owm.gzhubu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zlr.xuetiantiany.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gnw.wangdashe.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bcb.jianghu66.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://nqc.nanxuanxn.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://map.yanxiufei.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gqt.hysaishi.cn

[K07] 进制转换
来源：http://kee.chenzaomai.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uyr.gaohongyu789.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cey.jlsjyb.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rjc.hnqzz.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://asi.xuanzx.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vem.ehwqpu.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rhf.yj202588.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ztp.cqqwz.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fwh.hnqzz.top

[K08] 二进制序列化（非 JSON）
来源：http://aes.shzxlz.cn

Py:   pickle.dumps(obj)
来源：http://vve.ppjwa.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://uhe.shuidangran.top

JS:   v8.serialize(obj)        // Node
来源：http://jpy.vehdjk.com

TS:   v8.serialize(obj)        // Node
来源：http://nct.ppjwa.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tyi.ppjwa.cn

Go:   encoding/gob
来源：http://pll.0kj1m.cn

Ruby: Marshal.dump(obj)
来源：http://ipl.sufxvd.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gby.ywan-chungtsiang.top

================================================================================
来源：http://ryp.sxryk.cn

L. 网络请求
来源：http://zme.yanxiufei.cn

================================================================================
来源：http://way.shzxlz.cn

[L01] 发送 GET 请求
来源：http://fdv.gaohongyu789.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://smv.ivvv.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yzf.sjlbkw.cn

JS:   await fetch(url)
来源：http://bqr.iojbl.cn

TS:   await fetch(url)
来源：http://gcx.jiagoushi.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://unz.tarul.cn

Go:   resp, err := http.Get(url)
来源：http://lfp.mhx1999.top

Ruby: Net::HTTP.get(URI(url))
来源：http://fdu.wangshuangyany.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ezf.ehwqpu.com

[L02] 发送 POST JSON
来源：http://bat.yuxming.cn

Py:   requests.post(url, json={"a": 1})
来源：http://geu.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://szv.wangdashe.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lyh.yueranfly.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qsi.zdbjq.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ygo.shuidangran.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://odb.zhongyouzk.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://iib.ivvv.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sjd.zycfv.cn

[L03] 设置自定义请求头
来源：http://vut.fehbvm.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nfu.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zjo.cashguo.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nza.havefunace.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fxi.shangyingyoupin.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ffr.9152youxi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qao.pengpengdd.cyou

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ifj.hnqzz.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cws.daria6918.cn

[L04] 设置超时
来源：http://vsu.aibaodan.cn

Py:   requests.get(url, timeout=5)
来源：http://zxn.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://muh.ydjk.org.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jcj.quarkkingdee.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cjr.ydjk.org.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fns.ehwqpu.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lat.chenjidiqi.icu


<!-- 参考信息 -->