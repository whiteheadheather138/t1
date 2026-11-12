代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://hhw.sxryk.cn

C#:   e.Message;  e.StackTrace
来源：http://isv.zdbjq.cn

[H09] 带错误码的异常
来源：http://daq.tanke756.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yjr.svipenyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wxz.hesvh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gyn.zdbjq.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tdg.haohaochexian.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://agm.hywenlv.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://irm.aibaodan.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ppy.pengpengdd.cyou

C#:   // 自定义异常类中加 Code 属性
来源：http://atw.andypj.xyz

[H10] 资源自动释放
来源：http://ysn.ybcxt.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://wlh.shuidangran.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tsu.jiagoushi.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xtr.haohaochexian.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ozg.smart0.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://awp.sxryk.cn

Go:   defer f.Close()
来源：http://emd.nanxinkj.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://syc.cqqwz.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dpt.tian-w.cn

================================================================================
来源：http://pjp.havefunace.top

I. 正则表达式
来源：http://cxd.shangyingyoupin.top

================================================================================
来源：http://szy.hfpthk.cn

[I01] 判断是否匹配
来源：http://yxk.zdbjq.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lrg.shuidangran.top

PHP:  preg_match('/\d+/', $s);
来源：http://kla.yfazqb.com

JS:   /\d+/.test(s)
来源：http://fev.yangfankeji.com

TS:   /\d+/.test(s)
来源：http://kib.xingfuxueyuan.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yjm.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wjk.xuanzx.com

Ruby: s.match?(/\d+/)
来源：http://tap.jianghu66.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blr.yueranfly.top

[I02] 提取所有匹配
来源：http://puv.ydzc1.top

Py:   re.findall(r"\d+", s)
来源：http://ity.xinyue.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pck.yfazqb.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wpb.nwbrower.top

TS:   s.match(/\d+/g)
来源：http://qjb.cheryme.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://aws.yangfankeji.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yxa.aibaodan.cn

Ruby: s.scan(/\d+/)
来源：http://wmt.yfazqb.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rzf.fengsongda.top

[I03] 提取捕获分组
来源：http://eub.tanke756.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vwy.zhoulong.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ycv.yuxming.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://grp.xziqi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ehj.hfpthk.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ijl.316326.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vqy.xinyue.icu

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gon.sjlbkw.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://klh.hnxiangtu.top

[I04] 正则替换
来源：http://xrh.jqgfzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://djj.zhoulong.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ucl.andypj.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://ogu.hongshengwenyu.top

TS:   s.replace(/\d+/g, "#")
来源：http://jzr.xinyue.icu

Java: s.replaceAll("\\d+", "#")
来源：http://dkr.aibaodan.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://tib.sysykeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://dvg.sxryk.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zzy.jqgufenzy.top

[I05] 按正则拆分
来源：http://ozf.fengsongda.top

Py:   re.split(r"\s*,\s*", s)
来源：http://iai.ehwqpu.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ofl.yj20258.top

JS:   s.split(/\s*,\s*/)
来源：http://ibq.xylfe.cn

TS:   s.split(/\s*,\s*/)
来源：http://ebr.52xcode.cn

Java: s.split("\\s*,\\s*")
来源：http://zwz.shzxlz.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sdt.wangdashe.top

Ruby: s.split(/\s*,\s*/)
来源：http://yhz.jlsjyb.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rqw.feifeiyinyue.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qxb.shzxlz.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ifh.jinghuilouyu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vgd.birdmap.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://avc.ehwqpu.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vad.feifeiyinyue.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cyw.zhengqikj.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bmb.yanxiufei.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mxv.quarkkingdee.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rcs.zhixingplan.top

[I07] 忽略大小写与多行模式
来源：http://hle.svipenyu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://toi.ctjpmb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ptf.tanke756.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ojp.zhaomingkeji.xyz

TS:   /error/gim
来源：http://poo.gogol.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rtk.ppjwa.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://eis.vqdsnc.cn

Ruby: s.scan(/error/i)
来源：http://gqx.ydzc1.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zgd.tian-w.cn

[I08] 贪婪与非贪婪匹配
来源：http://cjt.cucudq.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kyz.zhixingplan.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wrp.yueranfly.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ilr.aibaodan.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mvr.yuxming.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://mjy.ydjk.org.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jxy.tian-w.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rmh.jiagoushi.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://het.fehbvm.com

================================================================================
来源：http://fxt.birdmap.top

J. 日期与时间
来源：http://ics.jinqigufen.top

================================================================================
来源：http://ihg.nwbrower.top

[J01] 获取当前时间
来源：http://qjw.dashuyun.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lua.9152youxi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kzb.hongshengwenyu.top

JS:   new Date();  Date.now()
来源：http://gtu.vehdjk.com

TS:   new Date();  Date.now()
来源：http://hib.jiagoushi.top

Java: LocalDateTime.now();  Instant.now()
来源：http://gci.xylfe.cn

Go:   time.Now()
来源：http://eli.chenjidiqi.icu

Ruby: Time.now
来源：http://qyr.daria6918.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bmm.yongpay.top

[J02] 格式化输出
来源：http://qzt.dashuyun.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yrr.nanxinkj.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://emz.fehbvm.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ekk.dianchejie.cn

TS:   d.toISOString()
来源：http://nsi.hnqzz.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kdk.yfazqb.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tev.zhijiandao.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bbi.sjlbkw.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://awe.yj20258.top

[J03] 字符串解析为日期
来源：http://bmb.0kj1m.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cus.jqgufenzy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rnh.yueranfly.top

JS:   new Date("2024-01-02")
来源：http://jft.fktsv.cn

TS:   new Date("2024-01-02")
来源：http://aje.ctjpmb.com

Java: LocalDate.parse("2024-01-02")
来源：http://hbt.nanxuanxn.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bgk.hcnkem.com

Ruby: Date.parse("2024-01-02")
来源：http://wpp.yangfankeji.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ejs.jianghu66.top

[J04] 时间戳与日期互转
来源：http://kbe.chenjidiqi.icu

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uxj.vqdsnc.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mpx.zhixingplan.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rgl.zhengqikj.top

TS:   Math.floor(Date.now() / 1000)
来源：http://yce.zhixingplan.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mrt.cashguo.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uxj.yonumen.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sym.fengsongda.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://clx.0kj1m.cn

[J05] 时间加减（加 7 天）
来源：http://pyu.ehwqpu.com

Py:   now + timedelta(days=7)
来源：http://nvv.gogol.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://djv.jyoumei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nkv.sjlbkw.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lya.haohaochexian.top

Java: LocalDate.now().plusDays(7)
来源：http://utb.hongshengwenyu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mdz.hywenlv.cn

Ruby: Time.now + 7 * 86400
来源：http://gsn.feifeiyinyue.top

C#:   DateTime.Now.AddDays(7)
来源：http://axb.wangdashe.top

[J06] 计算两时间之差
来源：http://rrz.hysaishi.cn

Py:   (end - start).total_seconds()
来源：http://dys.nanxuanxn.top

PHP:  $end->diff($start)->days;
来源：http://zfv.yangfankeji.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pxq.fanxiaobao.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uyq.xziqi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gbr.wangshuangyany.cn

Go:   end.Sub(start).Hours()
来源：http://lbi.yj20258888.top

Ruby: end - start                 # 返回秒数
来源：http://msy.sweek.top

C#:   (end - start).TotalSeconds
来源：http://wbt.vqdsnc.cn

[J07] 比较两个日期
来源：http://hsc.hysaishi.cn

Py:   d1 < d2;  d1 == d2
来源：http://spo.cucudq.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vvc.birdmap.top

JS:   d1.getTime() < d2.getTime()
来源：http://swi.havefunace.top

TS:   d1.getTime() < d2.getTime()
来源：http://sdw.hongshengwenyu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nfa.52xcode.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nqb.hywenlv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qii.pycfn.com

C#:   d1 < d2;  d1 == d2
来源：http://teq.sysykeji.top

[J08] 提取年月日与星期
来源：http://avn.52xcode.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sdi.hywenlv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nli.iojbl.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://een.gzhubu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bwt.vqdsnc.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sgl.zhiwuduotai.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hmv.jinyuanbaomall.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gwu.hcnkem.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ajn.xylfe.cn

[J09] 时区处理
来源：http://uwi.zdqjudy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qin.nanxinkj.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ual.meibo888.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fyp.dianchejie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wgh.vqdsnc.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yio.jqgfzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fwr.ctjpmb.com

Ruby: Time.now.getlocal("+08:00")
来源：http://xrm.zdbjq.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kjl.hfpthk.cn

[J10] 取今天 / 本月第一天
来源：http://qeq.yangfankeji.com

Py:   date.today();  date.today().replace(day=1)
来源：http://vuj.fzhhl.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://orx.jinghuilouyu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xcn.316326.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://adz.snrcjt.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://aag.hesvh.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gcw.smart0.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://goc.bbcook.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gqa.xuanzx.com

================================================================================
来源：http://avg.sufxvd.cn

K. JSON 与序列化
来源：http://zqh.zycfv.cn

================================================================================
来源：http://gsy.yanxiufei.cn

[K01] 对象转 JSON 字符串
来源：http://zjg.bjfxy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lwz.yuxming.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ccb.yuanzhike.top

JS:   JSON.stringify(obj)
来源：http://cut.xinyue.icu

TS:   JSON.stringify(obj)
来源：http://uzn.nanxuanxn.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yyj.havefunace.top

Go:   json.Marshal(obj)
来源：http://uyh.yj20258.top

Ruby: obj.to_json                                     // require "json"
来源：http://hzx.shangyingyoupin.top

C#:   JsonSerializer.Serialize(obj)
来源：http://xxz.guowangkeji.top

[K02] JSON 字符串转对象
来源：http://hnw.xylfe.cn

Py:   json.loads(s)
来源：http://xap.jqgfzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ntz.cqqwz.cn

JS:   JSON.parse(s)
来源：http://uza.pengpengdd.cyou

TS:   JSON.parse(s)
来源：http://phd.sxryk.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://eky.zdqjudy.top

Go:   json.Unmarshal(data, &v)
来源：http://fyd.shuidangran.top

Ruby: JSON.parse(s)
来源：http://aly.cdnleiting.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vgv.xuetiantiany.cn

[K03] JSON 美化输出（带缩进）
来源：http://lzn.zhiwuduotai.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tdb.hywenlv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vjo.dashuyun.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://lms.sysykeji.top

TS:   JSON.stringify(obj, null, 2)
来源：http://awq.havefunace.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pqj.andypj.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mwq.meibo888.top

Ruby: JSON.pretty_generate(obj)
来源：http://aul.mhx1999.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ekz.gotoacloud.top

[K04] 读取 JSON 文件
来源：http://kst.guowangkeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ctz.meibo888.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lrh.smart0.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://itl.pengpengdd.cyou

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hft.xingfuxueyuan.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fiv.gogol.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hhv.sjlbkw.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jcw.xziqi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xum.epnwcf.com

[K05] 深拷贝对象
来源：http://eis.yanxiufei.cn

Py:   copy.deepcopy(obj)
来源：http://gyt.pengpengdd.cyou

PHP:  unserialize(serialize($obj));
来源：http://kyd.zycfv.cn

JS:   structuredClone(obj)
来源：http://zqq.jinghuilouyu.cn

TS:   structuredClone(obj)
来源：http://fqu.gotoacloud.top

Java: // 手写拷贝构造，或序列化往返
来源：http://kiq.tian-w.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vdi.jyoumei.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bbr.meibo888.top

C#:   // 序列化往返，或自定义 Clone
来源：http://rds.tian-w.cn

[K06] 解析 URL 查询串
来源：http://sib.xuetiantiany.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ovn.yuanzhike.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fpw.bbcook.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xtt.fengsongda.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oxg.xinyue.icu

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ywa.cucudq.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://jok.jinghuilouyu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://loc.9152youxi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lub.jiagoushi.top

[K07] 进制转换
来源：http://gff.zhoulong.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yhh.sweek.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rdn.jiagoushi.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cgx.jqgufenzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mkd.zhiwuduotai.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://psv.fanxiaobao.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vmz.kuanghao11.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vok.guannengcc.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gjm.tian-w.cn

[K08] 二进制序列化（非 JSON）
来源：http://zub.gotoacloud.top

Py:   pickle.dumps(obj)
来源：http://xck.tanke756.top

PHP:  serialize($obj);  unserialize($s);
来源：http://fra.yonumen.top

JS:   v8.serialize(obj)        // Node
来源：http://wza.quarkkingdee.top

TS:   v8.serialize(obj)        // Node
来源：http://jcg.ydzc1.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fvh.aibaodan.cn

Go:   encoding/gob
来源：http://fzs.redwolf501.top

Ruby: Marshal.dump(obj)
来源：http://nos.yongpay.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qlt.sysykeji.top

================================================================================
来源：http://uac.iojbl.cn

L. 网络请求
来源：http://gcs.kuanghao11.cn

================================================================================
来源：http://opj.hnxiangtu.top

[L01] 发送 GET 请求
来源：http://lmb.hnqzz.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xcn.zdbjq.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yws.zycfv.cn

JS:   await fetch(url)
来源：http://tpz.redwolf501.top

TS:   await fetch(url)
来源：http://ush.smart0.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ppx.fzhhl.top

Go:   resp, err := http.Get(url)
来源：http://erq.dashuyun.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://aoa.guowangkeji.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uvt.tian-w.cn

[L02] 发送 POST JSON
来源：http://ygh.yueranfly.top

Py:   requests.post(url, json={"a": 1})
来源：http://bjc.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dom.jinqigfzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kpu.ywan-chungtsiang.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kph.aibaodan.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xpa.cheryme.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jeb.epnwcf.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://axl.c1oappe.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gry.c1oappe.top

[L03] 设置自定义请求头
来源：http://ncl.tanke756.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gtf.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kad.yongpay.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jqi.cucudq.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bpq.tianlin.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zak.c1oappe.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ett.epnwcf.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zha.guowangkeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ggg.zdbjq.cn

[L04] 设置超时
来源：http://wfp.dianchejie.cn

Py:   requests.get(url, timeout=5)
来源：http://uci.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qqo.tian-w.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://beq.daxiang520.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xoj.hysaishi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://new.gaohongyu789.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tsh.jiagoushi.top


<!-- 参考信息 -->