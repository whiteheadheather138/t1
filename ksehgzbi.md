代发 wailian999

[H07] 断言
来源：http://ito.hywenlv.cn

Py:   assert x > 0, "必须为正"
来源：http://jpd.wangshuangyany.cn

PHP:  assert($x > 0);
来源：http://zdr.0kj1m.cn

JS:   console.assert(x > 0);
来源：http://iyq.fengsongda.top

TS:   console.assert(x > 0);
来源：http://edq.ydjk.org.cn

Java: assert x > 0 : "必须为正";
来源：http://tzz.redwolf501.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dev.yonumen.top

Ruby: raise "必须为正" unless x > 0
来源：http://jat.fehbvm.com

C#:   Debug.Assert(x > 0);
来源：http://tfd.mhx1999.top

[H08] 获取错误信息与堆栈
来源：http://yhe.xylfe.cn

Py:   str(e);  traceback.format_exc()
来源：http://czf.yueranfly.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uoa.aibaodan.cn

JS:   e.message;  e.stack
来源：http://nxg.c1oappe.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://pom.nwbrower.top

Java: e.getMessage();  e.printStackTrace()
来源：http://hlo.xziqi.cn

Go:   err.Error()
来源：http://rvf.chenzaomai.com

Ruby: e.message;  e.backtrace
来源：http://cvc.jinqigufen.top

C#:   e.Message;  e.StackTrace
来源：http://ylu.nanxinkj.top

[H09] 带错误码的异常
来源：http://kzu.sysykeji.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://esj.hesvh.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xzb.xylfe.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qnk.hesvh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yan.sweek.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ukf.zhoulong.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kfc.xuanzx.com

Ruby: raise MyError.new("fail", 500)
来源：http://kuf.svipenyu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vvv.52xcode.cn

[H10] 资源自动释放
来源：http://tfo.sysykeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://smt.nwbrower.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cob.yvedp.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hav.ydjk.org.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://usf.fktsv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hjv.bbcook.cn

Go:   defer f.Close()
来源：http://auu.tarul.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vrd.c1oappe.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zrx.9152youxi.cn

================================================================================
来源：http://tyq.yongpay.top

I. 正则表达式
来源：http://bhm.kuanghao11.cn

================================================================================
来源：http://pnw.vehdjk.com

[I01] 判断是否匹配
来源：http://oxm.tianlin.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yct.iojbl.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gmw.guannengcc.top

JS:   /\d+/.test(s)
来源：http://vos.52xcode.cn

TS:   /\d+/.test(s)
来源：http://vjn.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fzg.havefunace.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cie.svipenyu.cn

Ruby: s.match?(/\d+/)
来源：http://wko.zhoulong.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ksc.xinyue.icu

[I02] 提取所有匹配
来源：http://nnd.yj202588.top

Py:   re.findall(r"\d+", s)
来源：http://afg.nwbrower.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://htm.ehwqpu.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bzw.yanxiufei.cn

TS:   s.match(/\d+/g)
来源：http://enp.yongpay.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nnl.shanyushiyangtech.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://afz.nanxuanxn.top

Ruby: s.scan(/\d+/)
来源：http://whu.haohaochexian.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://psw.smart0.xyz

[I03] 提取捕获分组
来源：http://bgd.ybcxt.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fuu.vehdjk.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zkt.dianchejie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yef.zdqjudy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://veh.haohaochexian.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://poy.haohaochexian.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gqc.zhongyouzk.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yjf.sufxvd.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baa.sufxvd.cn

[I04] 正则替换
来源：http://bwj.smart0.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://mgb.iojbl.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ghy.zdbjq.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pal.chenzaomai.com

TS:   s.replace(/\d+/g, "#")
来源：http://klt.redwolf501.top

Java: s.replaceAll("\\d+", "#")
来源：http://xgs.yj202588.top

Go:   re.ReplaceAllString(s, "#")
来源：http://jqz.ybcxt.top

Ruby: s.gsub(/\d+/, "#")
来源：http://obs.yj20258.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://eux.chenjidiqi.icu

[I05] 按正则拆分
来源：http://kue.daxiang520.top

Py:   re.split(r"\s*,\s*", s)
来源：http://car.shuidangran.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rce.yanxiufei.cn

JS:   s.split(/\s*,\s*/)
来源：http://ump.bjfxy.top

TS:   s.split(/\s*,\s*/)
来源：http://oio.chenjidiqi.icu

Java: s.split("\\s*,\\s*")
来源：http://yrc.svipenyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://oxd.kuanghao11.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pkl.fengsongda.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hzu.quarkkingdee.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zbt.feifeiyinyue.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://iuc.ybcxt.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lsa.haohaochexian.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zkb.redwolf501.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eax.mhx1999.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tri.yangfankeji.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dnc.mhx1999.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://niu.pengpengdd.cyou

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dfi.yj202588.top

[I07] 忽略大小写与多行模式
来源：http://rtr.tanke756.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kuy.redwolf501.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xtz.snrcjt.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://eam.zhongyouzk.top

TS:   /error/gim
来源：http://pwh.0kj1m.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wbz.yueranfly.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hso.hysaishi.cn

Ruby: s.scan(/error/i)
来源：http://gjl.tianlin.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://aom.zhixingplan.top

[I08] 贪婪与非贪婪匹配
来源：http://iek.vqdsnc.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://khr.yanxiufei.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://syg.wangdashe.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ocd.mhx1999.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://frq.c1oappe.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://yyo.ydjk.org.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xhu.havefunace.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dsg.hammf.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rfz.yongpay.top

================================================================================
来源：http://eyf.0kj1m.cn

J. 日期与时间
来源：http://jjk.shuidangran.top

================================================================================
来源：http://pqt.vqdsnc.cn

[J01] 获取当前时间
来源：http://xzh.bbcook.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wwx.epnwcf.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zlq.sjlbkw.cn

JS:   new Date();  Date.now()
来源：http://otf.hongshengwenyu.top

TS:   new Date();  Date.now()
来源：http://ilq.guowangkeji.top

Java: LocalDateTime.now();  Instant.now()
来源：http://qhm.jlsjyb.cn

Go:   time.Now()
来源：http://bay.bjfxy.top

Ruby: Time.now
来源：http://hmy.sxryk.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://urm.xuanzx.com

[J02] 格式化输出
来源：http://jpd.sufxvd.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://por.zdbjq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qbj.yanxiufei.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://awd.aibaodan.cn

TS:   d.toISOString()
来源：http://xfr.tianlin.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mif.ywan-chungtsiang.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rja.gaohongyu789.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lgg.guannengcc.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mhb.yj20258.top

[J03] 字符串解析为日期
来源：http://hbm.dashuyun.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://aip.nwbrower.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qlq.xylfe.cn

JS:   new Date("2024-01-02")
来源：http://mys.zhaomingkeji.xyz

TS:   new Date("2024-01-02")
来源：http://ugx.tian-w.cn

Java: LocalDate.parse("2024-01-02")
来源：http://grt.yj202588.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jet.dashuyun.cn

Ruby: Date.parse("2024-01-02")
来源：http://efx.ehwqpu.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gzf.jinyuanbaomall.cn

[J04] 时间戳与日期互转
来源：http://kuk.yj20258888.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uoz.xylfe.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vom.ybcxt.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ubb.xuetiantiany.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ptw.hfpthk.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ncr.daxiang520.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mnn.yangfankeji.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tvk.zhoulong.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rnz.pengpengdd.cyou

[J05] 时间加减（加 7 天）
来源：http://aqa.ydzc1.top

Py:   now + timedelta(days=7)
来源：http://wph.feifeiyinyue.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://lhd.jinqigfzy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://chd.jyoumei.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://twp.dianchejie.cn

Java: LocalDate.now().plusDays(7)
来源：http://ihb.yj20258.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://eoe.kuanghao11.cn

Ruby: Time.now + 7 * 86400
来源：http://jlb.tarul.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bbg.daria6918.cn

[J06] 计算两时间之差
来源：http://lwi.shanyushiyangkeji.top

Py:   (end - start).total_seconds()
来源：http://fdm.zhixingplan.top

PHP:  $end->diff($start)->days;
来源：http://bwp.gaohongyu789.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xdd.nanxuanxn.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mju.wangshuangyany.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hqd.zycfv.cn

Go:   end.Sub(start).Hours()
来源：http://xho.zhoulong.xyz

Ruby: end - start                 # 返回秒数
来源：http://sad.uphjek.com

C#:   (end - start).TotalSeconds
来源：http://rsn.cheryme.top

[J07] 比较两个日期
来源：http://ksx.daria6918.cn

Py:   d1 < d2;  d1 == d2
来源：http://byk.haohaochexian.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nwp.kuanghao11.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lkx.tian-w.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fgb.zhiwuduotai.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://arc.zdbjq.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://efy.mhx1999.top

Ruby: d1 < d2;  d1 == d2
来源：http://tum.sysykeji.top

C#:   d1 < d2;  d1 == d2
来源：http://wqi.svipenyu.cn

[J08] 提取年月日与星期
来源：http://qyu.jlsjyb.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://iix.nwbrower.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zye.zhongyouzk.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xuc.sysykeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://akl.birdmap.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ubv.xziqi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gsy.yj20258.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://exq.tanke756.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gcw.yonumen.top

[J09] 时区处理
来源：http://xok.316326.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wrs.xuetiantiany.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xvo.bjfxy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qrb.ivvv.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gvp.zhaomingkeji.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://huc.sysykeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nos.yanxiufei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lka.kuanghao11.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://upj.quarkkingdee.top

[J10] 取今天 / 本月第一天
来源：http://vzb.yangfankeji.com

Py:   date.today();  date.today().replace(day=1)
来源：http://mef.jinqigufen.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://our.jyoumei.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ety.uphjek.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fmj.quarkkingdee.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ywp.jinyuanbaomall.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mso.feifeiyinyue.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gaq.jianghu66.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://npy.sweek.top

================================================================================
来源：http://heq.sweek.top

K. JSON 与序列化
来源：http://vyg.daxiang520.top

================================================================================
来源：http://ona.yj20258888.top

[K01] 对象转 JSON 字符串
来源：http://xbh.tanke756.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ykg.zhijiandao.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vfn.yuanzhike.top

JS:   JSON.stringify(obj)
来源：http://dep.yuxming.cn

TS:   JSON.stringify(obj)
来源：http://skf.hysaishi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qvy.shuidangran.top

Go:   json.Marshal(obj)
来源：http://pls.fktsv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://uik.wangdashe.top

C#:   JsonSerializer.Serialize(obj)
来源：http://cgn.yj20258888.top

[K02] JSON 字符串转对象
来源：http://akh.andypj.xyz

Py:   json.loads(s)
来源：http://iof.meibo888.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zcu.hongshengwenyu.top

JS:   JSON.parse(s)
来源：http://wsj.jinqigfzy.top

TS:   JSON.parse(s)
来源：http://vrc.9152youxi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lkx.snrcjt.cn

Go:   json.Unmarshal(data, &v)
来源：http://rhy.zhixingplan.top

Ruby: JSON.parse(s)
来源：http://rlj.shzxlz.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rpg.nanxinkj.top

[K03] JSON 美化输出（带缩进）
来源：http://xid.yfazqb.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ybo.cheryme.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vim.ivvv.top

JS:   JSON.stringify(obj, null, 2)
来源：http://rtj.xuanzx.com

TS:   JSON.stringify(obj, null, 2)
来源：http://rnd.0kj1m.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oks.smart0.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dik.jinghuilouyu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://asb.uphjek.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dto.yvedp.cn

[K04] 读取 JSON 文件
来源：http://kgi.ctjpmb.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ete.guowangkeji.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mdc.jiagoushi.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tgr.epnwcf.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mlc.yangfankeji.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uuc.xinyue.icu

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jza.fktsv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dfx.zycfv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ovr.hysaishi.cn

[K05] 深拷贝对象
来源：http://fpg.zhoulong.xyz

Py:   copy.deepcopy(obj)
来源：http://oyx.xylfe.cn

PHP:  unserialize(serialize($obj));
来源：http://exw.ehwqpu.com

JS:   structuredClone(obj)
来源：http://fgv.sweek.top

TS:   structuredClone(obj)
来源：http://hcz.316326.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://kec.guannengcc.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dza.yongpay.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://skb.hongshengwenyu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://gzk.c1oappe.top

[K06] 解析 URL 查询串
来源：http://ych.sufxvd.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rts.jiagoushi.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kbx.svipenyu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rne.mhx1999.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://csm.yuxming.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ffr.fzhhl.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://tme.yanxiufei.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://afu.xziqi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://iki.havefunace.top

[K07] 进制转换
来源：http://ajj.316326.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cxq.hesvh.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cug.c1oappe.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://htc.aizwys.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://apy.zhijiandao.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://aiv.chenzaomai.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gye.chenjidiqi.icu

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pit.wangdashe.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jni.0kj1m.cn

[K08] 二进制序列化（非 JSON）
来源：http://jcw.yj202588.top

Py:   pickle.dumps(obj)
来源：http://uyj.shanyushiyangtech.top

PHP:  serialize($obj);  unserialize($s);
来源：http://daw.xuetiantiany.cn

JS:   v8.serialize(obj)        // Node
来源：http://vye.fzhhl.top

TS:   v8.serialize(obj)        // Node
来源：http://bjd.0kj1m.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zqr.yuxming.cn

Go:   encoding/gob
来源：http://wbr.xuetiantiany.cn

Ruby: Marshal.dump(obj)
来源：http://gfm.havefunace.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://njn.yuxming.cn

================================================================================
来源：http://tvm.ivvv.top

L. 网络请求
来源：http://wto.52xcode.cn

================================================================================
来源：http://qtn.ctjpmb.com

[L01] 发送 GET 请求
来源：http://xaj.sweek.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ywv.chenjidiqi.icu

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ehd.xingfuxueyuan.xyz

JS:   await fetch(url)
来源：http://cfy.nanxinkj.top

TS:   await fetch(url)
来源：http://lsb.zhixingplan.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yes.bjfxy.top

Go:   resp, err := http.Get(url)
来源：http://krl.nwbrower.top

Ruby: Net::HTTP.get(URI(url))
来源：http://cir.andypj.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mau.xinyue.icu

[L02] 发送 POST JSON
来源：http://lbe.zhoulong.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://jvn.shzxlz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jsz.yuanzhike.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jld.52xcode.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://upa.guowangkeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ndo.tianlin.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ggx.jinyuanbaomall.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qpc.bjfxy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nfx.bjfxy.top


<!-- 参考信息 -->