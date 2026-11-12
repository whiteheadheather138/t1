代发 wailian999

[H07] 断言
来源：http://euy.kuanghao11.cn

Py:   assert x > 0, "必须为正"
来源：http://ofn.zycfv.cn

PHP:  assert($x > 0);
来源：http://nwj.fehbvm.com

JS:   console.assert(x > 0);
来源：http://jjk.ydzc1.top

TS:   console.assert(x > 0);
来源：http://flz.ybcxt.top

Java: assert x > 0 : "必须为正";
来源：http://amx.xylfe.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dwq.nanxuanxn.top

Ruby: raise "必须为正" unless x > 0
来源：http://meo.zycfv.cn

C#:   Debug.Assert(x > 0);
来源：http://nwn.dianchejie.cn

[H08] 获取错误信息与堆栈
来源：http://ysn.chenjidiqi.icu

Py:   str(e);  traceback.format_exc()
来源：http://xfx.ydjk.org.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bfn.zhengqikj.top

JS:   e.message;  e.stack
来源：http://wip.jqgufenzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://bwl.cdnleiting.top

Java: e.getMessage();  e.printStackTrace()
来源：http://wiz.jqgfzy.top

Go:   err.Error()
来源：http://wsc.xingfuxueyuan.xyz

Ruby: e.message;  e.backtrace
来源：http://glt.cheryme.top

C#:   e.Message;  e.StackTrace
来源：http://bou.gogol.net.cn

[H09] 带错误码的异常
来源：http://bui.yuanzhike.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://aps.uphjek.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://lef.nwbrower.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bks.zhixingplan.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://uiv.52xcode.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jxu.yangfankeji.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zqa.c1oappe.top

Ruby: raise MyError.new("fail", 500)
来源：http://mhy.gogol.net.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qoi.sufxvd.cn

[H10] 资源自动释放
来源：http://pez.jlsjyb.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://slb.jinghuilouyu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tuc.316326.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lud.yfazqb.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ulb.jiagoushi.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vzm.haohaochexian.top

Go:   defer f.Close()
来源：http://etl.sufxvd.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vow.jinghuilouyu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xcn.pengpengdd.cyou

================================================================================
来源：http://wrn.fktsv.cn

I. 正则表达式
来源：http://tor.iojbl.cn

================================================================================
来源：http://ail.yvedp.cn

[I01] 判断是否匹配
来源：http://lhc.yj20258.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pgr.shzxlz.cn

PHP:  preg_match('/\d+/', $s);
来源：http://kke.fengsongda.top

JS:   /\d+/.test(s)
来源：http://oiq.xingfuxueyuan.xyz

TS:   /\d+/.test(s)
来源：http://jfn.jinyuanbaomall.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pxp.smart0.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pur.shuidangran.top

Ruby: s.match?(/\d+/)
来源：http://glw.tanke756.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://esk.shangyingyoupin.top

[I02] 提取所有匹配
来源：http://nwc.jiagoushi.top

Py:   re.findall(r"\d+", s)
来源：http://hka.zhengqikj.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uwi.yongpay.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zik.svipenyu.cn

TS:   s.match(/\d+/g)
来源：http://zqp.shanyushiyangtech.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dle.yj20258888.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uqc.vqdsnc.cn

Ruby: s.scan(/\d+/)
来源：http://jfa.snrcjt.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qqa.fengsongda.top

[I03] 提取捕获分组
来源：http://loy.xziqi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://spj.kuanghao11.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bai.xingfuxueyuan.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bmy.sweek.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://axt.zdqjudy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jlr.ydjk.org.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jqf.haohaochexian.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dug.xylfe.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gou.daxiang520.top

[I04] 正则替换
来源：http://zva.yj202588.top

Py:   re.sub(r"\d+", "#", s)
来源：http://izf.ydzc1.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ysu.zycfv.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mwo.jianghu66.top

TS:   s.replace(/\d+/g, "#")
来源：http://mja.xziqi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hes.9152youxi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://cza.gzhubu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://lgr.hnqzz.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://avf.kuanghao11.cn

[I05] 按正则拆分
来源：http://jwv.shzxlz.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://keb.zdbjq.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://squ.52xcode.cn

JS:   s.split(/\s*,\s*/)
来源：http://moq.ydzc1.top

TS:   s.split(/\s*,\s*/)
来源：http://xhu.zhaomingkeji.xyz

Java: s.split("\\s*,\\s*")
来源：http://wwl.epnwcf.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lku.sufxvd.cn

Ruby: s.split(/\s*,\s*/)
来源：http://neq.hysaishi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tvx.ehwqpu.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gpr.jlsjyb.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pxe.shuidangran.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zze.yj202588.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ivf.nanxinkj.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://riy.ppjwa.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://iwy.bjfxy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://aje.hongshengwenyu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gct.hnxiangtu.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gof.jlsjyb.cn

[I07] 忽略大小写与多行模式
来源：http://gsm.nanxuanxn.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gki.sysykeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bde.cqqwz.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://edy.ivvv.top

TS:   /error/gim
来源：http://mnx.shuidangran.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nuu.yuanzhike.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://beg.shzxlz.cn

Ruby: s.scan(/error/i)
来源：http://ugw.c1oappe.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jhj.cdnleiting.top

[I08] 贪婪与非贪婪匹配
来源：http://lmi.hnxiangtu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bsd.ctjpmb.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bsd.hywenlv.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zlt.cashguo.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vhi.wangdashe.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ddw.gotoacloud.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zpy.hysaishi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bui.ivvv.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hca.bbcook.cn

================================================================================
来源：http://gpr.hfpthk.cn

J. 日期与时间
来源：http://kdx.ehwqpu.com

================================================================================
来源：http://ggc.shzxlz.cn

[J01] 获取当前时间
来源：http://dbe.shanyushiyangkeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://edg.9152youxi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bmf.fanxiaobao.xyz

JS:   new Date();  Date.now()
来源：http://sou.hnqzz.top

TS:   new Date();  Date.now()
来源：http://jyh.shangyingyoupin.top

Java: LocalDateTime.now();  Instant.now()
来源：http://kll.haohaochexian.top

Go:   time.Now()
来源：http://vss.chenlongwang.top

Ruby: Time.now
来源：http://cdk.yuxming.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xbe.pycfn.com

[J02] 格式化输出
来源：http://pap.xuanzx.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uau.zhaomingkeji.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gcu.shzxlz.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lrf.fehbvm.com

TS:   d.toISOString()
来源：http://bbm.guannengcc.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zkv.aizwys.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fbj.gzhubu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hxa.fengsongda.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lok.jqgfzy.top

[J03] 字符串解析为日期
来源：http://gyv.cucudq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://frf.jinyuanbaomall.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://szi.andypj.xyz

JS:   new Date("2024-01-02")
来源：http://uzf.52xcode.cn

TS:   new Date("2024-01-02")
来源：http://dih.9152youxi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xxf.tarul.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kjr.aizwys.cn

Ruby: Date.parse("2024-01-02")
来源：http://mpe.ppjwa.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lkr.yongpay.top

[J04] 时间戳与日期互转
来源：http://ghb.havefunace.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://trz.yongpay.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://esu.sweek.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nnf.vehdjk.com

TS:   Math.floor(Date.now() / 1000)
来源：http://dyk.wangshuangyany.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lme.feifeiyinyue.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rwu.hysaishi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pkd.ywan-chungtsiang.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://duu.sysykeji.top

[J05] 时间加减（加 7 天）
来源：http://yuf.svipenyu.cn

Py:   now + timedelta(days=7)
来源：http://qea.cucudq.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rsa.kuanghao11.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cjg.nanxuanxn.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bkz.sufxvd.cn

Java: LocalDate.now().plusDays(7)
来源：http://euk.hysaishi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ile.ppjwa.cn

Ruby: Time.now + 7 * 86400
来源：http://ylj.yongpay.top

C#:   DateTime.Now.AddDays(7)
来源：http://pdg.xuetiantiany.cn

[J06] 计算两时间之差
来源：http://qtp.ehwqpu.com

Py:   (end - start).total_seconds()
来源：http://ijn.zdbjq.cn

PHP:  $end->diff($start)->days;
来源：http://yyy.shzxlz.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ldz.zhaomingkeji.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://trx.hammf.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dnh.sxryk.cn

Go:   end.Sub(start).Hours()
来源：http://yhh.yj202588.top

Ruby: end - start                 # 返回秒数
来源：http://fok.uphjek.com

C#:   (end - start).TotalSeconds
来源：http://uol.hnxiangtu.top

[J07] 比较两个日期
来源：http://tod.birdmap.top

Py:   d1 < d2;  d1 == d2
来源：http://xun.xuanzx.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fkm.yuanzhike.top

JS:   d1.getTime() < d2.getTime()
来源：http://iel.uphjek.com

TS:   d1.getTime() < d2.getTime()
来源：http://mmu.bbcook.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hhg.jqgfzy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vnw.gotoacloud.top

Ruby: d1 < d2;  d1 == d2
来源：http://awy.sweek.top

C#:   d1 < d2;  d1 == d2
来源：http://ptg.cheryme.top

[J08] 提取年月日与星期
来源：http://txx.svipenyu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hgq.haohaochexian.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ajm.9152youxi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bed.andypj.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vrl.xinyue.icu

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://loi.cdnleiting.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vje.zhoulong.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rsu.cheryme.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hip.havefunace.top

[J09] 时区处理
来源：http://dad.fengsongda.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sik.fanxiaobao.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xuc.vehdjk.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://apt.52xcode.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cvy.tarul.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://joo.cucudq.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nms.yongpay.top

Ruby: Time.now.getlocal("+08:00")
来源：http://abv.zhongyouzk.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zuh.andypj.xyz

[J10] 取今天 / 本月第一天
来源：http://hqi.yuanzhike.top

Py:   date.today();  date.today().replace(day=1)
来源：http://mfo.smart0.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pyg.yanxiufei.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://int.ybcxt.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mek.wangdashe.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ilt.hnqzz.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wwi.jinyuanbaomall.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fpq.yvedp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bum.nanxinkj.top

================================================================================
来源：http://wla.pengpengdd.cyou

K. JSON 与序列化
来源：http://zqk.cheryme.top

================================================================================
来源：http://mon.shuidangran.top

[K01] 对象转 JSON 字符串
来源：http://wpg.meibo888.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jvv.shanyushiyangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fex.pengpengdd.cyou

JS:   JSON.stringify(obj)
来源：http://rqo.hysaishi.cn

TS:   JSON.stringify(obj)
来源：http://ljz.hongshengwenyu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zsb.cheryme.top

Go:   json.Marshal(obj)
来源：http://ord.tarul.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xkx.zhoulong.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://jwo.ivvv.top

[K02] JSON 字符串转对象
来源：http://bpr.svipenyu.cn

Py:   json.loads(s)
来源：http://ksc.wangshuangyany.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://udy.guannengcc.top

JS:   JSON.parse(s)
来源：http://fem.yj202588.top

TS:   JSON.parse(s)
来源：http://zvd.yuxming.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jjp.daria6918.cn

Go:   json.Unmarshal(data, &v)
来源：http://mwc.fengsongda.top

Ruby: JSON.parse(s)
来源：http://awh.andypj.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fjc.zhixingplan.top

[K03] JSON 美化输出（带缩进）
来源：http://gtt.uphjek.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pyf.ywan-chungtsiang.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sot.yongpay.top

JS:   JSON.stringify(obj, null, 2)
来源：http://hff.jlsjyb.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://goj.dashuyun.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ylf.yanxiufei.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ahk.0kj1m.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pcf.fengsongda.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tbj.jiagoushi.top

[K04] 读取 JSON 文件
来源：http://jex.9152youxi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pej.316326.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ppx.zhixingplan.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://imj.hysaishi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oft.ybcxt.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://coy.hfpthk.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pes.shanyushiyangtech.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://mwd.havefunace.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wvl.gogol.net.cn

[K05] 深拷贝对象
来源：http://ptl.cqqwz.cn

Py:   copy.deepcopy(obj)
来源：http://vbf.shuidangran.top

PHP:  unserialize(serialize($obj));
来源：http://vgo.nwbrower.top

JS:   structuredClone(obj)
来源：http://acu.redwolf501.top

TS:   structuredClone(obj)
来源：http://tfr.zhaomingkeji.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://jfe.jiagoushi.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hqi.ydzc1.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nsm.xinyue.icu

C#:   // 序列化往返，或自定义 Clone
来源：http://jpv.cashguo.top

[K06] 解析 URL 查询串
来源：http://aqc.cheryme.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zit.daria6918.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lng.kuanghao11.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yfj.yj20258888.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mef.kuanghao11.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lgb.hcnkem.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://snq.hongshengwenyu.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vgz.nanxuanxn.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ugd.hcnkem.com

[K07] 进制转换
来源：http://ail.jqgufenzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://meu.shangyingyoupin.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cip.ctjpmb.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://eyi.svipenyu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://trl.aibaodan.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pvw.nanxinkj.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pop.jinyuanbaomall.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ygx.zhiwuduotai.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fgo.snrcjt.cn

[K08] 二进制序列化（非 JSON）
来源：http://fgo.nwbrower.top

Py:   pickle.dumps(obj)
来源：http://lyu.fzhhl.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qra.zhijiandao.cn

JS:   v8.serialize(obj)        // Node
来源：http://wxd.jqgfzy.top

TS:   v8.serialize(obj)        // Node
来源：http://oog.pycfn.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://irw.guannengcc.top

Go:   encoding/gob
来源：http://vos.vehdjk.com

Ruby: Marshal.dump(obj)
来源：http://hir.smart0.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gwz.zhiwuduotai.top

================================================================================
来源：http://emo.zycfv.cn

L. 网络请求
来源：http://mbu.jinqigfzy.top

================================================================================
来源：http://mkd.ivvv.top

[L01] 发送 GET 请求
来源：http://ijy.nanxuanxn.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://avz.sjlbkw.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dqz.yfazqb.com

JS:   await fetch(url)
来源：http://jdc.sysykeji.top

TS:   await fetch(url)
来源：http://ivz.vqdsnc.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://aij.bbcook.cn

Go:   resp, err := http.Get(url)
来源：http://ydt.andypj.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://kef.feifeiyinyue.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mdy.hesvh.cn

[L02] 发送 POST JSON
来源：http://qnz.cucudq.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mmb.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zef.haohaochexian.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zcr.jiagoushi.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aus.sweek.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zug.cashguo.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ooe.nanxuanxn.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fwz.zhijiandao.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://otr.jqgfzy.top


<!-- 参考信息 -->