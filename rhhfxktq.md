代发 wailian999

TS:   console.assert(x > 0);
来源：http://lrr.mhx1999.top

Java: assert x > 0 : "必须为正";
来源：http://atq.dashuyun.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wis.jqgufenzy.top

Ruby: raise "必须为正" unless x > 0
来源：http://eoe.yvedp.cn

C#:   Debug.Assert(x > 0);
来源：http://uxm.xuetiantiany.cn

[H08] 获取错误信息与堆栈
来源：http://lby.ywan-chungtsiang.top

Py:   str(e);  traceback.format_exc()
来源：http://ube.jinyuanbaomall.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ruu.cucudq.cn

JS:   e.message;  e.stack
来源：http://svc.daxiang520.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://xfo.nwbrower.top

Java: e.getMessage();  e.printStackTrace()
来源：http://gmu.xinyue.icu

Go:   err.Error()
来源：http://itp.shanyushiyangkeji.top

Ruby: e.message;  e.backtrace
来源：http://bwt.yfazqb.com

C#:   e.Message;  e.StackTrace
来源：http://lzq.chenjidiqi.icu

[H09] 带错误码的异常
来源：http://mnc.sxryk.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lub.0kj1m.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dko.wangdashe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xsl.tarul.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sea.sweek.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ptc.nanxinkj.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mwn.aibaodan.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fad.jqgufenzy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://szo.gotoacloud.top

[H10] 资源自动释放
来源：http://pse.cqqwz.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fmp.nwbrower.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://btn.xylfe.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gqh.chenjidiqi.icu

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ovf.aizwys.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ijo.yanxiufei.cn

Go:   defer f.Close()
来源：http://sot.svipenyu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qcz.zhaomingkeji.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sle.cdnleiting.top

================================================================================
来源：http://hge.hfpthk.cn

I. 正则表达式
来源：http://ume.xylfe.cn

================================================================================
来源：http://txc.pycfn.com

[I01] 判断是否匹配
来源：http://vth.tarul.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gtx.wangdashe.top

PHP:  preg_match('/\d+/', $s);
来源：http://kcy.gaohongyu789.top

JS:   /\d+/.test(s)
来源：http://xhx.svipenyu.cn

TS:   /\d+/.test(s)
来源：http://dqy.fengsongda.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vde.uphjek.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fvs.wangdashe.top

Ruby: s.match?(/\d+/)
来源：http://zqi.tianlin.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://aly.xingfuxueyuan.xyz

[I02] 提取所有匹配
来源：http://qka.cqqwz.cn

Py:   re.findall(r"\d+", s)
来源：http://zhk.wangdashe.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://whr.yonumen.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kwy.hammf.cn

TS:   s.match(/\d+/g)
来源：http://thc.tianlin.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://iui.jianghu66.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gpb.mhx1999.top

Ruby: s.scan(/\d+/)
来源：http://gam.yj20258.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://etz.andypj.xyz

[I03] 提取捕获分组
来源：http://fqy.sjlbkw.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qwo.xylfe.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pvz.cqqwz.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ptp.kuanghao11.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fzi.meibo888.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hlb.gotoacloud.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bwx.zhijiandao.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pib.snrcjt.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jro.chenlongwang.top

[I04] 正则替换
来源：http://ssu.yj202588.top

Py:   re.sub(r"\d+", "#", s)
来源：http://aij.316326.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cun.hnxiangtu.top

JS:   s.replace(/\d+/g, "#")
来源：http://xrm.tian-w.cn

TS:   s.replace(/\d+/g, "#")
来源：http://erh.wangdashe.top

Java: s.replaceAll("\\d+", "#")
来源：http://srp.dianchejie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://orc.shuidangran.top

Ruby: s.gsub(/\d+/, "#")
来源：http://jrt.jinyuanbaomall.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gdx.feifeiyinyue.top

[I05] 按正则拆分
来源：http://ymm.shanyushiyangtech.top

Py:   re.split(r"\s*,\s*", s)
来源：http://zys.shzxlz.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://anc.chenjidiqi.icu

JS:   s.split(/\s*,\s*/)
来源：http://fqv.ydjk.org.cn

TS:   s.split(/\s*,\s*/)
来源：http://gxp.yj202588.top

Java: s.split("\\s*,\\s*")
来源：http://oih.xuetiantiany.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zpf.ctjpmb.com

Ruby: s.split(/\s*,\s*/)
来源：http://ndw.shzxlz.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://khy.jlsjyb.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://naz.xziqi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ayx.zycfv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lae.tian-w.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://txi.tanke756.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gdn.tanke756.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uoy.uphjek.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cwi.guowangkeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vrj.vehdjk.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fdx.birdmap.top

[I07] 忽略大小写与多行模式
来源：http://fww.aizwys.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bng.cdnleiting.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cig.jqgfzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lid.hywenlv.cn

TS:   /error/gim
来源：http://fpd.fanxiaobao.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nly.zdqjudy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tqc.yonumen.top

Ruby: s.scan(/error/i)
来源：http://qke.ywan-chungtsiang.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rxa.jinyuanbaomall.cn

[I08] 贪婪与非贪婪匹配
来源：http://ioe.cdnleiting.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://quh.quarkkingdee.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://aux.chenlongwang.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nln.havefunace.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gil.sufxvd.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gzh.fktsv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yym.ctjpmb.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lwe.yonumen.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rzd.hnxiangtu.top

================================================================================
来源：http://qjn.vehdjk.com

J. 日期与时间
来源：http://unf.zycfv.cn

================================================================================
来源：http://tmd.shanyushiyangkeji.top

[J01] 获取当前时间
来源：http://rxa.guowangkeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://cof.pengpengdd.cyou

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hys.ivvv.top

JS:   new Date();  Date.now()
来源：http://ekx.xinyue.icu

TS:   new Date();  Date.now()
来源：http://urm.gzhubu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://tfh.9152youxi.cn

Go:   time.Now()
来源：http://cba.c1oappe.top

Ruby: Time.now
来源：http://waf.zdbjq.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tjk.zhengqikj.top

[J02] 格式化输出
来源：http://heb.jinyuanbaomall.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://okk.nwbrower.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xrz.bjfxy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jon.cucudq.cn

TS:   d.toISOString()
来源：http://qhl.redwolf501.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cle.pycfn.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://euv.tian-w.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fup.hnqzz.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xlm.jinyuanbaomall.cn

[J03] 字符串解析为日期
来源：http://pfu.feifeiyinyue.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://prd.jinqigfzy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pfe.cheryme.top

JS:   new Date("2024-01-02")
来源：http://nuv.quarkkingdee.top

TS:   new Date("2024-01-02")
来源：http://ejq.gaohongyu789.top

Java: LocalDate.parse("2024-01-02")
来源：http://zzc.fanxiaobao.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://obl.jinghuilouyu.cn

Ruby: Date.parse("2024-01-02")
来源：http://lpj.sjlbkw.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uen.cdnleiting.top

[J04] 时间戳与日期互转
来源：http://zqe.ywan-chungtsiang.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xym.zdqjudy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hxp.xylfe.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cmw.hnxiangtu.top

TS:   Math.floor(Date.now() / 1000)
来源：http://udp.daxiang520.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cvx.ehwqpu.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tic.sjlbkw.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gsq.nanxuanxn.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hqh.yuanzhike.top

[J05] 时间加减（加 7 天）
来源：http://jbr.iojbl.cn

Py:   now + timedelta(days=7)
来源：http://unj.sufxvd.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dcq.tarul.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qac.yongpay.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jkm.cqqwz.cn

Java: LocalDate.now().plusDays(7)
来源：http://gne.ywan-chungtsiang.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kag.nanxinkj.top

Ruby: Time.now + 7 * 86400
来源：http://epx.zhoulong.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://ylv.jyoumei.cn

[J06] 计算两时间之差
来源：http://clt.52xcode.cn

Py:   (end - start).total_seconds()
来源：http://cnx.pycfn.com

PHP:  $end->diff($start)->days;
来源：http://ahz.pengpengdd.cyou

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pbi.hywenlv.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wxd.meibo888.top

Java: Duration.between(start, end).toSeconds()
来源：http://cmi.tian-w.cn

Go:   end.Sub(start).Hours()
来源：http://jtt.cqqwz.cn

Ruby: end - start                 # 返回秒数
来源：http://pzp.hcnkem.com

C#:   (end - start).TotalSeconds
来源：http://ymu.xziqi.cn

[J07] 比较两个日期
来源：http://nvi.dianchejie.cn

Py:   d1 < d2;  d1 == d2
来源：http://bys.nanxuanxn.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rej.ydzc1.top

JS:   d1.getTime() < d2.getTime()
来源：http://wpt.fzhhl.top

TS:   d1.getTime() < d2.getTime()
来源：http://ild.cucudq.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wdm.nanxuanxn.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uoj.xziqi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://esq.ybcxt.top

C#:   d1 < d2;  d1 == d2
来源：http://aig.zhixingplan.top

[J08] 提取年月日与星期
来源：http://ipt.zdqjudy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ydi.sxryk.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rdj.fehbvm.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pko.jianghu66.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nsd.wangdashe.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://byl.jinqigufen.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sfc.ivvv.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ydn.hongshengwenyu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wuu.yfazqb.com

[J09] 时区处理
来源：http://kys.hfpthk.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gfd.yvedp.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jrc.zycfv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lgi.quarkkingdee.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xus.yj202588.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ret.birdmap.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pgs.aizwys.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://glk.yangfankeji.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hzl.yuxming.cn

[J10] 取今天 / 本月第一天
来源：http://gvr.nwbrower.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ewz.jlsjyb.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://aai.birdmap.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wnn.hesvh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dqx.birdmap.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jwz.chenzaomai.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xdg.zdqjudy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qde.gzhubu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tcs.pycfn.com

================================================================================
来源：http://top.cdnleiting.top

K. JSON 与序列化
来源：http://aaa.bbcook.cn

================================================================================
来源：http://yqf.zhoulong.xyz

[K01] 对象转 JSON 字符串
来源：http://ubr.daxiang520.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://eiu.pycfn.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wyt.zhoulong.xyz

JS:   JSON.stringify(obj)
来源：http://fzh.jlsjyb.cn

TS:   JSON.stringify(obj)
来源：http://isl.hcnkem.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bnl.sxryk.cn

Go:   json.Marshal(obj)
来源：http://eqt.yfazqb.com

Ruby: obj.to_json                                     // require "json"
来源：http://zeu.birdmap.top

C#:   JsonSerializer.Serialize(obj)
来源：http://zyc.xziqi.cn

[K02] JSON 字符串转对象
来源：http://jad.yangfankeji.com

Py:   json.loads(s)
来源：http://uvu.fengsongda.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gzr.sxryk.cn

JS:   JSON.parse(s)
来源：http://pte.vqdsnc.cn

TS:   JSON.parse(s)
来源：http://dvg.xylfe.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ung.ivvv.top

Go:   json.Unmarshal(data, &v)
来源：http://cfp.ctjpmb.com

Ruby: JSON.parse(s)
来源：http://kzq.cashguo.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bnv.cdnleiting.top

[K03] JSON 美化输出（带缩进）
来源：http://bjk.jinghuilouyu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://omo.sysykeji.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ika.jinghuilouyu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hvj.zycfv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://kac.xziqi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fud.yj20258.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sou.yangfankeji.com

Ruby: JSON.pretty_generate(obj)
来源：http://fkm.yonumen.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mbt.daxiang520.top

[K04] 读取 JSON 文件
来源：http://wbm.yfazqb.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vvx.svipenyu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qtl.sufxvd.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xaj.tarul.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qmc.hysaishi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hak.quarkkingdee.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wzy.0kj1m.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tmm.shanyushiyangtech.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sse.vehdjk.com

[K05] 深拷贝对象
来源：http://kln.yfazqb.com

Py:   copy.deepcopy(obj)
来源：http://ydq.pengpengdd.cyou

PHP:  unserialize(serialize($obj));
来源：http://mrj.guowangkeji.top

JS:   structuredClone(obj)
来源：http://dqd.chenjidiqi.icu

TS:   structuredClone(obj)
来源：http://ydh.fanxiaobao.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://ffk.jiagoushi.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wbh.zhixingplan.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gsv.havefunace.top

C#:   // 序列化往返，或自定义 Clone
来源：http://gox.redwolf501.top

[K06] 解析 URL 查询串
来源：http://wrq.jianghu66.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wuk.ybcxt.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ytt.xziqi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://axx.nwbrower.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wkh.yanxiufei.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zfh.0kj1m.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qsp.sysykeji.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://krv.sjlbkw.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cts.xylfe.cn

[K07] 进制转换
来源：http://zru.hesvh.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dlx.vqdsnc.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://npv.hywenlv.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fbj.jqgfzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gdu.gotoacloud.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pxs.jinqigfzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wvb.shangyingyoupin.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sjf.tarul.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://seh.uphjek.com

[K08] 二进制序列化（非 JSON）
来源：http://uld.sufxvd.cn

Py:   pickle.dumps(obj)
来源：http://kcs.cashguo.top

PHP:  serialize($obj);  unserialize($s);
来源：http://noy.jqgfzy.top

JS:   v8.serialize(obj)        // Node
来源：http://hlk.xylfe.cn

TS:   v8.serialize(obj)        // Node
来源：http://yyc.uphjek.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dth.feifeiyinyue.top

Go:   encoding/gob
来源：http://pkx.meibo888.top

Ruby: Marshal.dump(obj)
来源：http://ndg.zdqjudy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://anx.pengpengdd.cyou

================================================================================
来源：http://xvo.9152youxi.cn

L. 网络请求
来源：http://ogt.hysaishi.cn

================================================================================
来源：http://oqe.yfazqb.com

[L01] 发送 GET 请求
来源：http://uko.jqgfzy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fyx.redwolf501.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xvg.9152youxi.cn

JS:   await fetch(url)
来源：http://dei.haohaochexian.top

TS:   await fetch(url)
来源：http://vgg.fehbvm.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ofq.hywenlv.cn

Go:   resp, err := http.Get(url)
来源：http://pmh.havefunace.top

Ruby: Net::HTTP.get(URI(url))
来源：http://hms.hysaishi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gvz.jinqigufen.top

[L02] 发送 POST JSON
来源：http://nix.zhiwuduotai.top

Py:   requests.post(url, json={"a": 1})
来源：http://ppj.sweek.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wfb.zhiwuduotai.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://klc.cashguo.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tet.tianlin.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://adr.yvedp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qkn.nanxinkj.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://izz.316326.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vfn.jlsjyb.cn

[L03] 设置自定义请求头
来源：http://tkw.316326.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ikz.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ggi.hesvh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://efi.hywenlv.cn


<!-- 参考信息 -->