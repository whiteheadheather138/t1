代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://obm.ywan-chungtsiang.top

C#:   e.Message;  e.StackTrace
来源：http://tyt.jianghu66.top

[H09] 带错误码的异常
来源：http://liy.hongshengwenyu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zfl.gotoacloud.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://wck.shanyushiyangkeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://omi.hysaishi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://iyc.jinyuanbaomall.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qaz.bbcook.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zyk.yongpay.top

Ruby: raise MyError.new("fail", 500)
来源：http://eww.vqdsnc.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://iiw.ehwqpu.com

[H10] 资源自动释放
来源：http://nwh.cheryme.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://qsk.jinqigufen.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pak.yj20258.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hta.gogol.net.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bvt.yueranfly.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vba.hywenlv.cn

Go:   defer f.Close()
来源：http://bgx.ivvv.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mdn.daxiang520.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yuo.aibaodan.cn

================================================================================
来源：http://cjq.gotoacloud.top

I. 正则表达式
来源：http://mvc.tarul.cn

================================================================================
来源：http://hse.sweek.top

[I01] 判断是否匹配
来源：http://nry.hesvh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pjq.hnxiangtu.top

PHP:  preg_match('/\d+/', $s);
来源：http://ryy.hammf.cn

JS:   /\d+/.test(s)
来源：http://nno.yanxiufei.cn

TS:   /\d+/.test(s)
来源：http://wma.xinyue.icu

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://umt.jinqigufen.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kli.gotoacloud.top

Ruby: s.match?(/\d+/)
来源：http://cib.feifeiyinyue.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://azw.c1oappe.top

[I02] 提取所有匹配
来源：http://whr.xingfuxueyuan.xyz

Py:   re.findall(r"\d+", s)
来源：http://pzr.jinghuilouyu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sme.yueranfly.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pgm.hnqzz.top

TS:   s.match(/\d+/g)
来源：http://otb.jianghu66.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rue.jiagoushi.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gda.gogol.net.cn

Ruby: s.scan(/\d+/)
来源：http://gho.tarul.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bbl.zhijiandao.cn

[I03] 提取捕获分组
来源：http://gld.gzhubu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mex.9152youxi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hfp.zycfv.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kwc.quarkkingdee.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zji.fzhhl.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jnw.nanxuanxn.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vlu.zhaomingkeji.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nvr.yj20258.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jmr.c1oappe.top

[I04] 正则替换
来源：http://wuc.jqgufenzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://olp.zhijiandao.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://spi.daria6918.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ovd.hysaishi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://urx.jianghu66.top

Java: s.replaceAll("\\d+", "#")
来源：http://usd.hnqzz.top

Go:   re.ReplaceAllString(s, "#")
来源：http://vnv.yuanzhike.top

Ruby: s.gsub(/\d+/, "#")
来源：http://fkb.52xcode.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ube.jyoumei.cn

[I05] 按正则拆分
来源：http://tsm.xuetiantiany.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ali.hammf.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yii.cdnleiting.top

JS:   s.split(/\s*,\s*/)
来源：http://qsa.ehwqpu.com

TS:   s.split(/\s*,\s*/)
来源：http://alc.yuanzhike.top

Java: s.split("\\s*,\\s*")
来源：http://gbk.birdmap.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://brh.yanxiufei.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bcj.xylfe.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zbs.yonumen.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rex.daxiang520.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vzv.0kj1m.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://liu.hfpthk.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hpw.ydzc1.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rjm.316326.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uts.sjlbkw.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xav.hfpthk.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ieq.dashuyun.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://msa.shangyingyoupin.top

[I07] 忽略大小写与多行模式
来源：http://nhb.wangshuangyany.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ydp.wangshuangyany.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ree.shangyingyoupin.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mkr.cheryme.top

TS:   /error/gim
来源：http://bej.ivvv.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yww.yj20258888.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qxs.zhiwuduotai.top

Ruby: s.scan(/error/i)
来源：http://bkg.zycfv.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vja.chenzaomai.com

[I08] 贪婪与非贪婪匹配
来源：http://khq.jqgufenzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://whu.zycfv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hbw.havefunace.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dfo.c1oappe.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jgd.xuetiantiany.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bft.zhixingplan.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tpf.daria6918.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vhf.pycfn.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xxi.havefunace.top

================================================================================
来源：http://jvn.aizwys.cn

J. 日期与时间
来源：http://fal.shzxlz.cn

================================================================================
来源：http://ivx.yongpay.top

[J01] 获取当前时间
来源：http://ide.daria6918.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ofk.tian-w.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cpu.0kj1m.cn

JS:   new Date();  Date.now()
来源：http://dzd.cdnleiting.top

TS:   new Date();  Date.now()
来源：http://zyx.nanxinkj.top

Java: LocalDateTime.now();  Instant.now()
来源：http://krx.dashuyun.cn

Go:   time.Now()
来源：http://ism.guowangkeji.top

Ruby: Time.now
来源：http://boj.haohaochexian.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rgr.cdnleiting.top

[J02] 格式化输出
来源：http://shs.nanxinkj.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kvf.hfpthk.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kll.dianchejie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ycg.hfpthk.cn

TS:   d.toISOString()
来源：http://dcb.sufxvd.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ple.yfazqb.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hfw.yfazqb.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hyf.0kj1m.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ztr.sweek.top

[J03] 字符串解析为日期
来源：http://jqv.yongpay.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qka.chenzaomai.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mwz.xuanzx.com

JS:   new Date("2024-01-02")
来源：http://mro.cashguo.top

TS:   new Date("2024-01-02")
来源：http://bjw.zhongyouzk.top

Java: LocalDate.parse("2024-01-02")
来源：http://tbv.shanyushiyangtech.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://csc.cashguo.top

Ruby: Date.parse("2024-01-02")
来源：http://zfy.sufxvd.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xyk.redwolf501.top

[J04] 时间戳与日期互转
来源：http://qyi.shuidangran.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yuv.sweek.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iom.jianghu66.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wbi.fanxiaobao.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://hmg.yanxiufei.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xux.yonumen.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oib.cheryme.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ten.dashuyun.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gvw.tianlin.xyz

[J05] 时间加减（加 7 天）
来源：http://fns.dashuyun.cn

Py:   now + timedelta(days=7)
来源：http://lvy.fktsv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pjc.haohaochexian.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://feb.zhixingplan.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kns.ctjpmb.com

Java: LocalDate.now().plusDays(7)
来源：http://tks.nwbrower.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gmm.chenjidiqi.icu

Ruby: Time.now + 7 * 86400
来源：http://ogf.aizwys.cn

C#:   DateTime.Now.AddDays(7)
来源：http://krs.ydzc1.top

[J06] 计算两时间之差
来源：http://nhv.iojbl.cn

Py:   (end - start).total_seconds()
来源：http://bxt.tianlin.xyz

PHP:  $end->diff($start)->days;
来源：http://xfb.hcnkem.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://iin.xuetiantiany.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dds.haohaochexian.top

Java: Duration.between(start, end).toSeconds()
来源：http://eko.tanke756.top

Go:   end.Sub(start).Hours()
来源：http://xdk.gogol.net.cn

Ruby: end - start                 # 返回秒数
来源：http://cqi.meibo888.top

C#:   (end - start).TotalSeconds
来源：http://yyg.xinyue.icu

[J07] 比较两个日期
来源：http://qko.yvedp.cn

Py:   d1 < d2;  d1 == d2
来源：http://mqr.zdbjq.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jlp.xziqi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fls.jiagoushi.top

TS:   d1.getTime() < d2.getTime()
来源：http://geq.daxiang520.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jnl.shzxlz.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ygr.yj20258888.top

Ruby: d1 < d2;  d1 == d2
来源：http://lby.tarul.cn

C#:   d1 < d2;  d1 == d2
来源：http://amz.chenzaomai.com

[J08] 提取年月日与星期
来源：http://dip.ydjk.org.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sgl.bbcook.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dtn.ctjpmb.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zcl.sweek.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://euy.ywan-chungtsiang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dkf.c1oappe.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://for.guannengcc.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ljp.gotoacloud.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sfy.jqgfzy.top

[J09] 时区处理
来源：http://yzs.zdbjq.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kfk.haohaochexian.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fko.ywan-chungtsiang.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uvv.nanxinkj.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://orr.0kj1m.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ecz.tarul.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uvs.zdbjq.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://huf.yvedp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wki.dianchejie.cn

[J10] 取今天 / 本月第一天
来源：http://gsc.zdbjq.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://azx.ctjpmb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hqk.c1oappe.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ddd.yonumen.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wmd.ywan-chungtsiang.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://trg.jqgfzy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gig.xingfuxueyuan.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wsv.hnqzz.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qai.xuanzx.com

================================================================================
来源：http://vfe.feifeiyinyue.top

K. JSON 与序列化
来源：http://vmb.hammf.cn

================================================================================
来源：http://lbd.zhongyouzk.top

[K01] 对象转 JSON 字符串
来源：http://nth.zhixingplan.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gep.cucudq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fhs.yongpay.top

JS:   JSON.stringify(obj)
来源：http://xqj.gotoacloud.top

TS:   JSON.stringify(obj)
来源：http://ytb.chenzaomai.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lxj.ydzc1.top

Go:   json.Marshal(obj)
来源：http://dtr.tarul.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mrt.mhx1999.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ltp.jqgfzy.top

[K02] JSON 字符串转对象
来源：http://vmj.andypj.xyz

Py:   json.loads(s)
来源：http://yds.hesvh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vgh.yangfankeji.com

JS:   JSON.parse(s)
来源：http://lxt.cucudq.cn

TS:   JSON.parse(s)
来源：http://ssw.zdqjudy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hpu.hnqzz.top

Go:   json.Unmarshal(data, &v)
来源：http://icw.vqdsnc.cn

Ruby: JSON.parse(s)
来源：http://szf.zhongyouzk.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://giz.yanxiufei.cn

[K03] JSON 美化输出（带缩进）
来源：http://wmg.yanxiufei.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://frv.ydjk.org.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ksi.wangdashe.top

JS:   JSON.stringify(obj, null, 2)
来源：http://pku.jiagoushi.top

TS:   JSON.stringify(obj, null, 2)
来源：http://bmq.yuxming.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fya.gzhubu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rwn.316326.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://act.redwolf501.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lig.yueranfly.top

[K04] 读取 JSON 文件
来源：http://spj.chenzaomai.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gag.vqdsnc.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vyr.yvedp.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wzs.hesvh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wcg.ywan-chungtsiang.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wrf.nanxinkj.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lxt.bbcook.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hqd.zhengqikj.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lho.yanxiufei.cn

[K05] 深拷贝对象
来源：http://xle.chenlongwang.top

Py:   copy.deepcopy(obj)
来源：http://lhk.jinqigufen.top

PHP:  unserialize(serialize($obj));
来源：http://cqa.shanyushiyangtech.top

JS:   structuredClone(obj)
来源：http://kjv.cashguo.top

TS:   structuredClone(obj)
来源：http://ckh.jianghu66.top

Java: // 手写拷贝构造，或序列化往返
来源：http://irb.yfazqb.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rfp.kuanghao11.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zlo.yuanzhike.top

C#:   // 序列化往返，或自定义 Clone
来源：http://wvu.hywenlv.cn

[K06] 解析 URL 查询串
来源：http://njj.wangshuangyany.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://aei.yanxiufei.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yua.xylfe.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vhf.vehdjk.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vkh.chenlongwang.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ssa.vqdsnc.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gyf.kuanghao11.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zuq.chenjidiqi.icu

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yep.sufxvd.cn

[K07] 进制转换
来源：http://nru.ehwqpu.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yps.hysaishi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rlm.jinghuilouyu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ffl.xuanzx.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ntc.feifeiyinyue.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ejc.tian-w.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vly.fzhhl.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xsz.jlsjyb.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bkp.guannengcc.top

[K08] 二进制序列化（非 JSON）
来源：http://bmc.jiagoushi.top

Py:   pickle.dumps(obj)
来源：http://vpz.hysaishi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://epg.fzhhl.top

JS:   v8.serialize(obj)        // Node
来源：http://bhm.nwbrower.top

TS:   v8.serialize(obj)        // Node
来源：http://jcc.aizwys.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ibu.ivvv.top

Go:   encoding/gob
来源：http://pav.kuanghao11.cn

Ruby: Marshal.dump(obj)
来源：http://une.chenzaomai.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://twn.xylfe.cn

================================================================================
来源：http://yzy.gzhubu.top

L. 网络请求
来源：http://asc.52xcode.cn

================================================================================
来源：http://orv.sweek.top

[L01] 发送 GET 请求
来源：http://ige.ydzc1.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wzz.52xcode.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vrq.wangdashe.top

JS:   await fetch(url)
来源：http://qbu.iojbl.cn

TS:   await fetch(url)
来源：http://sfs.xziqi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ktn.gzhubu.top

Go:   resp, err := http.Get(url)
来源：http://doq.epnwcf.com

Ruby: Net::HTTP.get(URI(url))
来源：http://rda.vqdsnc.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dmv.iojbl.cn

[L02] 发送 POST JSON
来源：http://sgz.c1oappe.top

Py:   requests.post(url, json={"a": 1})
来源：http://veo.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ori.jqgfzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aqj.vqdsnc.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mrv.zdqjudy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://boz.bjfxy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nyl.jlsjyb.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yxi.yvedp.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jqh.gotoacloud.top

[L03] 设置自定义请求头
来源：http://tvl.zycfv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pmw.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://oot.fehbvm.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://keu.yuanzhike.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uqv.zhengqikj.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hwt.cqqwz.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sva.quarkkingdee.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uyy.quarkkingdee.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vdp.chenlongwang.top

[L04] 设置超时
来源：http://srp.jlsjyb.cn

Py:   requests.get(url, timeout=5)
来源：http://rme.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hzq.ehwqpu.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hwp.xinyue.icu

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pzs.ywan-chungtsiang.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ylb.gaohongyu789.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fpc.ydzc1.top


<!-- 参考信息 -->