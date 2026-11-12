代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://yub.zhongyouzk.top

C#:   e.Message;  e.StackTrace
来源：http://den.yj20258888.top

[H09] 带错误码的异常
来源：http://knw.fengsongda.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hvz.jiagoushi.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://xvs.sufxvd.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bfj.dianchejie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mzb.tanke756.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rxx.hfpthk.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bin.ybcxt.top

Ruby: raise MyError.new("fail", 500)
来源：http://xwj.haohaochexian.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xes.hywenlv.cn

[H10] 资源自动释放
来源：http://suv.hesvh.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ldc.havefunace.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://szq.haohaochexian.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://thb.wangdashe.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ifd.jqgufenzy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ano.cashguo.top

Go:   defer f.Close()
来源：http://xdd.yongpay.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zqy.hnxiangtu.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://swv.9152youxi.cn

================================================================================
来源：http://gtr.hammf.cn

I. 正则表达式
来源：http://ljk.kuanghao11.cn

================================================================================
来源：http://ftn.ivvv.top

[I01] 判断是否匹配
来源：http://gej.guowangkeji.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ttq.snrcjt.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vaa.xingfuxueyuan.xyz

JS:   /\d+/.test(s)
来源：http://pvt.snrcjt.cn

TS:   /\d+/.test(s)
来源：http://kkm.fzhhl.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://syc.tanke756.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gpf.yongpay.top

Ruby: s.match?(/\d+/)
来源：http://jjd.aibaodan.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hou.xinyue.icu

[I02] 提取所有匹配
来源：http://vkv.ehwqpu.com

Py:   re.findall(r"\d+", s)
来源：http://irl.dianchejie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://eed.ydzc1.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vzd.epnwcf.com

TS:   s.match(/\d+/g)
来源：http://lcs.cqqwz.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://waj.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xrh.yongpay.top

Ruby: s.scan(/\d+/)
来源：http://rru.uphjek.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ohb.vehdjk.com

[I03] 提取捕获分组
来源：http://lbm.sufxvd.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blg.316326.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://scr.hongshengwenyu.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tag.yangfankeji.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://izp.zhoulong.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://eit.nanxuanxn.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dei.jinyuanbaomall.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kvu.guowangkeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qeu.cashguo.top

[I04] 正则替换
来源：http://lok.mhx1999.top

Py:   re.sub(r"\d+", "#", s)
来源：http://afm.yj20258.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ibm.aizwys.cn

JS:   s.replace(/\d+/g, "#")
来源：http://vbx.cheryme.top

TS:   s.replace(/\d+/g, "#")
来源：http://suk.yueranfly.top

Java: s.replaceAll("\\d+", "#")
来源：http://vry.hywenlv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pda.daxiang520.top

Ruby: s.gsub(/\d+/, "#")
来源：http://tmd.zhongyouzk.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fba.yueranfly.top

[I05] 按正则拆分
来源：http://mql.zhongyouzk.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ypq.xuetiantiany.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://buq.yonumen.top

JS:   s.split(/\s*,\s*/)
来源：http://krv.zdbjq.cn

TS:   s.split(/\s*,\s*/)
来源：http://jdu.xuetiantiany.cn

Java: s.split("\\s*,\\s*")
来源：http://sah.fzhhl.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tzx.xziqi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://oiv.zycfv.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://don.shzxlz.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://txm.gotoacloud.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ghq.xziqi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dcz.jqgufenzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://clr.ppjwa.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uvm.xuetiantiany.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vya.sweek.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qzz.fengsongda.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kay.kuanghao11.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vke.xuanzx.com

[I07] 忽略大小写与多行模式
来源：http://mqn.chenzaomai.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mgo.birdmap.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yqp.yueranfly.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pob.haohaochexian.top

TS:   /error/gim
来源：http://hun.yvedp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jna.sxryk.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zwd.jyoumei.cn

Ruby: s.scan(/error/i)
来源：http://nft.zhoulong.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zdh.fengsongda.top

[I08] 贪婪与非贪婪匹配
来源：http://jea.sjlbkw.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xun.guannengcc.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kwv.quarkkingdee.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cue.zhaomingkeji.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://isb.birdmap.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://vzi.uphjek.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pgw.jinghuilouyu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://duy.svipenyu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://las.tanke756.top

================================================================================
来源：http://wxa.tian-w.cn

J. 日期与时间
来源：http://ilv.daria6918.cn

================================================================================
来源：http://zhm.yanxiufei.cn

[J01] 获取当前时间
来源：http://eae.zdqjudy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://tcq.ppjwa.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://iox.andypj.xyz

JS:   new Date();  Date.now()
来源：http://yuo.aizwys.cn

TS:   new Date();  Date.now()
来源：http://kbc.jqgfzy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://lva.jinqigufen.top

Go:   time.Now()
来源：http://vqi.kuanghao11.cn

Ruby: Time.now
来源：http://jvw.fzhhl.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nau.mhx1999.top

[J02] 格式化输出
来源：http://vhe.jqgufenzy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sth.yvedp.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wjn.yvedp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pco.jqgufenzy.top

TS:   d.toISOString()
来源：http://zgq.zhengqikj.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mat.shangyingyoupin.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vuv.ydjk.org.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zqk.fktsv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xdm.shangyingyoupin.top

[J03] 字符串解析为日期
来源：http://ekm.zdqjudy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lym.chenjidiqi.icu

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://izl.fehbvm.com

JS:   new Date("2024-01-02")
来源：http://ljj.fktsv.cn

TS:   new Date("2024-01-02")
来源：http://jkg.yangfankeji.com

Java: LocalDate.parse("2024-01-02")
来源：http://iin.yongpay.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qpo.guannengcc.top

Ruby: Date.parse("2024-01-02")
来源：http://fid.ydzc1.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cuf.yuxming.cn

[J04] 时间戳与日期互转
来源：http://ect.yueranfly.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xol.hywenlv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ryi.hywenlv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://moe.hysaishi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://znx.hammf.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ynx.yanxiufei.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vdy.wangdashe.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tru.gogol.net.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lkn.ivvv.top

[J05] 时间加减（加 7 天）
来源：http://aeo.jinyuanbaomall.cn

Py:   now + timedelta(days=7)
来源：http://ged.ydjk.org.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yav.ehwqpu.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cky.pengpengdd.cyou

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bpk.chenjidiqi.icu

Java: LocalDate.now().plusDays(7)
来源：http://jsg.mhx1999.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xkb.andypj.xyz

Ruby: Time.now + 7 * 86400
来源：http://qkh.pycfn.com

C#:   DateTime.Now.AddDays(7)
来源：http://yfh.ehwqpu.com

[J06] 计算两时间之差
来源：http://xpn.vqdsnc.cn

Py:   (end - start).total_seconds()
来源：http://khp.ehwqpu.com

PHP:  $end->diff($start)->days;
来源：http://msz.nanxinkj.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bfl.mhx1999.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vxc.316326.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://yni.yangfankeji.com

Go:   end.Sub(start).Hours()
来源：http://hhq.birdmap.top

Ruby: end - start                 # 返回秒数
来源：http://dyi.svipenyu.cn

C#:   (end - start).TotalSeconds
来源：http://pxr.fehbvm.com

[J07] 比较两个日期
来源：http://vqp.yangfankeji.com

Py:   d1 < d2;  d1 == d2
来源：http://dbs.chenzaomai.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zhf.dianchejie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://sjw.xingfuxueyuan.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://xte.nanxinkj.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://axz.ehwqpu.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xhr.pengpengdd.cyou

Ruby: d1 < d2;  d1 == d2
来源：http://sar.cashguo.top

C#:   d1 < d2;  d1 == d2
来源：http://dlc.yj20258.top

[J08] 提取年月日与星期
来源：http://ddm.sjlbkw.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wsk.yanxiufei.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kmp.gaohongyu789.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bhr.tarul.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fke.svipenyu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://seg.zhoulong.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vqp.ehwqpu.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qvf.yonumen.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ewe.chenjidiqi.icu

[J09] 时区处理
来源：http://wfp.aibaodan.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vbc.hesvh.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rpm.shanyushiyangtech.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vif.tarul.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zzf.gogol.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://btj.xylfe.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://eij.chenlongwang.top

Ruby: Time.now.getlocal("+08:00")
来源：http://dwv.epnwcf.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://iri.hongshengwenyu.top

[J10] 取今天 / 本月第一天
来源：http://gcf.gotoacloud.top

Py:   date.today();  date.today().replace(day=1)
来源：http://mcy.ydjk.org.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://myp.zhengqikj.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://veh.cheryme.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vrf.zhongyouzk.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ply.xylfe.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://thm.zhoulong.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xig.sufxvd.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nnd.chenlongwang.top

================================================================================
来源：http://ppd.xuanzx.com

K. JSON 与序列化
来源：http://jmv.kuanghao11.cn

================================================================================
来源：http://ful.zhiwuduotai.top

[K01] 对象转 JSON 字符串
来源：http://uce.zycfv.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xvr.316326.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ssc.fehbvm.com

JS:   JSON.stringify(obj)
来源：http://uhl.birdmap.top

TS:   JSON.stringify(obj)
来源：http://ztu.yongpay.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uij.sufxvd.cn

Go:   json.Marshal(obj)
来源：http://odq.xuanzx.com

Ruby: obj.to_json                                     // require "json"
来源：http://jcz.mhx1999.top

C#:   JsonSerializer.Serialize(obj)
来源：http://jgg.pycfn.com

[K02] JSON 字符串转对象
来源：http://bph.cucudq.cn

Py:   json.loads(s)
来源：http://yfm.yj20258.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://eyl.shangyingyoupin.top

JS:   JSON.parse(s)
来源：http://xlm.havefunace.top

TS:   JSON.parse(s)
来源：http://tfd.jiagoushi.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://alk.tanke756.top

Go:   json.Unmarshal(data, &v)
来源：http://wld.hcnkem.com

Ruby: JSON.parse(s)
来源：http://uoe.fehbvm.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ssv.zhengqikj.top

[K03] JSON 美化输出（带缩进）
来源：http://vgp.sysykeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bag.wangshuangyany.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qbc.sysykeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://usx.fktsv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://iwv.shzxlz.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ugx.smart0.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lhq.jinghuilouyu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hrv.sxryk.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nwg.cqqwz.cn

[K04] 读取 JSON 文件
来源：http://hkg.hcnkem.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kij.chenjidiqi.icu

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://idq.daxiang520.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ijp.jqgufenzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sqr.yj20258888.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ele.dashuyun.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vgp.yanxiufei.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vyo.wangshuangyany.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qwf.cqqwz.cn

[K05] 深拷贝对象
来源：http://cjk.gzhubu.top

Py:   copy.deepcopy(obj)
来源：http://ffy.guowangkeji.top

PHP:  unserialize(serialize($obj));
来源：http://zog.svipenyu.cn

JS:   structuredClone(obj)
来源：http://nbd.shanyushiyangtech.top

TS:   structuredClone(obj)
来源：http://jkb.fktsv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kqk.9152youxi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lwx.gaohongyu789.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dci.mhx1999.top

C#:   // 序列化往返，或自定义 Clone
来源：http://zho.52xcode.cn

[K06] 解析 URL 查询串
来源：http://mcb.tanke756.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dvy.yuanzhike.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ihl.tarul.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fjv.daria6918.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wbd.xingfuxueyuan.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bag.daxiang520.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://pcs.dianchejie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vdi.yvedp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://chs.yj20258.top

[K07] 进制转换
来源：http://yji.sysykeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://aws.ivvv.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wry.snrcjt.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pkq.shanyushiyangtech.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kdt.redwolf501.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fwp.uphjek.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://elb.guowangkeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dzd.vehdjk.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ubp.pycfn.com

[K08] 二进制序列化（非 JSON）
来源：http://xdr.sufxvd.cn

Py:   pickle.dumps(obj)
来源：http://auk.zhaomingkeji.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://qsj.hongshengwenyu.top

JS:   v8.serialize(obj)        // Node
来源：http://asv.zdbjq.cn

TS:   v8.serialize(obj)        // Node
来源：http://ykg.cqqwz.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://npn.uphjek.com

Go:   encoding/gob
来源：http://qgb.yj20258.top

Ruby: Marshal.dump(obj)
来源：http://cag.bjfxy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://esm.vqdsnc.cn

================================================================================
来源：http://rgb.sweek.top

L. 网络请求
来源：http://mdh.yj20258.top

================================================================================
来源：http://xug.xuetiantiany.cn

[L01] 发送 GET 请求
来源：http://svf.fzhhl.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://grs.shangyingyoupin.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yhb.xziqi.cn

JS:   await fetch(url)
来源：http://hab.ppjwa.cn

TS:   await fetch(url)
来源：http://odd.chenlongwang.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://iig.chenlongwang.top

Go:   resp, err := http.Get(url)
来源：http://vte.yj20258.top

Ruby: Net::HTTP.get(URI(url))
来源：http://eyf.yanxiufei.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gbt.jqgufenzy.top

[L02] 发送 POST JSON
来源：http://pfd.smart0.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://pzs.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tif.fehbvm.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jgk.hywenlv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ahg.tarul.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ytc.cheryme.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ozc.wangshuangyany.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gnh.gaohongyu789.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pal.xziqi.cn

[L03] 设置自定义请求头
来源：http://ikh.hongshengwenyu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tfl.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qsb.jinghuilouyu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uux.jqgfzy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xsa.ywan-chungtsiang.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mjj.yongpay.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://asq.hcnkem.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://noc.pycfn.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wqe.zhongyouzk.top

[L04] 设置超时
来源：http://iyg.svipenyu.cn

Py:   requests.get(url, timeout=5)
来源：http://koc.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mgt.yuxming.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qho.zhaomingkeji.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qlx.yfazqb.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gtc.tanke756.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wib.havefunace.top


<!-- 参考信息 -->