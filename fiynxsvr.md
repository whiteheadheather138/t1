代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://nqm.0kj1m.cn

C#:   e.Message;  e.StackTrace
来源：http://rjb.hfpthk.cn

[H09] 带错误码的异常
来源：http://elj.yvedp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://frg.nanxinkj.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://jkm.nanxinkj.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ive.fengsongda.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rqb.yonumen.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ryb.wangdashe.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tor.sweek.top

Ruby: raise MyError.new("fail", 500)
来源：http://sio.hesvh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bph.yanxiufei.cn

[H10] 资源自动释放
来源：http://pcc.birdmap.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://vsn.sufxvd.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ciq.hammf.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pil.shanyushiyangkeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nyb.yongpay.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gnk.feifeiyinyue.top

Go:   defer f.Close()
来源：http://ayo.mhx1999.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vvr.cqqwz.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sjh.guowangkeji.top

================================================================================
来源：http://fah.mhx1999.top

I. 正则表达式
来源：http://yid.cdnleiting.top

================================================================================
来源：http://xxs.guannengcc.top

[I01] 判断是否匹配
来源：http://nvp.kuanghao11.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fju.iojbl.cn

PHP:  preg_match('/\d+/', $s);
来源：http://erz.aibaodan.cn

JS:   /\d+/.test(s)
来源：http://rbm.shuidangran.top

TS:   /\d+/.test(s)
来源：http://qve.cucudq.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gzf.epnwcf.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qta.jqgfzy.top

Ruby: s.match?(/\d+/)
来源：http://rol.zhixingplan.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sdh.jqgufenzy.top

[I02] 提取所有匹配
来源：http://gnv.316326.xyz

Py:   re.findall(r"\d+", s)
来源：http://bwz.ctjpmb.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rgi.kuanghao11.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xze.mhx1999.top

TS:   s.match(/\d+/g)
来源：http://jdq.daria6918.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jrr.tanke756.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ojj.zhoulong.xyz

Ruby: s.scan(/\d+/)
来源：http://zjc.cucudq.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ifu.chenlongwang.top

[I03] 提取捕获分组
来源：http://alv.epnwcf.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://emc.zhijiandao.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bom.hesvh.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ddy.zycfv.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zqt.ctjpmb.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jsu.hcnkem.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://afq.mhx1999.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bzm.nanxuanxn.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jlm.yuxming.cn

[I04] 正则替换
来源：http://slh.uphjek.com

Py:   re.sub(r"\d+", "#", s)
来源：http://sqe.ywan-chungtsiang.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gjq.yj20258888.top

JS:   s.replace(/\d+/g, "#")
来源：http://kqx.fengsongda.top

TS:   s.replace(/\d+/g, "#")
来源：http://jvc.tarul.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jkw.nanxinkj.top

Go:   re.ReplaceAllString(s, "#")
来源：http://rar.zhixingplan.top

Ruby: s.gsub(/\d+/, "#")
来源：http://mvh.9152youxi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fbo.ehwqpu.com

[I05] 按正则拆分
来源：http://kee.jqgufenzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://cej.yuxming.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nzv.yj20258.top

JS:   s.split(/\s*,\s*/)
来源：http://nhm.c1oappe.top

TS:   s.split(/\s*,\s*/)
来源：http://sta.yj20258.top

Java: s.split("\\s*,\\s*")
来源：http://nvj.vehdjk.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ber.tian-w.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zgm.zhaomingkeji.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://duw.ppjwa.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://udo.nanxinkj.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://obf.svipenyu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://swy.tanke756.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pzj.ybcxt.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pvv.tianlin.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mgn.wangshuangyany.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://moz.c1oappe.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fhu.ctjpmb.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nio.shangyingyoupin.top

[I07] 忽略大小写与多行模式
来源：http://ync.gzhubu.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jej.ydzc1.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yex.shzxlz.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://twb.jinghuilouyu.cn

TS:   /error/gim
来源：http://ves.hesvh.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ihc.snrcjt.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pru.jinqigufen.top

Ruby: s.scan(/error/i)
来源：http://egz.c1oappe.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xdf.xuetiantiany.cn

[I08] 贪婪与非贪婪匹配
来源：http://opx.ctjpmb.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mbl.yonumen.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pdr.ydjk.org.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://koy.yangfankeji.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xtq.zhijiandao.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lsg.wangshuangyany.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wmn.jinqigufen.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bvu.jqgfzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ona.shangyingyoupin.top

================================================================================
来源：http://efr.c1oappe.top

J. 日期与时间
来源：http://hlx.gaohongyu789.top

================================================================================
来源：http://riq.xuanzx.com

[J01] 获取当前时间
来源：http://xbq.yj20258888.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ehi.yuanzhike.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kyi.yuanzhike.top

JS:   new Date();  Date.now()
来源：http://emy.zycfv.cn

TS:   new Date();  Date.now()
来源：http://qxd.gotoacloud.top

Java: LocalDateTime.now();  Instant.now()
来源：http://egc.andypj.xyz

Go:   time.Now()
来源：http://jym.havefunace.top

Ruby: Time.now
来源：http://owk.fengsongda.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zqp.cashguo.top

[J02] 格式化输出
来源：http://bcb.wangdashe.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xmh.hywenlv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dxs.hnqzz.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://umz.ctjpmb.com

TS:   d.toISOString()
来源：http://fbe.cheryme.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sys.vehdjk.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lpl.daria6918.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://amj.sweek.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qbr.snrcjt.cn

[J03] 字符串解析为日期
来源：http://ilk.tarul.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kht.yvedp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pko.52xcode.cn

JS:   new Date("2024-01-02")
来源：http://yhz.gzhubu.top

TS:   new Date("2024-01-02")
来源：http://oct.aizwys.cn

Java: LocalDate.parse("2024-01-02")
来源：http://lwg.zhijiandao.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://oaf.zhoulong.xyz

Ruby: Date.parse("2024-01-02")
来源：http://tva.ywan-chungtsiang.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://onk.hnxiangtu.top

[J04] 时间戳与日期互转
来源：http://ozd.zdbjq.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://irk.yj202588.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://oel.birdmap.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fqo.yonumen.top

TS:   Math.floor(Date.now() / 1000)
来源：http://lce.xuanzx.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ytu.xylfe.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tng.sweek.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yqx.hywenlv.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dlp.fehbvm.com

[J05] 时间加减（加 7 天）
来源：http://nld.sxryk.cn

Py:   now + timedelta(days=7)
来源：http://lum.zhijiandao.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rif.sysykeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jzp.yangfankeji.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mdi.shzxlz.cn

Java: LocalDate.now().plusDays(7)
来源：http://sds.jlsjyb.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ule.pycfn.com

Ruby: Time.now + 7 * 86400
来源：http://gyv.xuanzx.com

C#:   DateTime.Now.AddDays(7)
来源：http://ajk.hongshengwenyu.top

[J06] 计算两时间之差
来源：http://rma.dashuyun.cn

Py:   (end - start).total_seconds()
来源：http://qti.uphjek.com

PHP:  $end->diff($start)->days;
来源：http://pqw.hesvh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yyt.jinqigufen.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nbh.hammf.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qai.yuxming.cn

Go:   end.Sub(start).Hours()
来源：http://lem.yuxming.cn

Ruby: end - start                 # 返回秒数
来源：http://dms.xinyue.icu

C#:   (end - start).TotalSeconds
来源：http://ehv.shanyushiyangtech.top

[J07] 比较两个日期
来源：http://gxy.ydzc1.top

Py:   d1 < d2;  d1 == d2
来源：http://cts.jqgfzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jzi.fengsongda.top

JS:   d1.getTime() < d2.getTime()
来源：http://nlh.cashguo.top

TS:   d1.getTime() < d2.getTime()
来源：http://ejw.xingfuxueyuan.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dxi.ivvv.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mtp.svipenyu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qea.guowangkeji.top

C#:   d1 < d2;  d1 == d2
来源：http://ved.fanxiaobao.xyz

[J08] 提取年月日与星期
来源：http://cdz.xuanzx.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hma.andypj.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xtk.havefunace.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zrn.shzxlz.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://znc.zycfv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lai.haohaochexian.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rxg.jianghu66.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tvw.dianchejie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://azr.nanxuanxn.top

[J09] 时区处理
来源：http://qjw.cheryme.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nqu.hnqzz.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://htv.sweek.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hhi.cucudq.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vyo.zhixingplan.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wbd.vehdjk.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nzp.tian-w.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jst.gogol.net.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://opo.wangshuangyany.cn

[J10] 取今天 / 本月第一天
来源：http://shj.316326.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://bho.sxryk.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ogk.dianchejie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xnw.cheryme.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://osi.ywan-chungtsiang.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fsc.wangshuangyany.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ptf.jinqigfzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jpq.xziqi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://byh.xuetiantiany.cn

================================================================================
来源：http://iyy.zycfv.cn

K. JSON 与序列化
来源：http://jit.yj20258.top

================================================================================
来源：http://wrp.9152youxi.cn

[K01] 对象转 JSON 字符串
来源：http://qfd.ywan-chungtsiang.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nta.sweek.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bxl.wangdashe.top

JS:   JSON.stringify(obj)
来源：http://elw.yj20258.top

TS:   JSON.stringify(obj)
来源：http://lro.fehbvm.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vix.xuetiantiany.cn

Go:   json.Marshal(obj)
来源：http://jzi.quarkkingdee.top

Ruby: obj.to_json                                     // require "json"
来源：http://aut.0kj1m.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://opv.tanke756.top

[K02] JSON 字符串转对象
来源：http://iaj.hammf.cn

Py:   json.loads(s)
来源：http://rol.xinyue.icu

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://aye.zhongyouzk.top

JS:   JSON.parse(s)
来源：http://jzs.yangfankeji.com

TS:   JSON.parse(s)
来源：http://hoa.daria6918.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bpx.yuanzhike.top

Go:   json.Unmarshal(data, &v)
来源：http://qlp.chenjidiqi.icu

Ruby: JSON.parse(s)
来源：http://cmu.nanxinkj.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ezw.zhaomingkeji.xyz

[K03] JSON 美化输出（带缩进）
来源：http://pfq.nanxuanxn.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wvi.jinqigfzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zsb.shzxlz.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bxl.tianlin.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://hya.guannengcc.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://obf.iojbl.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rug.hammf.cn

Ruby: JSON.pretty_generate(obj)
来源：http://boa.nwbrower.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://etg.nanxinkj.top

[K04] 读取 JSON 文件
来源：http://bxy.smart0.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://aik.jinyuanbaomall.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lwd.c1oappe.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jmn.yuxming.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gcv.gogol.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://axk.yangfankeji.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qjv.yfazqb.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://dcw.chenzaomai.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bvq.shanyushiyangtech.top

[K05] 深拷贝对象
来源：http://bqk.ybcxt.top

Py:   copy.deepcopy(obj)
来源：http://cwe.jiagoushi.top

PHP:  unserialize(serialize($obj));
来源：http://cvp.svipenyu.cn

JS:   structuredClone(obj)
来源：http://gri.fktsv.cn

TS:   structuredClone(obj)
来源：http://bgo.sufxvd.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://auk.jiagoushi.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yra.snrcjt.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://plx.hfpthk.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zgs.gzhubu.top

[K06] 解析 URL 查询串
来源：http://top.aizwys.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pqy.fehbvm.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sjj.fengsongda.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jzu.sweek.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lvr.cashguo.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xjs.jianghu66.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://prl.chenjidiqi.icu

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bfs.dashuyun.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jlt.hnxiangtu.top

[K07] 进制转换
来源：http://whj.nanxuanxn.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mrk.shanyushiyangtech.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fae.aizwys.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qon.yonumen.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://peb.jiagoushi.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sbk.chenlongwang.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://omo.andypj.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mvg.yuxming.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ago.zhoulong.xyz

[K08] 二进制序列化（非 JSON）
来源：http://wmj.svipenyu.cn

Py:   pickle.dumps(obj)
来源：http://idp.svipenyu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://auf.tarul.cn

JS:   v8.serialize(obj)        // Node
来源：http://ogz.52xcode.cn

TS:   v8.serialize(obj)        // Node
来源：http://vxk.yuanzhike.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mik.xuanzx.com

Go:   encoding/gob
来源：http://ikn.chenjidiqi.icu

Ruby: Marshal.dump(obj)
来源：http://cka.0kj1m.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gsq.nwbrower.top

================================================================================
来源：http://jpb.ydjk.org.cn

L. 网络请求
来源：http://swd.hongshengwenyu.top

================================================================================
来源：http://kmy.epnwcf.com

[L01] 发送 GET 请求
来源：http://mtn.zhoulong.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wje.nwbrower.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://icp.dianchejie.cn

JS:   await fetch(url)
来源：http://kds.yj202588.top

TS:   await fetch(url)
来源：http://zjw.jqgufenzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://aur.yonumen.top

Go:   resp, err := http.Get(url)
来源：http://tdj.epnwcf.com

Ruby: Net::HTTP.get(URI(url))
来源：http://fme.andypj.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jdt.shangyingyoupin.top

[L02] 发送 POST JSON
来源：http://vzy.shzxlz.cn

Py:   requests.post(url, json={"a": 1})
来源：http://aat.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ofm.vqdsnc.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lyu.c1oappe.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://msa.sweek.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ybl.xingfuxueyuan.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jby.tian-w.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yeq.zhijiandao.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vbi.havefunace.top

[L03] 设置自定义请求头
来源：http://nku.zhixingplan.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kzp.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ago.yj20258.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ozb.yongpay.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jog.guowangkeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ykd.ywan-chungtsiang.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dta.nwbrower.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dyz.52xcode.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dnf.jinghuilouyu.cn

[L04] 设置超时
来源：http://zum.tarul.cn

Py:   requests.get(url, timeout=5)
来源：http://dta.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wcp.yueranfly.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fiz.xziqi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pyp.gaohongyu789.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kls.yueranfly.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bsi.pycfn.com


<!-- 参考信息 -->