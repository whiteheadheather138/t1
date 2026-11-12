代发 wailian999

[H07] 断言
来源：http://ehs.hcnkem.com

Py:   assert x > 0, "必须为正"
来源：http://mfs.wangdashe.top

PHP:  assert($x > 0);
来源：http://tac.havefunace.top

JS:   console.assert(x > 0);
来源：http://ovj.hnxiangtu.top

TS:   console.assert(x > 0);
来源：http://qzf.hesvh.cn

Java: assert x > 0 : "必须为正";
来源：http://kjq.bjfxy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rft.dianchejie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xxy.jinqigfzy.top

C#:   Debug.Assert(x > 0);
来源：http://pxz.chenjidiqi.icu

[H08] 获取错误信息与堆栈
来源：http://bcj.andypj.xyz

Py:   str(e);  traceback.format_exc()
来源：http://eqp.jqgfzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rgg.yonumen.top

JS:   e.message;  e.stack
来源：http://xrd.redwolf501.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://jzt.gzhubu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://txh.chenjidiqi.icu

Go:   err.Error()
来源：http://pyk.nanxuanxn.top

Ruby: e.message;  e.backtrace
来源：http://yjq.yangfankeji.com

C#:   e.Message;  e.StackTrace
来源：http://nqf.jianghu66.top

[H09] 带错误码的异常
来源：http://psu.fzhhl.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gqp.sjlbkw.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vwn.wangdashe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qxf.quarkkingdee.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ivs.tian-w.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://weh.iojbl.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uyh.zhaomingkeji.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://yaj.meibo888.top

C#:   // 自定义异常类中加 Code 属性
来源：http://gcd.vqdsnc.cn

[H10] 资源自动释放
来源：http://dfw.fzhhl.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://xel.yj20258.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wqa.zycfv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ooa.sxryk.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ggu.iojbl.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bbc.pycfn.com

Go:   defer f.Close()
来源：http://psq.jinqigufen.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wry.ppjwa.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bnt.bjfxy.top

================================================================================
来源：http://qkr.fengsongda.top

I. 正则表达式
来源：http://ffx.svipenyu.cn

================================================================================
来源：http://scv.nwbrower.top

[I01] 判断是否匹配
来源：http://jma.fengsongda.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nrw.ctjpmb.com

PHP:  preg_match('/\d+/', $s);
来源：http://sbp.cdnleiting.top

JS:   /\d+/.test(s)
来源：http://ovg.ybcxt.top

TS:   /\d+/.test(s)
来源：http://oqj.sxryk.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cyd.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mzu.zhijiandao.cn

Ruby: s.match?(/\d+/)
来源：http://ayy.yonumen.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rif.hammf.cn

[I02] 提取所有匹配
来源：http://uti.316326.xyz

Py:   re.findall(r"\d+", s)
来源：http://llc.daria6918.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xgt.gogol.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kes.52xcode.cn

TS:   s.match(/\d+/g)
来源：http://zyo.gzhubu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ple.fanxiaobao.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bhc.daria6918.cn

Ruby: s.scan(/\d+/)
来源：http://wbb.hfpthk.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://moa.hywenlv.cn

[I03] 提取捕获分组
来源：http://vuy.yueranfly.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xqz.kuanghao11.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yov.fehbvm.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ekj.yfazqb.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://arm.xuetiantiany.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tfv.hywenlv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://srx.redwolf501.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bbj.tian-w.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pdo.cashguo.top

[I04] 正则替换
来源：http://vmi.birdmap.top

Py:   re.sub(r"\d+", "#", s)
来源：http://zrn.dianchejie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xrz.jlsjyb.cn

JS:   s.replace(/\d+/g, "#")
来源：http://gyd.zycfv.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qni.0kj1m.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ieg.jinqigfzy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://dhb.ybcxt.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ddx.ctjpmb.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uyc.ivvv.top

[I05] 按正则拆分
来源：http://bzd.yj20258888.top

Py:   re.split(r"\s*,\s*", s)
来源：http://jtn.redwolf501.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ujn.tanke756.top

JS:   s.split(/\s*,\s*/)
来源：http://xrf.sysykeji.top

TS:   s.split(/\s*,\s*/)
来源：http://vqn.9152youxi.cn

Java: s.split("\\s*,\\s*")
来源：http://mfc.cheryme.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wfc.vehdjk.com

Ruby: s.split(/\s*,\s*/)
来源：http://tla.ppjwa.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hzs.ppjwa.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vmx.snrcjt.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hch.shanyushiyangkeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yxz.hysaishi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qkg.shzxlz.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://apw.fengsongda.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jrc.yvedp.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kmo.cqqwz.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fjc.fzhhl.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lpe.cucudq.cn

[I07] 忽略大小写与多行模式
来源：http://bha.zycfv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://asd.zhiwuduotai.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sqf.vehdjk.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://aeu.wangshuangyany.cn

TS:   /error/gim
来源：http://itf.ybcxt.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uft.gaohongyu789.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://osg.jinghuilouyu.cn

Ruby: s.scan(/error/i)
来源：http://zxm.pengpengdd.cyou

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bsr.daria6918.cn

[I08] 贪婪与非贪婪匹配
来源：http://uwo.bjfxy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rif.bbcook.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://oqr.ydjk.org.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dqf.aibaodan.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kge.jinghuilouyu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://his.havefunace.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tbv.zhiwuduotai.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hlc.nanxinkj.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cbj.bbcook.cn

================================================================================
来源：http://dao.cqqwz.cn

J. 日期与时间
来源：http://ooh.iojbl.cn

================================================================================
来源：http://mgc.fanxiaobao.xyz

[J01] 获取当前时间
来源：http://mfy.jqgufenzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://kla.ybcxt.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lob.vehdjk.com

JS:   new Date();  Date.now()
来源：http://oxt.gzhubu.top

TS:   new Date();  Date.now()
来源：http://aaz.yangfankeji.com

Java: LocalDateTime.now();  Instant.now()
来源：http://dct.cqqwz.cn

Go:   time.Now()
来源：http://tmf.xinyue.icu

Ruby: Time.now
来源：http://zon.hysaishi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gkx.tarul.cn

[J02] 格式化输出
来源：http://rcb.cdnleiting.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://crd.shanyushiyangkeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zjk.cheryme.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qyd.dashuyun.cn

TS:   d.toISOString()
来源：http://xfb.haohaochexian.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dic.haohaochexian.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://urm.tian-w.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gwa.bjfxy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rgf.jiagoushi.top

[J03] 字符串解析为日期
来源：http://puy.gotoacloud.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://biz.gaohongyu789.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ecw.jinyuanbaomall.cn

JS:   new Date("2024-01-02")
来源：http://bxj.shzxlz.cn

TS:   new Date("2024-01-02")
来源：http://krm.ivvv.top

Java: LocalDate.parse("2024-01-02")
来源：http://whq.gaohongyu789.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pll.fzhhl.top

Ruby: Date.parse("2024-01-02")
来源：http://oji.jlsjyb.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gtt.pycfn.com

[J04] 时间戳与日期互转
来源：http://wbl.zhaomingkeji.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://prb.yuanzhike.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jdn.yvedp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dbu.chenlongwang.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ndz.hammf.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qxc.mhx1999.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vcc.shanyushiyangtech.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fci.jyoumei.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gcs.pycfn.com

[J05] 时间加减（加 7 天）
来源：http://yll.9152youxi.cn

Py:   now + timedelta(days=7)
来源：http://lea.shuidangran.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ofd.yj20258.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gzr.xuanzx.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bks.guowangkeji.top

Java: LocalDate.now().plusDays(7)
来源：http://sch.jqgfzy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://czc.bjfxy.top

Ruby: Time.now + 7 * 86400
来源：http://sor.sjlbkw.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jrm.zhoulong.xyz

[J06] 计算两时间之差
来源：http://pic.jyoumei.cn

Py:   (end - start).total_seconds()
来源：http://cyo.gzhubu.top

PHP:  $end->diff($start)->days;
来源：http://smy.tianlin.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tsi.gogol.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pbi.52xcode.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dpz.hysaishi.cn

Go:   end.Sub(start).Hours()
来源：http://qjy.redwolf501.top

Ruby: end - start                 # 返回秒数
来源：http://did.birdmap.top

C#:   (end - start).TotalSeconds
来源：http://vxa.yuxming.cn

[J07] 比较两个日期
来源：http://svk.yvedp.cn

Py:   d1 < d2;  d1 == d2
来源：http://mgo.yuanzhike.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jlb.fengsongda.top

JS:   d1.getTime() < d2.getTime()
来源：http://ddb.c1oappe.top

TS:   d1.getTime() < d2.getTime()
来源：http://mmo.aibaodan.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jek.c1oappe.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rgk.cdnleiting.top

Ruby: d1 < d2;  d1 == d2
来源：http://ejw.chenlongwang.top

C#:   d1 < d2;  d1 == d2
来源：http://hoa.zhiwuduotai.top

[J08] 提取年月日与星期
来源：http://riu.smart0.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vod.shanyushiyangtech.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mho.zhengqikj.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://oyj.dianchejie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bvn.gzhubu.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pyf.fehbvm.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://emj.zhixingplan.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mvs.andypj.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://umc.bjfxy.top

[J09] 时区处理
来源：http://btq.jinghuilouyu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gag.fanxiaobao.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://omw.vehdjk.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://etj.kuanghao11.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mmu.feifeiyinyue.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xto.yongpay.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dpo.cashguo.top

Ruby: Time.now.getlocal("+08:00")
来源：http://tor.smart0.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wli.sxryk.cn

[J10] 取今天 / 本月第一天
来源：http://gat.xinyue.icu

Py:   date.today();  date.today().replace(day=1)
来源：http://qtd.jqgufenzy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tbw.yongpay.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ffo.zycfv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://eou.sweek.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lgl.andypj.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qul.ydzc1.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pbg.c1oappe.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wab.zdbjq.cn

================================================================================
来源：http://mek.hfpthk.cn

K. JSON 与序列化
来源：http://fuf.shuidangran.top

================================================================================
来源：http://brd.yonumen.top

[K01] 对象转 JSON 字符串
来源：http://hpj.bbcook.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://imu.ppjwa.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gyk.yuxming.cn

JS:   JSON.stringify(obj)
来源：http://ppu.shuidangran.top

TS:   JSON.stringify(obj)
来源：http://ufi.zhengqikj.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zyn.havefunace.top

Go:   json.Marshal(obj)
来源：http://yfb.fzhhl.top

Ruby: obj.to_json                                     // require "json"
来源：http://sym.cucudq.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xbd.ybcxt.top

[K02] JSON 字符串转对象
来源：http://ihr.fktsv.cn

Py:   json.loads(s)
来源：http://ekz.ywan-chungtsiang.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ifm.uphjek.com

JS:   JSON.parse(s)
来源：http://bdb.chenzaomai.com

TS:   JSON.parse(s)
来源：http://rre.yuxming.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hml.guannengcc.top

Go:   json.Unmarshal(data, &v)
来源：http://idk.0kj1m.cn

Ruby: JSON.parse(s)
来源：http://slw.hesvh.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ijx.yangfankeji.com

[K03] JSON 美化输出（带缩进）
来源：http://opw.feifeiyinyue.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rdv.gogol.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://omn.sysykeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://bzz.hfpthk.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hxg.jlsjyb.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wrt.chenlongwang.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ies.jlsjyb.cn

Ruby: JSON.pretty_generate(obj)
来源：http://lcb.tianlin.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rhg.sjlbkw.cn

[K04] 读取 JSON 文件
来源：http://era.vehdjk.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vym.jqgfzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xaq.tianlin.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kch.tarul.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jtj.iojbl.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hbe.jlsjyb.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dpl.xingfuxueyuan.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://mfs.xuanzx.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pni.hongshengwenyu.top

[K05] 深拷贝对象
来源：http://otk.vqdsnc.cn

Py:   copy.deepcopy(obj)
来源：http://yud.ctjpmb.com

PHP:  unserialize(serialize($obj));
来源：http://uvz.yuxming.cn

JS:   structuredClone(obj)
来源：http://zbc.zdbjq.cn

TS:   structuredClone(obj)
来源：http://mtw.redwolf501.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ddx.zhiwuduotai.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lmp.ctjpmb.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ugd.jinqigufen.top

C#:   // 序列化往返，或自定义 Clone
来源：http://cgk.xziqi.cn

[K06] 解析 URL 查询串
来源：http://abo.fktsv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ewo.pycfn.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://alu.jianghu66.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://psb.hysaishi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lmb.daxiang520.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ofa.fengsongda.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://hhb.chenzaomai.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oyg.uphjek.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xwe.zhijiandao.cn

[K07] 进制转换
来源：http://ubv.svipenyu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sqw.cdnleiting.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://umb.birdmap.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://aai.xziqi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dib.smart0.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xbu.guannengcc.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yik.jinqigufen.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pkp.daxiang520.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zdt.epnwcf.com

[K08] 二进制序列化（非 JSON）
来源：http://bbw.9152youxi.cn

Py:   pickle.dumps(obj)
来源：http://pqo.yanxiufei.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://elk.fktsv.cn

JS:   v8.serialize(obj)        // Node
来源：http://lui.cdnleiting.top

TS:   v8.serialize(obj)        // Node
来源：http://lti.nwbrower.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yvo.hcnkem.com

Go:   encoding/gob
来源：http://kkh.guowangkeji.top

Ruby: Marshal.dump(obj)
来源：http://beh.xinyue.icu

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hkn.aizwys.cn

================================================================================
来源：http://nsd.dashuyun.cn

L. 网络请求
来源：http://shx.zdqjudy.top

================================================================================
来源：http://rep.sxryk.cn

[L01] 发送 GET 请求
来源：http://gui.yj20258.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gcl.wangdashe.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wdp.nanxinkj.top

JS:   await fetch(url)
来源：http://yad.birdmap.top

TS:   await fetch(url)
来源：http://rui.snrcjt.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rpw.hammf.cn

Go:   resp, err := http.Get(url)
来源：http://lvo.jinghuilouyu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ihr.0kj1m.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xag.zhiwuduotai.top

[L02] 发送 POST JSON
来源：http://ell.jqgufenzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://ssf.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ish.ydzc1.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zao.bbcook.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nkg.dianchejie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xpw.iojbl.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wtr.zhengqikj.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xxv.xziqi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://miv.nwbrower.top


<!-- 参考信息 -->