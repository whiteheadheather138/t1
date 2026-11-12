代发 wailian999

[H07] 断言
来源：http://zvi.nwbrower.top

Py:   assert x > 0, "必须为正"
来源：http://swy.uphjek.com

PHP:  assert($x > 0);
来源：http://cle.hysaishi.cn

JS:   console.assert(x > 0);
来源：http://ynb.cqqwz.cn

TS:   console.assert(x > 0);
来源：http://hlb.gogol.net.cn

Java: assert x > 0 : "必须为正";
来源：http://bpa.gzhubu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wvg.yangfankeji.com

Ruby: raise "必须为正" unless x > 0
来源：http://wxo.chenzaomai.com

C#:   Debug.Assert(x > 0);
来源：http://kks.yuanzhike.top

[H08] 获取错误信息与堆栈
来源：http://adc.ydzc1.top

Py:   str(e);  traceback.format_exc()
来源：http://mef.jinqigufen.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://idl.wangshuangyany.cn

JS:   e.message;  e.stack
来源：http://uqb.jqgufenzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://psh.hongshengwenyu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ivk.yfazqb.com

Go:   err.Error()
来源：http://tzq.pycfn.com

Ruby: e.message;  e.backtrace
来源：http://vtt.zdqjudy.top

C#:   e.Message;  e.StackTrace
来源：http://rmd.jinqigfzy.top

[H09] 带错误码的异常
来源：http://mht.0kj1m.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://eep.haohaochexian.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://rrz.zhoulong.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rjk.sjlbkw.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pyr.wangdashe.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xlp.haohaochexian.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fmt.ctjpmb.com

Ruby: raise MyError.new("fail", 500)
来源：http://tey.vqdsnc.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ega.hcnkem.com

[H10] 资源自动释放
来源：http://ouo.redwolf501.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://bcg.jinghuilouyu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wxx.tianlin.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rvi.aibaodan.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tze.ydzc1.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cbc.jianghu66.top

Go:   defer f.Close()
来源：http://yvx.cashguo.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cht.mhx1999.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://okv.hfpthk.cn

================================================================================
来源：http://quo.zhoulong.xyz

I. 正则表达式
来源：http://ome.bjfxy.top

================================================================================
来源：http://lod.ydjk.org.cn

[I01] 判断是否匹配
来源：http://fsn.chenjidiqi.icu

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://msj.ydjk.org.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xha.redwolf501.top

JS:   /\d+/.test(s)
来源：http://who.xinyue.icu

TS:   /\d+/.test(s)
来源：http://hun.sufxvd.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nqx.sufxvd.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cov.andypj.xyz

Ruby: s.match?(/\d+/)
来源：http://fbz.nwbrower.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pgz.cashguo.top

[I02] 提取所有匹配
来源：http://tss.zhixingplan.top

Py:   re.findall(r"\d+", s)
来源：http://vni.yvedp.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hsa.zhijiandao.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://eog.redwolf501.top

TS:   s.match(/\d+/g)
来源：http://tig.chenjidiqi.icu

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ege.xuanzx.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cen.yueranfly.top

Ruby: s.scan(/\d+/)
来源：http://pnh.shangyingyoupin.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://woz.snrcjt.cn

[I03] 提取捕获分组
来源：http://osi.xuetiantiany.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zok.haohaochexian.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qdq.zhijiandao.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hqm.nanxuanxn.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qsw.gotoacloud.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rkp.zhijiandao.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://anv.tianlin.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://swy.hnqzz.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pny.sweek.top

[I04] 正则替换
来源：http://ngh.jlsjyb.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gee.shuidangran.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sfl.bjfxy.top

JS:   s.replace(/\d+/g, "#")
来源：http://hub.c1oappe.top

TS:   s.replace(/\d+/g, "#")
来源：http://gjc.haohaochexian.top

Java: s.replaceAll("\\d+", "#")
来源：http://tar.feifeiyinyue.top

Go:   re.ReplaceAllString(s, "#")
来源：http://qnv.sweek.top

Ruby: s.gsub(/\d+/, "#")
来源：http://tek.vehdjk.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fza.iojbl.cn

[I05] 按正则拆分
来源：http://igf.ctjpmb.com

Py:   re.split(r"\s*,\s*", s)
来源：http://xfy.daria6918.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xmd.smart0.xyz

JS:   s.split(/\s*,\s*/)
来源：http://vyf.fzhhl.top

TS:   s.split(/\s*,\s*/)
来源：http://yob.redwolf501.top

Java: s.split("\\s*,\\s*")
来源：http://tzq.ydzc1.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://eay.dianchejie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ecn.yongpay.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://god.jinqigufen.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hoi.ybcxt.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hxc.shanyushiyangkeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bbg.yj202588.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rsg.sufxvd.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://trt.jiagoushi.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://duc.shuidangran.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fub.pengpengdd.cyou

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jtc.jinyuanbaomall.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://amv.hysaishi.cn

[I07] 忽略大小写与多行模式
来源：http://xwp.zdbjq.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vwp.tarul.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nho.smart0.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://olx.sysykeji.top

TS:   /error/gim
来源：http://mck.jqgufenzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jad.sjlbkw.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lji.cqqwz.cn

Ruby: s.scan(/error/i)
来源：http://zja.hesvh.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cvj.birdmap.top

[I08] 贪婪与非贪婪匹配
来源：http://qyg.nwbrower.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zcj.hongshengwenyu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zvs.c1oappe.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jxy.zhaomingkeji.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pdf.sysykeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://csp.xinyue.icu

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://aea.pengpengdd.cyou

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mtp.xylfe.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hie.fanxiaobao.xyz

================================================================================
来源：http://gox.zhengqikj.top

J. 日期与时间
来源：http://nvx.ywan-chungtsiang.top

================================================================================
来源：http://qbs.snrcjt.cn

[J01] 获取当前时间
来源：http://aed.0kj1m.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xqd.ehwqpu.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hou.fktsv.cn

JS:   new Date();  Date.now()
来源：http://rpd.nwbrower.top

TS:   new Date();  Date.now()
来源：http://mkv.xuanzx.com

Java: LocalDateTime.now();  Instant.now()
来源：http://uvb.0kj1m.cn

Go:   time.Now()
来源：http://nzy.jqgfzy.top

Ruby: Time.now
来源：http://wnp.aizwys.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jid.pengpengdd.cyou

[J02] 格式化输出
来源：http://xnb.meibo888.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nqj.hongshengwenyu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kui.fehbvm.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uhz.tian-w.cn

TS:   d.toISOString()
来源：http://owf.smart0.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mqo.smart0.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://aov.fanxiaobao.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uux.chenlongwang.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qzn.svipenyu.cn

[J03] 字符串解析为日期
来源：http://kpu.chenjidiqi.icu

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bzg.jinqigufen.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jdb.jqgufenzy.top

JS:   new Date("2024-01-02")
来源：http://sjc.pycfn.com

TS:   new Date("2024-01-02")
来源：http://mvd.bbcook.cn

Java: LocalDate.parse("2024-01-02")
来源：http://eci.zycfv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zie.cdnleiting.top

Ruby: Date.parse("2024-01-02")
来源：http://wej.guowangkeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kvg.fktsv.cn

[J04] 时间戳与日期互转
来源：http://mst.daxiang520.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rxw.hnqzz.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nkx.redwolf501.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qkg.hywenlv.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yus.vqdsnc.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://irv.gaohongyu789.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wbx.kuanghao11.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mma.hongshengwenyu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ksy.zdbjq.cn

[J05] 时间加减（加 7 天）
来源：http://tqf.yuxming.cn

Py:   now + timedelta(days=7)
来源：http://fth.fzhhl.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://zmr.yuanzhike.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://srn.cucudq.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zdo.yongpay.top

Java: LocalDate.now().plusDays(7)
来源：http://fue.sweek.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://oah.aizwys.cn

Ruby: Time.now + 7 * 86400
来源：http://tnb.cqqwz.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qgx.quarkkingdee.top

[J06] 计算两时间之差
来源：http://uol.chenzaomai.com

Py:   (end - start).total_seconds()
来源：http://rjn.chenjidiqi.icu

PHP:  $end->diff($start)->days;
来源：http://ahv.jiagoushi.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://frw.zdqjudy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rwl.jinghuilouyu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rtt.hfpthk.cn

Go:   end.Sub(start).Hours()
来源：http://puw.cucudq.cn

Ruby: end - start                 # 返回秒数
来源：http://pbz.iojbl.cn

C#:   (end - start).TotalSeconds
来源：http://xmk.0kj1m.cn

[J07] 比较两个日期
来源：http://mja.birdmap.top

Py:   d1 < d2;  d1 == d2
来源：http://tmb.ywan-chungtsiang.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vuu.cucudq.cn

JS:   d1.getTime() < d2.getTime()
来源：http://eey.fehbvm.com

TS:   d1.getTime() < d2.getTime()
来源：http://onx.svipenyu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uoy.zdbjq.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://aoz.sweek.top

Ruby: d1 < d2;  d1 == d2
来源：http://dsi.andypj.xyz

C#:   d1 < d2;  d1 == d2
来源：http://pwy.hnxiangtu.top

[J08] 提取年月日与星期
来源：http://gsw.zhixingplan.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ccq.shuidangran.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baz.ivvv.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vel.gogol.net.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dah.hesvh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gdh.gzhubu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qne.ybcxt.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pba.fanxiaobao.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dpm.smart0.xyz

[J09] 时区处理
来源：http://gpr.zhaomingkeji.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cmg.hnqzz.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://htt.fehbvm.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mqk.daxiang520.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ekb.smart0.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vlg.tarul.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ucd.xingfuxueyuan.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://zov.fehbvm.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jfe.cdnleiting.top

[J10] 取今天 / 本月第一天
来源：http://dqr.hongshengwenyu.top

Py:   date.today();  date.today().replace(day=1)
来源：http://brn.yuanzhike.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qca.aizwys.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://shs.fktsv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hcj.vehdjk.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rti.jqgufenzy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xan.ydzc1.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cmd.shzxlz.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oqu.hfpthk.cn

================================================================================
来源：http://vqo.fanxiaobao.xyz

K. JSON 与序列化
来源：http://yhx.gzhubu.top

================================================================================
来源：http://avu.redwolf501.top

[K01] 对象转 JSON 字符串
来源：http://jtw.pengpengdd.cyou

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ccq.gotoacloud.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://asp.svipenyu.cn

JS:   JSON.stringify(obj)
来源：http://iiv.quarkkingdee.top

TS:   JSON.stringify(obj)
来源：http://pep.zhijiandao.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://iti.gogol.net.cn

Go:   json.Marshal(obj)
来源：http://jrl.jinghuilouyu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://tsn.dianchejie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://iso.aizwys.cn

[K02] JSON 字符串转对象
来源：http://oln.quarkkingdee.top

Py:   json.loads(s)
来源：http://nfi.aizwys.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bor.nanxuanxn.top

JS:   JSON.parse(s)
来源：http://ptf.sxryk.cn

TS:   JSON.parse(s)
来源：http://ems.xziqi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mck.c1oappe.top

Go:   json.Unmarshal(data, &v)
来源：http://kdp.quarkkingdee.top

Ruby: JSON.parse(s)
来源：http://lfo.yj20258.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wuj.jinqigufen.top

[K03] JSON 美化输出（带缩进）
来源：http://kco.dashuyun.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mgm.yongpay.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cph.havefunace.top

JS:   JSON.stringify(obj, null, 2)
来源：http://fjr.yanxiufei.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bjh.yj20258888.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://htp.fehbvm.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nkj.dianchejie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pot.xuetiantiany.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rxl.yvedp.cn

[K04] 读取 JSON 文件
来源：http://lrq.cheryme.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bik.wangshuangyany.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dhi.zhixingplan.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fqf.vehdjk.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xun.dashuyun.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://msz.yongpay.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ird.shanyushiyangkeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://boj.guannengcc.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fju.nanxuanxn.top

[K05] 深拷贝对象
来源：http://bce.jinyuanbaomall.cn

Py:   copy.deepcopy(obj)
来源：http://wgk.ydzc1.top

PHP:  unserialize(serialize($obj));
来源：http://rxp.ehwqpu.com

JS:   structuredClone(obj)
来源：http://etu.jianghu66.top

TS:   structuredClone(obj)
来源：http://law.52xcode.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://stu.hongshengwenyu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vjl.gogol.net.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wen.dianchejie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rtw.smart0.xyz

[K06] 解析 URL 查询串
来源：http://swt.shzxlz.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rfi.cashguo.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xwk.fzhhl.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xdn.gzhubu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sll.sufxvd.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xse.fehbvm.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://mmy.sxryk.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://foj.zdbjq.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gsq.ywan-chungtsiang.top

[K07] 进制转换
来源：http://rba.gzhubu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pfo.gotoacloud.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kam.zhijiandao.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://emw.jlsjyb.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://csy.hysaishi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://olt.zhijiandao.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jmd.hfpthk.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jji.havefunace.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dwc.kuanghao11.cn

[K08] 二进制序列化（非 JSON）
来源：http://osg.0kj1m.cn

Py:   pickle.dumps(obj)
来源：http://zpd.zhaomingkeji.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://bwg.c1oappe.top

JS:   v8.serialize(obj)        // Node
来源：http://rxm.zdbjq.cn

TS:   v8.serialize(obj)        // Node
来源：http://nbm.ivvv.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wpy.hongshengwenyu.top

Go:   encoding/gob
来源：http://zew.pengpengdd.cyou

Ruby: Marshal.dump(obj)
来源：http://sym.shzxlz.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hkf.9152youxi.cn

================================================================================
来源：http://dgt.yangfankeji.com

L. 网络请求
来源：http://dbq.tarul.cn

================================================================================
来源：http://yiy.yueranfly.top

[L01] 发送 GET 请求
来源：http://xfk.jqgufenzy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xyo.snrcjt.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nka.c1oappe.top

JS:   await fetch(url)
来源：http://apj.jqgfzy.top

TS:   await fetch(url)
来源：http://tkg.daria6918.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xef.kuanghao11.cn

Go:   resp, err := http.Get(url)
来源：http://kbu.nanxuanxn.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ezg.yvedp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vok.zhiwuduotai.top

[L02] 发送 POST JSON
来源：http://mvv.9152youxi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vqn.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ctu.316326.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dmw.cheryme.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bzc.epnwcf.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xhz.tanke756.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yzw.cucudq.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://for.shuidangran.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://djo.jyoumei.cn


<!-- 参考信息 -->