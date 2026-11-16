代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://mdj.yj20258.top

[H08] 获取错误信息与堆栈
来源：http://bzk.pengpengdd.cyou

Py:   str(e);  traceback.format_exc()
来源：http://alb.tarul.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wde.gaohongyu789.top

JS:   e.message;  e.stack
来源：http://owk.sufxvd.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qps.c1oappe.top

Java: e.getMessage();  e.printStackTrace()
来源：http://zay.epnwcf.com

Go:   err.Error()
来源：http://szd.0kj1m.cn

Ruby: e.message;  e.backtrace
来源：http://mdw.shangyingyoupin.top

C#:   e.Message;  e.StackTrace
来源：http://pif.hesvh.cn

[H09] 带错误码的异常
来源：http://adm.fzhhl.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://som.wangshuangyany.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://lre.shanyushiyangtech.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://llc.smart0.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xjp.aizwys.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fnt.hnxiangtu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://igy.zhengqikj.top

Ruby: raise MyError.new("fail", 500)
来源：http://kwa.52xcode.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://izo.gzhubu.top

[H10] 资源自动释放
来源：http://olu.tanke756.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://xns.jiagoushi.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jwc.cqqwz.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://idz.xinyue.icu

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bpq.snrcjt.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://scw.xuetiantiany.cn

Go:   defer f.Close()
来源：http://ywc.fzhhl.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://amf.cdnleiting.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fpl.mhx1999.top

================================================================================
来源：http://hwx.sjlbkw.cn

I. 正则表达式
来源：http://pts.316326.xyz

================================================================================
来源：http://pke.fzhhl.top

[I01] 判断是否匹配
来源：http://fwr.shzxlz.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xvc.yangfankeji.com

PHP:  preg_match('/\d+/', $s);
来源：http://uff.wangshuangyany.cn

JS:   /\d+/.test(s)
来源：http://nim.gaohongyu789.top

TS:   /\d+/.test(s)
来源：http://gkz.ywan-chungtsiang.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://joz.yvedp.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mtd.guowangkeji.top

Ruby: s.match?(/\d+/)
来源：http://rsq.snrcjt.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://coq.jiagoushi.top

[I02] 提取所有匹配
来源：http://vbs.yuanzhike.top

Py:   re.findall(r"\d+", s)
来源：http://zyc.gaohongyu789.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://usa.quarkkingdee.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vrk.jianghu66.top

TS:   s.match(/\d+/g)
来源：http://kbr.svipenyu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gtu.316326.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jjs.guannengcc.top

Ruby: s.scan(/\d+/)
来源：http://fst.xziqi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ooc.yfazqb.com

[I03] 提取捕获分组
来源：http://vmu.zhengqikj.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://goj.tian-w.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qss.ehwqpu.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kdx.fktsv.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tpd.dashuyun.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zpq.ehwqpu.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pca.tian-w.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jdy.sufxvd.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nxb.guannengcc.top

[I04] 正则替换
来源：http://dkc.jyoumei.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xso.jinyuanbaomall.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wwz.nwbrower.top

JS:   s.replace(/\d+/g, "#")
来源：http://wkc.jlsjyb.cn

TS:   s.replace(/\d+/g, "#")
来源：http://evr.chenjidiqi.icu

Java: s.replaceAll("\\d+", "#")
来源：http://cto.xinyue.icu

Go:   re.ReplaceAllString(s, "#")
来源：http://jqs.bjfxy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://nho.hfpthk.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fiz.yonumen.top

[I05] 按正则拆分
来源：http://qdr.haohaochexian.top

Py:   re.split(r"\s*,\s*", s)
来源：http://xhc.birdmap.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://iia.xuanzx.com

JS:   s.split(/\s*,\s*/)
来源：http://pyv.guannengcc.top

TS:   s.split(/\s*,\s*/)
来源：http://xfi.yvedp.cn

Java: s.split("\\s*,\\s*")
来源：http://ils.jiagoushi.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gop.cashguo.top

Ruby: s.split(/\s*,\s*/)
来源：http://jgo.ctjpmb.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nak.xingfuxueyuan.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rsw.nanxuanxn.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://idl.gogol.net.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://itq.aizwys.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rvn.haohaochexian.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lqs.cheryme.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://knn.cqqwz.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fnp.xingfuxueyuan.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://toq.zhixingplan.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://teg.yueranfly.top

[I07] 忽略大小写与多行模式
来源：http://qkj.yueranfly.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://egz.dashuyun.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ahn.yuanzhike.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bdq.xingfuxueyuan.xyz

TS:   /error/gim
来源：http://pja.bjfxy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qcx.haohaochexian.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pkg.xuanzx.com

Ruby: s.scan(/error/i)
来源：http://uqy.guowangkeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rjk.sysykeji.top

[I08] 贪婪与非贪婪匹配
来源：http://rlr.sweek.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://brk.sweek.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gau.jqgufenzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://aaa.yongpay.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jal.xuetiantiany.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://yji.zdqjudy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fmh.aibaodan.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rpk.9152youxi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fpd.hnqzz.top

================================================================================
来源：http://jkk.yanxiufei.cn

J. 日期与时间
来源：http://hrf.fzhhl.top

================================================================================
来源：http://wou.svipenyu.cn

[J01] 获取当前时间
来源：http://dlz.guannengcc.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://eyo.xuetiantiany.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://djb.aizwys.cn

JS:   new Date();  Date.now()
来源：http://izk.guowangkeji.top

TS:   new Date();  Date.now()
来源：http://jfi.dianchejie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jey.tianlin.xyz

Go:   time.Now()
来源：http://sha.nanxuanxn.top

Ruby: Time.now
来源：http://mvk.shuidangran.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://szz.tanke756.top

[J02] 格式化输出
来源：http://pnr.9152youxi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://toq.zhiwuduotai.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://byo.aizwys.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://edu.yongpay.top

TS:   d.toISOString()
来源：http://nez.sweek.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xcx.meibo888.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fok.guowangkeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vuz.fehbvm.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qee.fehbvm.com

[J03] 字符串解析为日期
来源：http://pnw.zdbjq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://laz.fktsv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xes.uphjek.com

JS:   new Date("2024-01-02")
来源：http://tlm.iojbl.cn

TS:   new Date("2024-01-02")
来源：http://tqz.zhoulong.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://lbx.cheryme.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://znh.gogol.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://zmf.zdbjq.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ouy.jinyuanbaomall.cn

[J04] 时间戳与日期互转
来源：http://kle.ppjwa.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://knl.iojbl.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kaq.nwbrower.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://krk.chenzaomai.com

TS:   Math.floor(Date.now() / 1000)
来源：http://zgo.fktsv.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fty.shangyingyoupin.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vjl.yj202588.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ynr.zdbjq.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gqq.nwbrower.top

[J05] 时间加减（加 7 天）
来源：http://avr.hongshengwenyu.top

Py:   now + timedelta(days=7)
来源：http://wux.aizwys.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://uyy.yonumen.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qvk.ppjwa.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hit.zhixingplan.top

Java: LocalDate.now().plusDays(7)
来源：http://jia.nanxinkj.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uei.andypj.xyz

Ruby: Time.now + 7 * 86400
来源：http://slk.jinqigufen.top

C#:   DateTime.Now.AddDays(7)
来源：http://tof.hfpthk.cn

[J06] 计算两时间之差
来源：http://yim.cashguo.top

Py:   (end - start).total_seconds()
来源：http://hhh.xingfuxueyuan.xyz

PHP:  $end->diff($start)->days;
来源：http://lrc.pycfn.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://olv.jlsjyb.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kky.guowangkeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://cbb.ydjk.org.cn

Go:   end.Sub(start).Hours()
来源：http://aca.jlsjyb.cn

Ruby: end - start                 # 返回秒数
来源：http://pdp.316326.xyz

C#:   (end - start).TotalSeconds
来源：http://rjs.pengpengdd.cyou

[J07] 比较两个日期
来源：http://psk.shangyingyoupin.top

Py:   d1 < d2;  d1 == d2
来源：http://zvi.snrcjt.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cdq.vqdsnc.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yur.wangdashe.top

TS:   d1.getTime() < d2.getTime()
来源：http://tan.svipenyu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dum.jinghuilouyu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ech.jyoumei.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lli.wangshuangyany.cn

C#:   d1 < d2;  d1 == d2
来源：http://mud.dianchejie.cn

[J08] 提取年月日与星期
来源：http://gzr.jlsjyb.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vsi.xylfe.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xpo.sweek.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vej.haohaochexian.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ums.nanxinkj.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ajb.redwolf501.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zlv.jinqigfzy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://apj.yuxming.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://juw.fktsv.cn

[J09] 时区处理
来源：http://xbn.c1oappe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lta.jiagoushi.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://oeh.xinyue.icu

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://prt.zhiwuduotai.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vof.yongpay.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rgg.chenjidiqi.icu

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pwr.dashuyun.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://afb.zhaomingkeji.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rjr.zdqjudy.top

[J10] 取今天 / 本月第一天
来源：http://ume.ybcxt.top

Py:   date.today();  date.today().replace(day=1)
来源：http://liy.cheryme.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ylg.daxiang520.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://psv.zhengqikj.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mhw.cheryme.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ysn.guannengcc.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yjr.svipenyu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://urz.yuxming.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lcw.bjfxy.top

================================================================================
来源：http://hot.smart0.xyz

K. JSON 与序列化
来源：http://wrh.sysykeji.top

================================================================================
来源：http://hnw.sxryk.cn

[K01] 对象转 JSON 字符串
来源：http://shc.guowangkeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zgg.chenjidiqi.icu

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://asz.fengsongda.top

JS:   JSON.stringify(obj)
来源：http://yie.vehdjk.com

TS:   JSON.stringify(obj)
来源：http://lnk.chenlongwang.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ghb.chenzaomai.com

Go:   json.Marshal(obj)
来源：http://hbk.9152youxi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qiv.hysaishi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xei.sjlbkw.cn

[K02] JSON 字符串转对象
来源：http://ims.hfpthk.cn

Py:   json.loads(s)
来源：http://yzb.cashguo.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://erg.xingfuxueyuan.xyz

JS:   JSON.parse(s)
来源：http://pdq.aibaodan.cn

TS:   JSON.parse(s)
来源：http://qfw.hcnkem.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pns.gotoacloud.top

Go:   json.Unmarshal(data, &v)
来源：http://crp.aibaodan.cn

Ruby: JSON.parse(s)
来源：http://dum.sweek.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pzg.hesvh.cn

[K03] JSON 美化输出（带缩进）
来源：http://bdy.shzxlz.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://acx.daria6918.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hol.zdbjq.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qum.redwolf501.top

TS:   JSON.stringify(obj, null, 2)
来源：http://vgw.chenjidiqi.icu

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sbl.jlsjyb.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qps.bjfxy.top

Ruby: JSON.pretty_generate(obj)
来源：http://nuu.yanxiufei.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zdy.yvedp.cn

[K04] 读取 JSON 文件
来源：http://abr.sysykeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hbj.52xcode.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jvo.hammf.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vpi.xinyue.icu

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ptx.sysykeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tlo.xinyue.icu

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dma.hysaishi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://het.shuidangran.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bxq.cashguo.top

[K05] 深拷贝对象
来源：http://pru.xinyue.icu

Py:   copy.deepcopy(obj)
来源：http://lrf.svipenyu.cn

PHP:  unserialize(serialize($obj));
来源：http://hck.xinyue.icu

JS:   structuredClone(obj)
来源：http://fec.bjfxy.top

TS:   structuredClone(obj)
来源：http://qui.uphjek.com

Java: // 手写拷贝构造，或序列化往返
来源：http://yes.ctjpmb.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zgm.jinyuanbaomall.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ymn.zhixingplan.top

C#:   // 序列化往返，或自定义 Clone
来源：http://smd.fzhhl.top

[K06] 解析 URL 查询串
来源：http://yzu.jqgufenzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xrr.chenzaomai.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xxm.yj20258888.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zph.jinghuilouyu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wqs.birdmap.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xvp.zhiwuduotai.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://lnv.aizwys.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hzn.zhoulong.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uyw.cashguo.top

[K07] 进制转换
来源：http://bal.ctjpmb.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hcz.jianghu66.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jgn.yangfankeji.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vrb.zhijiandao.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fiq.birdmap.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qrc.haohaochexian.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tky.sxryk.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://woy.yueranfly.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pci.yj20258.top

[K08] 二进制序列化（非 JSON）
来源：http://gsm.cdnleiting.top

Py:   pickle.dumps(obj)
来源：http://uul.shzxlz.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sua.zdqjudy.top

JS:   v8.serialize(obj)        // Node
来源：http://bta.andypj.xyz

TS:   v8.serialize(obj)        // Node
来源：http://bji.chenjidiqi.icu

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lek.kuanghao11.cn

Go:   encoding/gob
来源：http://iur.nanxinkj.top

Ruby: Marshal.dump(obj)
来源：http://tst.xuanzx.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vut.jinqigfzy.top

================================================================================
来源：http://eph.nanxinkj.top

L. 网络请求
来源：http://ehb.yangfankeji.com

================================================================================
来源：http://ozr.tarul.cn

[L01] 发送 GET 请求
来源：http://jeq.9152youxi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pvu.chenlongwang.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wbr.andypj.xyz

JS:   await fetch(url)
来源：http://sjn.guannengcc.top

TS:   await fetch(url)
来源：http://yod.jinghuilouyu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://phs.fktsv.cn

Go:   resp, err := http.Get(url)
来源：http://grp.jinqigufen.top

Ruby: Net::HTTP.get(URI(url))
来源：http://bnw.hnqzz.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fzq.zhengqikj.top

[L02] 发送 POST JSON
来源：http://vfa.snrcjt.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qte.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wjs.hysaishi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uqc.yanxiufei.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://csx.hongshengwenyu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ebb.yongpay.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fop.zhengqikj.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mmo.feifeiyinyue.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jcu.nanxuanxn.top

[L03] 设置自定义请求头
来源：http://ydl.cucudq.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ywz.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ryv.jianghu66.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nef.hywenlv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ayg.zhengqikj.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rvn.xingfuxueyuan.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bsv.snrcjt.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vjj.shuidangran.top


<!-- 参考信息 -->