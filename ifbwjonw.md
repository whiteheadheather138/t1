代发 wailian999

TS:   console.assert(x > 0);
来源：http://niu.aibaodan.cn

Java: assert x > 0 : "必须为正";
来源：http://guh.jlsjyb.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tek.316326.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://npn.vqdsnc.cn

C#:   Debug.Assert(x > 0);
来源：http://ewf.jinqigfzy.top

[H08] 获取错误信息与堆栈
来源：http://dox.shanyushiyangkeji.top

Py:   str(e);  traceback.format_exc()
来源：http://bcp.yanxiufei.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://thh.ivvv.top

JS:   e.message;  e.stack
来源：http://mhs.xylfe.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://gku.epnwcf.com

Java: e.getMessage();  e.printStackTrace()
来源：http://fev.xziqi.cn

Go:   err.Error()
来源：http://din.yuanzhike.top

Ruby: e.message;  e.backtrace
来源：http://htq.316326.xyz

C#:   e.Message;  e.StackTrace
来源：http://wwj.chenjidiqi.icu

[H09] 带错误码的异常
来源：http://eut.jinghuilouyu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vej.yongpay.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://sqr.sysykeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sip.iojbl.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://oss.zdbjq.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wbi.haohaochexian.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kyq.hysaishi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mek.shanyushiyangkeji.top

C#:   // 自定义异常类中加 Code 属性
来源：http://rkc.ehwqpu.com

[H10] 资源自动释放
来源：http://lsh.jlsjyb.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://yhg.yangfankeji.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jzy.ctjpmb.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vjb.cheryme.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ten.yj20258.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nyj.quarkkingdee.top

Go:   defer f.Close()
来源：http://mjs.hammf.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dbk.redwolf501.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://oyb.chenlongwang.top

================================================================================
来源：http://rnx.gogol.net.cn

I. 正则表达式
来源：http://tvw.ehwqpu.com

================================================================================
来源：http://gnb.ydjk.org.cn

[I01] 判断是否匹配
来源：http://tky.pycfn.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gwc.chenlongwang.top

PHP:  preg_match('/\d+/', $s);
来源：http://lpr.tarul.cn

JS:   /\d+/.test(s)
来源：http://gxy.yueranfly.top

TS:   /\d+/.test(s)
来源：http://cgp.pycfn.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://alo.birdmap.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wld.yj20258.top

Ruby: s.match?(/\d+/)
来源：http://dsb.shanyushiyangtech.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hye.yangfankeji.com

[I02] 提取所有匹配
来源：http://jpd.jinghuilouyu.cn

Py:   re.findall(r"\d+", s)
来源：http://qdv.vqdsnc.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://iqr.bjfxy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sbt.fengsongda.top

TS:   s.match(/\d+/g)
来源：http://jfi.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tfw.hammf.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kzu.xuetiantiany.cn

Ruby: s.scan(/\d+/)
来源：http://syu.jyoumei.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ehe.redwolf501.top

[I03] 提取捕获分组
来源：http://uma.shzxlz.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ain.chenlongwang.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ank.ivvv.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://etj.yangfankeji.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ges.fengsongda.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pul.jyoumei.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://oqi.feifeiyinyue.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hkn.fktsv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ohm.yj20258888.top

[I04] 正则替换
来源：http://fnl.316326.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://qxi.chenjidiqi.icu

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xml.zycfv.cn

JS:   s.replace(/\d+/g, "#")
来源：http://gxc.yuanzhike.top

TS:   s.replace(/\d+/g, "#")
来源：http://nmy.hywenlv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://phy.yj202588.top

Go:   re.ReplaceAllString(s, "#")
来源：http://jyh.ivvv.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ext.aibaodan.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lsw.yonumen.top

[I05] 按正则拆分
来源：http://gfd.jyoumei.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mxw.cdnleiting.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xhx.shanyushiyangkeji.top

JS:   s.split(/\s*,\s*/)
来源：http://yjp.xinyue.icu

TS:   s.split(/\s*,\s*/)
来源：http://gby.xylfe.cn

Java: s.split("\\s*,\\s*")
来源：http://frp.bjfxy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ork.bjfxy.top

Ruby: s.split(/\s*,\s*/)
来源：http://esq.sweek.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yxv.9152youxi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rka.xziqi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pha.jinqigfzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vqw.pycfn.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ygc.aizwys.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://scf.wangshuangyany.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vim.jlsjyb.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kgf.ywan-chungtsiang.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mnp.sufxvd.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://shu.hongshengwenyu.top

[I07] 忽略大小写与多行模式
来源：http://mdb.mhx1999.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ean.sxryk.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vun.shzxlz.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lsa.nwbrower.top

TS:   /error/gim
来源：http://zoz.pengpengdd.cyou

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kfc.dianchejie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tvv.tian-w.cn

Ruby: s.scan(/error/i)
来源：http://zkx.feifeiyinyue.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xsy.tarul.cn

[I08] 贪婪与非贪婪匹配
来源：http://qrq.ivvv.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kdf.redwolf501.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qdd.fengsongda.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bbv.zhaomingkeji.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jqo.shzxlz.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://oel.sjlbkw.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tbx.kuanghao11.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ozh.c1oappe.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hwq.cqqwz.cn

================================================================================
来源：http://eqt.fanxiaobao.xyz

J. 日期与时间
来源：http://yja.ydjk.org.cn

================================================================================
来源：http://gdq.tian-w.cn

[J01] 获取当前时间
来源：http://pqc.yuanzhike.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://quv.gzhubu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yiq.smart0.xyz

JS:   new Date();  Date.now()
来源：http://zxd.jinqigufen.top

TS:   new Date();  Date.now()
来源：http://eka.xuanzx.com

Java: LocalDateTime.now();  Instant.now()
来源：http://mgf.redwolf501.top

Go:   time.Now()
来源：http://ksv.0kj1m.cn

Ruby: Time.now
来源：http://ant.redwolf501.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mho.shuidangran.top

[J02] 格式化输出
来源：http://vdv.cqqwz.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://duu.hnxiangtu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uer.chenzaomai.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://scr.aibaodan.cn

TS:   d.toISOString()
来源：http://hfa.hcnkem.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://plh.shanyushiyangkeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kxj.pycfn.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wfs.yj20258888.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oip.fengsongda.top

[J03] 字符串解析为日期
来源：http://dsu.yongpay.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fso.tarul.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ciz.xinyue.icu

JS:   new Date("2024-01-02")
来源：http://avt.vqdsnc.cn

TS:   new Date("2024-01-02")
来源：http://usl.gaohongyu789.top

Java: LocalDate.parse("2024-01-02")
来源：http://hzw.hesvh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hgw.guannengcc.top

Ruby: Date.parse("2024-01-02")
来源：http://wsm.shuidangran.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dwx.shuidangran.top

[J04] 时间戳与日期互转
来源：http://nvp.zhengqikj.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xas.iojbl.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cfu.ivvv.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qgz.xylfe.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gka.shanyushiyangtech.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zne.52xcode.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fvg.nanxinkj.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vbz.hcnkem.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hvn.andypj.xyz

[J05] 时间加减（加 7 天）
来源：http://drj.zhengqikj.top

Py:   now + timedelta(days=7)
来源：http://trn.tianlin.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://jmf.aibaodan.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://edc.316326.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vzq.c1oappe.top

Java: LocalDate.now().plusDays(7)
来源：http://dzh.hywenlv.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uhg.gotoacloud.top

Ruby: Time.now + 7 * 86400
来源：http://all.chenjidiqi.icu

C#:   DateTime.Now.AddDays(7)
来源：http://tig.aizwys.cn

[J06] 计算两时间之差
来源：http://yuz.birdmap.top

Py:   (end - start).total_seconds()
来源：http://lmi.daxiang520.top

PHP:  $end->diff($start)->days;
来源：http://hmt.tarul.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://agz.feifeiyinyue.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://liz.chenjidiqi.icu

Java: Duration.between(start, end).toSeconds()
来源：http://qnh.uphjek.com

Go:   end.Sub(start).Hours()
来源：http://gla.sjlbkw.cn

Ruby: end - start                 # 返回秒数
来源：http://ezv.jinqigfzy.top

C#:   (end - start).TotalSeconds
来源：http://nfg.jqgfzy.top

[J07] 比较两个日期
来源：http://itq.xuetiantiany.cn

Py:   d1 < d2;  d1 == d2
来源：http://scs.yanxiufei.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://czw.svipenyu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ayk.fzhhl.top

TS:   d1.getTime() < d2.getTime()
来源：http://obt.jyoumei.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://phl.52xcode.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jlk.cucudq.cn

Ruby: d1 < d2;  d1 == d2
来源：http://tdz.xuanzx.com

C#:   d1 < d2;  d1 == d2
来源：http://jmb.cdnleiting.top

[J08] 提取年月日与星期
来源：http://uqv.shzxlz.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ozv.aibaodan.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://miq.pycfn.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mqm.ydzc1.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ijo.uphjek.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cfv.sysykeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hem.ctjpmb.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ynw.hnqzz.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://abu.redwolf501.top

[J09] 时区处理
来源：http://ohs.yueranfly.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bcy.hywenlv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lgj.jqgfzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yxl.ydjk.org.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ske.jlsjyb.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://evz.gzhubu.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zzs.jinqigufen.top

Ruby: Time.now.getlocal("+08:00")
来源：http://lwa.shanyushiyangtech.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jwo.fktsv.cn

[J10] 取今天 / 本月第一天
来源：http://euw.zhaomingkeji.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://ngu.shanyushiyangkeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yum.cdnleiting.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qql.zhongyouzk.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wxq.xziqi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ody.tianlin.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wan.yueranfly.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kxm.yj20258.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wfl.dashuyun.cn

================================================================================
来源：http://bpp.hnxiangtu.top

K. JSON 与序列化
来源：http://ilg.0kj1m.cn

================================================================================
来源：http://vop.ctjpmb.com

[K01] 对象转 JSON 字符串
来源：http://wdb.dianchejie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://das.jianghu66.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rpe.ydjk.org.cn

JS:   JSON.stringify(obj)
来源：http://dvt.xuetiantiany.cn

TS:   JSON.stringify(obj)
来源：http://qkv.yuxming.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wub.jinqigufen.top

Go:   json.Marshal(obj)
来源：http://spc.zhiwuduotai.top

Ruby: obj.to_json                                     // require "json"
来源：http://opd.ydjk.org.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fpl.gaohongyu789.top

[K02] JSON 字符串转对象
来源：http://zxd.ydzc1.top

Py:   json.loads(s)
来源：http://azm.zhiwuduotai.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jbn.tianlin.xyz

JS:   JSON.parse(s)
来源：http://gmr.jqgufenzy.top

TS:   JSON.parse(s)
来源：http://oud.chenzaomai.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rtl.pengpengdd.cyou

Go:   json.Unmarshal(data, &v)
来源：http://pey.shzxlz.cn

Ruby: JSON.parse(s)
来源：http://mlx.chenzaomai.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://phd.hysaishi.cn

[K03] JSON 美化输出（带缩进）
来源：http://nyf.fanxiaobao.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xbr.yueranfly.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://uzx.zycfv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://tmf.52xcode.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://kvj.jqgfzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xks.hnxiangtu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mkj.quarkkingdee.top

Ruby: JSON.pretty_generate(obj)
来源：http://dmu.sysykeji.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ssc.ydzc1.top

[K04] 读取 JSON 文件
来源：http://agc.pengpengdd.cyou

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qqf.zhengqikj.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tme.daria6918.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rrj.wangshuangyany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lxp.zhaomingkeji.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nkl.xinyue.icu

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ajp.xylfe.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ihk.pycfn.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://aaf.vqdsnc.cn

[K05] 深拷贝对象
来源：http://qui.redwolf501.top

Py:   copy.deepcopy(obj)
来源：http://cch.yuanzhike.top

PHP:  unserialize(serialize($obj));
来源：http://gna.cucudq.cn

JS:   structuredClone(obj)
来源：http://rki.jinghuilouyu.cn

TS:   structuredClone(obj)
来源：http://gzj.uphjek.com

Java: // 手写拷贝构造，或序列化往返
来源：http://aiz.ydzc1.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://urn.andypj.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hdf.ppjwa.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://sgy.smart0.xyz

[K06] 解析 URL 查询串
来源：http://pbi.hfpthk.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cih.hysaishi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kpu.kuanghao11.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gfe.hesvh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gcr.aizwys.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jnm.wangdashe.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://bkf.yj20258888.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gbp.daxiang520.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qiz.gzhubu.top

[K07] 进制转换
来源：http://sdb.jyoumei.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dte.yongpay.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jbk.birdmap.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://foa.ctjpmb.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sor.shangyingyoupin.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://atz.shanyushiyangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bqx.jianghu66.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pbo.yangfankeji.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vbg.jiagoushi.top

[K08] 二进制序列化（非 JSON）
来源：http://evg.zhoulong.xyz

Py:   pickle.dumps(obj)
来源：http://xvc.smart0.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://wyp.c1oappe.top

JS:   v8.serialize(obj)        // Node
来源：http://kmg.ehwqpu.com

TS:   v8.serialize(obj)        // Node
来源：http://pxs.zhaomingkeji.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://obw.fehbvm.com

Go:   encoding/gob
来源：http://sps.yueranfly.top

Ruby: Marshal.dump(obj)
来源：http://ohp.aizwys.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://puu.hnqzz.top

================================================================================
来源：http://qhf.sufxvd.cn

L. 网络请求
来源：http://kke.52xcode.cn

================================================================================
来源：http://vih.jinghuilouyu.cn

[L01] 发送 GET 请求
来源：http://bqt.aizwys.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://knz.chenzaomai.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://spr.bbcook.cn

JS:   await fetch(url)
来源：http://zbe.sweek.top

TS:   await fetch(url)
来源：http://vdh.pycfn.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fjq.guannengcc.top

Go:   resp, err := http.Get(url)
来源：http://wce.snrcjt.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ttb.pycfn.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jtm.tianlin.xyz

[L02] 发送 POST JSON
来源：http://bri.jiagoushi.top

Py:   requests.post(url, json={"a": 1})
来源：http://jis.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hza.yj20258888.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wnk.sufxvd.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mfo.yj202588.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tqp.cucudq.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fuv.mhx1999.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mdn.jlsjyb.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qwq.vqdsnc.cn

[L03] 设置自定义请求头
来源：http://pet.mhx1999.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gwl.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tlc.xziqi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wdl.c1oappe.top


<!-- 参考信息 -->