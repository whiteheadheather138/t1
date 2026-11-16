代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://ziv.ydjk.org.cn

[H08] 获取错误信息与堆栈
来源：http://mxn.hywenlv.cn

Py:   str(e);  traceback.format_exc()
来源：http://zbg.gogol.net.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://raz.cdnleiting.top

JS:   e.message;  e.stack
来源：http://kjx.sxryk.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xka.tarul.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://iiu.cucudq.cn

Go:   err.Error()
来源：http://dvc.uphjek.com

Ruby: e.message;  e.backtrace
来源：http://aai.fanxiaobao.xyz

C#:   e.Message;  e.StackTrace
来源：http://nyr.dianchejie.cn

[H09] 带错误码的异常
来源：http://hdd.gzhubu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dic.birdmap.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://aot.ybcxt.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mrb.xingfuxueyuan.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ynz.chenlongwang.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fuw.sysykeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gzt.gzhubu.top

Ruby: raise MyError.new("fail", 500)
来源：http://end.gaohongyu789.top

C#:   // 自定义异常类中加 Code 属性
来源：http://jav.redwolf501.top

[H10] 资源自动释放
来源：http://ztt.snrcjt.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ngc.jiagoushi.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rsr.yanxiufei.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://eun.cheryme.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zcv.jinghuilouyu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uyh.hysaishi.cn

Go:   defer f.Close()
来源：http://kxy.sweek.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ose.smart0.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://elu.hnqzz.top

================================================================================
来源：http://whb.ywan-chungtsiang.top

I. 正则表达式
来源：http://hcs.cashguo.top

================================================================================
来源：http://ibn.hammf.cn

[I01] 判断是否匹配
来源：http://tkr.yj202588.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cmo.ydzc1.top

PHP:  preg_match('/\d+/', $s);
来源：http://bau.birdmap.top

JS:   /\d+/.test(s)
来源：http://hgx.xylfe.cn

TS:   /\d+/.test(s)
来源：http://mdz.aizwys.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dme.ctjpmb.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xvz.daxiang520.top

Ruby: s.match?(/\d+/)
来源：http://zcw.yuanzhike.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bbr.pycfn.com

[I02] 提取所有匹配
来源：http://tpo.zdqjudy.top

Py:   re.findall(r"\d+", s)
来源：http://utf.chenzaomai.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tab.yonumen.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bvb.zycfv.cn

TS:   s.match(/\d+/g)
来源：http://rdl.hammf.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qhx.fktsv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yzw.yj20258.top

Ruby: s.scan(/\d+/)
来源：http://hxa.jlsjyb.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ilr.epnwcf.com

[I03] 提取捕获分组
来源：http://tuc.zhijiandao.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fge.xuanzx.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ayb.birdmap.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hsk.xuetiantiany.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ffu.zhijiandao.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ysg.hesvh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jcq.jqgufenzy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mdx.xingfuxueyuan.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gdg.gaohongyu789.top

[I04] 正则替换
来源：http://qlh.yongpay.top

Py:   re.sub(r"\d+", "#", s)
来源：http://xze.shanyushiyangtech.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vcy.xingfuxueyuan.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://buf.sxryk.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xhi.xziqi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bzh.316326.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://ttq.xingfuxueyuan.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://cky.birdmap.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qxu.cheryme.top

[I05] 按正则拆分
来源：http://nyf.nwbrower.top

Py:   re.split(r"\s*,\s*", s)
来源：http://rma.xylfe.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://npk.svipenyu.cn

JS:   s.split(/\s*,\s*/)
来源：http://yma.jinghuilouyu.cn

TS:   s.split(/\s*,\s*/)
来源：http://nsc.zdqjudy.top

Java: s.split("\\s*,\\s*")
来源：http://sua.zhiwuduotai.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://owp.gotoacloud.top

Ruby: s.split(/\s*,\s*/)
来源：http://tlq.nwbrower.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ndk.xuetiantiany.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://szt.chenlongwang.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gpt.svipenyu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gtp.shanyushiyangtech.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://buc.bbcook.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lxq.jqgufenzy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uuc.tianlin.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://eus.chenjidiqi.icu

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uld.nwbrower.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ftk.yueranfly.top

[I07] 忽略大小写与多行模式
来源：http://nju.zhixingplan.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fta.nanxinkj.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dzb.wangdashe.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://biv.sweek.top

TS:   /error/gim
来源：http://rko.meibo888.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dvn.ctjpmb.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vgh.guowangkeji.top

Ruby: s.scan(/error/i)
来源：http://fdm.dashuyun.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tqa.yfazqb.com

[I08] 贪婪与非贪婪匹配
来源：http://hyr.cdnleiting.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://crb.cucudq.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cct.yfazqb.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kuu.hcnkem.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qma.yonumen.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ipl.zhixingplan.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ovc.shzxlz.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gvj.xuetiantiany.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wcg.tianlin.xyz

================================================================================
来源：http://sro.hesvh.cn

J. 日期与时间
来源：http://rya.cashguo.top

================================================================================
来源：http://tyy.meibo888.top

[J01] 获取当前时间
来源：http://euy.xziqi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://paw.yvedp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ehe.redwolf501.top

JS:   new Date();  Date.now()
来源：http://wdi.hysaishi.cn

TS:   new Date();  Date.now()
来源：http://fsv.wangdashe.top

Java: LocalDateTime.now();  Instant.now()
来源：http://trn.yj20258.top

Go:   time.Now()
来源：http://heo.mhx1999.top

Ruby: Time.now
来源：http://pvp.gzhubu.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qaj.zdbjq.cn

[J02] 格式化输出
来源：http://xmz.zdbjq.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jfi.cucudq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yrd.jinyuanbaomall.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bnw.yfazqb.com

TS:   d.toISOString()
来源：http://ybu.aizwys.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ifx.shanyushiyangtech.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xyg.jinqigufen.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fjh.hnxiangtu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lat.yfazqb.com

[J03] 字符串解析为日期
来源：http://spj.cqqwz.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wmb.shuidangran.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wwu.shanyushiyangkeji.top

JS:   new Date("2024-01-02")
来源：http://sii.ydzc1.top

TS:   new Date("2024-01-02")
来源：http://ahr.sweek.top

Java: LocalDate.parse("2024-01-02")
来源：http://vpc.fanxiaobao.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://faq.birdmap.top

Ruby: Date.parse("2024-01-02")
来源：http://wea.dianchejie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://suq.sysykeji.top

[J04] 时间戳与日期互转
来源：http://pml.cqqwz.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://veh.daria6918.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://buv.epnwcf.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sdz.svipenyu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://sno.tarul.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pyv.shuidangran.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xsc.chenzaomai.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lgs.yj20258888.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fby.tanke756.top

[J05] 时间加减（加 7 天）
来源：http://vzu.gaohongyu789.top

Py:   now + timedelta(days=7)
来源：http://oge.zhiwuduotai.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://xte.ctjpmb.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wme.yanxiufei.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wej.havefunace.top

Java: LocalDate.now().plusDays(7)
来源：http://bvo.yangfankeji.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ygq.yfazqb.com

Ruby: Time.now + 7 * 86400
来源：http://pno.hammf.cn

C#:   DateTime.Now.AddDays(7)
来源：http://iad.ehwqpu.com

[J06] 计算两时间之差
来源：http://hjv.nanxuanxn.top

Py:   (end - start).total_seconds()
来源：http://fgd.jyoumei.cn

PHP:  $end->diff($start)->days;
来源：http://por.guannengcc.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ina.zhixingplan.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://juu.svipenyu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bos.epnwcf.com

Go:   end.Sub(start).Hours()
来源：http://dsy.yanxiufei.cn

Ruby: end - start                 # 返回秒数
来源：http://byh.jyoumei.cn

C#:   (end - start).TotalSeconds
来源：http://xgf.fzhhl.top

[J07] 比较两个日期
来源：http://pgx.yj20258888.top

Py:   d1 < d2;  d1 == d2
来源：http://qvi.guannengcc.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lnj.cqqwz.cn

JS:   d1.getTime() < d2.getTime()
来源：http://grx.jinqigufen.top

TS:   d1.getTime() < d2.getTime()
来源：http://ymy.hcnkem.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wvg.xinyue.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://roa.yuxming.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vzc.feifeiyinyue.top

C#:   d1 < d2;  d1 == d2
来源：http://aai.tian-w.cn

[J08] 提取年月日与星期
来源：http://kzs.epnwcf.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qlz.guowangkeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lzg.hfpthk.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bhq.ydzc1.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rlr.zhoulong.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bin.wangshuangyany.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rws.tarul.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wim.daxiang520.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://oxb.svipenyu.cn

[J09] 时区处理
来源：http://foo.vqdsnc.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ojz.haohaochexian.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bcq.yj20258888.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qcv.shanyushiyangkeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wrh.zhijiandao.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zot.jlsjyb.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hlo.guannengcc.top

Ruby: Time.now.getlocal("+08:00")
来源：http://omo.pengpengdd.cyou

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ona.gaohongyu789.top

[J10] 取今天 / 本月第一天
来源：http://uee.hcnkem.com

Py:   date.today();  date.today().replace(day=1)
来源：http://xil.guowangkeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://aos.gaohongyu789.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nlo.bbcook.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://skz.smart0.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rcs.sxryk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lsr.pengpengdd.cyou

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bto.xuetiantiany.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dke.yangfankeji.com

================================================================================
来源：http://ofh.fehbvm.com

K. JSON 与序列化
来源：http://azf.yonumen.top

================================================================================
来源：http://epi.hnxiangtu.top

[K01] 对象转 JSON 字符串
来源：http://cwy.zhengqikj.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://irk.fzhhl.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pzx.yj202588.top

JS:   JSON.stringify(obj)
来源：http://dqx.jqgufenzy.top

TS:   JSON.stringify(obj)
来源：http://pdy.52xcode.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dxj.meibo888.top

Go:   json.Marshal(obj)
来源：http://dbp.jinqigufen.top

Ruby: obj.to_json                                     // require "json"
来源：http://zgs.shzxlz.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jum.hnqzz.top

[K02] JSON 字符串转对象
来源：http://oxz.shzxlz.cn

Py:   json.loads(s)
来源：http://yfm.ywan-chungtsiang.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://esl.guannengcc.top

JS:   JSON.parse(s)
来源：http://qlz.sweek.top

TS:   JSON.parse(s)
来源：http://cmo.zycfv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dkf.haohaochexian.top

Go:   json.Unmarshal(data, &v)
来源：http://sxa.jlsjyb.cn

Ruby: JSON.parse(s)
来源：http://rqu.andypj.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mbs.xuetiantiany.cn

[K03] JSON 美化输出（带缩进）
来源：http://vsm.xinyue.icu

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kkf.fktsv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lus.bbcook.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://whe.zhoulong.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://pzt.yj20258.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oba.iojbl.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://odq.ivvv.top

Ruby: JSON.pretty_generate(obj)
来源：http://fbn.chenzaomai.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ytq.xylfe.cn

[K04] 读取 JSON 文件
来源：http://bbk.chenjidiqi.icu

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zri.hongshengwenyu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cts.zdbjq.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kvg.cucudq.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uot.aibaodan.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gxz.gzhubu.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fgt.316326.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://rzj.shanyushiyangkeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xdr.shuidangran.top

[K05] 深拷贝对象
来源：http://mmd.xziqi.cn

Py:   copy.deepcopy(obj)
来源：http://bea.bjfxy.top

PHP:  unserialize(serialize($obj));
来源：http://yru.cdnleiting.top

JS:   structuredClone(obj)
来源：http://war.yj20258888.top

TS:   structuredClone(obj)
来源：http://dmg.hysaishi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qsk.chenjidiqi.icu

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://riv.sysykeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jku.zdbjq.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ykf.dianchejie.cn

[K06] 解析 URL 查询串
来源：http://abs.yanxiufei.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ytv.epnwcf.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rqz.cashguo.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eho.hywenlv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://prr.zhaomingkeji.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://juv.wangshuangyany.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bln.chenzaomai.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qmd.yueranfly.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mjy.jyoumei.cn

[K07] 进制转换
来源：http://vxy.cashguo.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wos.ehwqpu.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jjt.c1oappe.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ysn.zhongyouzk.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zfc.yj202588.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ihr.snrcjt.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mml.jianghu66.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xfx.gaohongyu789.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zzp.xziqi.cn

[K08] 二进制序列化（非 JSON）
来源：http://sfk.chenzaomai.com

Py:   pickle.dumps(obj)
来源：http://gjk.smart0.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://byv.zdqjudy.top

JS:   v8.serialize(obj)        // Node
来源：http://ygb.aibaodan.cn

TS:   v8.serialize(obj)        // Node
来源：http://zns.dashuyun.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nxw.xuanzx.com

Go:   encoding/gob
来源：http://siq.zdqjudy.top

Ruby: Marshal.dump(obj)
来源：http://ykt.gaohongyu789.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xrb.gotoacloud.top

================================================================================
来源：http://gxg.cashguo.top

L. 网络请求
来源：http://zjm.xylfe.cn

================================================================================
来源：http://eof.nanxinkj.top

[L01] 发送 GET 请求
来源：http://dwl.jqgufenzy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tsw.ydzc1.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://afw.redwolf501.top

JS:   await fetch(url)
来源：http://dzh.quarkkingdee.top

TS:   await fetch(url)
来源：http://jmu.uphjek.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://eya.hcnkem.com

Go:   resp, err := http.Get(url)
来源：http://qxx.ctjpmb.com

Ruby: Net::HTTP.get(URI(url))
来源：http://xae.guowangkeji.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rtc.cqqwz.cn

[L02] 发送 POST JSON
来源：http://auj.nwbrower.top

Py:   requests.post(url, json={"a": 1})
来源：http://jmp.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ldp.yj202588.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dql.tianlin.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ebs.jqgfzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ovy.9152youxi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fmt.ehwqpu.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mfx.zhixingplan.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rpy.yuanzhike.top

[L03] 设置自定义请求头
来源：http://kva.zhongyouzk.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uhv.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rhj.yuxming.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zbw.ivvv.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yhv.shangyingyoupin.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cmf.cucudq.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lxf.yongpay.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://csc.mhx1999.top


<!-- 参考信息 -->