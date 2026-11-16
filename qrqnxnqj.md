代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://lcd.yueranfly.top

[H08] 获取错误信息与堆栈
来源：http://hlk.hysaishi.cn

Py:   str(e);  traceback.format_exc()
来源：http://khg.shzxlz.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tuz.hongshengwenyu.top

JS:   e.message;  e.stack
来源：http://xwf.ydzc1.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://svu.guowangkeji.top

Java: e.getMessage();  e.printStackTrace()
来源：http://olk.pycfn.com

Go:   err.Error()
来源：http://lro.vqdsnc.cn

Ruby: e.message;  e.backtrace
来源：http://jte.zhixingplan.top

C#:   e.Message;  e.StackTrace
来源：http://gvo.yj20258888.top

[H09] 带错误码的异常
来源：http://chf.zhiwuduotai.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://spz.vqdsnc.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zes.shanyushiyangkeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lou.ydjk.org.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bkb.yuanzhike.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pln.yueranfly.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hdj.yuxming.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wgo.jqgfzy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ldo.andypj.xyz

[H10] 资源自动释放
来源：http://uxp.quarkkingdee.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://lop.yj202588.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pte.tanke756.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sob.birdmap.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gyq.jinqigfzy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://meo.aibaodan.cn

Go:   defer f.Close()
来源：http://ygh.haohaochexian.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dch.ybcxt.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dub.xuanzx.com

================================================================================
来源：http://lzf.vehdjk.com

I. 正则表达式
来源：http://pic.yueranfly.top

================================================================================
来源：http://rmg.ppjwa.cn

[I01] 判断是否匹配
来源：http://svm.chenjidiqi.icu

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mtc.zycfv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://kpi.sufxvd.cn

JS:   /\d+/.test(s)
来源：http://uhe.gaohongyu789.top

TS:   /\d+/.test(s)
来源：http://bfr.cqqwz.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vnk.fktsv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gpr.quarkkingdee.top

Ruby: s.match?(/\d+/)
来源：http://cxu.fktsv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cwr.fzhhl.top

[I02] 提取所有匹配
来源：http://cuh.zhiwuduotai.top

Py:   re.findall(r"\d+", s)
来源：http://zkd.cdnleiting.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zhz.zdqjudy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://iue.zdqjudy.top

TS:   s.match(/\d+/g)
来源：http://wjb.uphjek.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fto.yj202588.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sfe.wangshuangyany.cn

Ruby: s.scan(/\d+/)
来源：http://mpo.hongshengwenyu.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mmu.kuanghao11.cn

[I03] 提取捕获分组
来源：http://anc.jlsjyb.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fas.tian-w.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xbc.yonumen.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dsh.haohaochexian.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rox.sufxvd.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jpd.hongshengwenyu.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://saq.epnwcf.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gnv.jinqigufen.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://oci.zhiwuduotai.top

[I04] 正则替换
来源：http://lnw.nwbrower.top

Py:   re.sub(r"\d+", "#", s)
来源：http://pnl.zhaomingkeji.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jos.daria6918.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dbv.jinqigfzy.top

TS:   s.replace(/\d+/g, "#")
来源：http://aew.uphjek.com

Java: s.replaceAll("\\d+", "#")
来源：http://pwn.uphjek.com

Go:   re.ReplaceAllString(s, "#")
来源：http://gss.zycfv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://eox.jinqigfzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jkf.wangshuangyany.cn

[I05] 按正则拆分
来源：http://tag.fktsv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dhd.nanxuanxn.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qwm.zhengqikj.top

JS:   s.split(/\s*,\s*/)
来源：http://vrw.hnqzz.top

TS:   s.split(/\s*,\s*/)
来源：http://jsk.xinyue.icu

Java: s.split("\\s*,\\s*")
来源：http://odw.tarul.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zel.hysaishi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jjw.guowangkeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zsm.redwolf501.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xzb.daria6918.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qle.epnwcf.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yoo.shangyingyoupin.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lnl.c1oappe.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qjr.xinyue.icu

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nha.chenzaomai.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cgl.dashuyun.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cgj.jqgfzy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mcn.bbcook.cn

[I07] 忽略大小写与多行模式
来源：http://qts.mhx1999.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rdc.snrcjt.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fre.cucudq.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dhg.aibaodan.cn

TS:   /error/gim
来源：http://mqh.cucudq.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zmj.fzhhl.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vkn.316326.xyz

Ruby: s.scan(/error/i)
来源：http://cyq.jinqigfzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ekp.fengsongda.top

[I08] 贪婪与非贪婪匹配
来源：http://fck.sxryk.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jgm.fanxiaobao.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xld.dianchejie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://val.cheryme.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xsr.redwolf501.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ajs.fanxiaobao.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wxe.hongshengwenyu.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mbt.ctjpmb.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://egn.guannengcc.top

================================================================================
来源：http://ekt.xinyue.icu

J. 日期与时间
来源：http://yhz.chenlongwang.top

================================================================================
来源：http://ors.yueranfly.top

[J01] 获取当前时间
来源：http://esa.hongshengwenyu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://wnp.cheryme.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://oio.jqgufenzy.top

JS:   new Date();  Date.now()
来源：http://bto.jinqigfzy.top

TS:   new Date();  Date.now()
来源：http://pnz.jiagoushi.top

Java: LocalDateTime.now();  Instant.now()
来源：http://sml.pengpengdd.cyou

Go:   time.Now()
来源：http://beg.tianlin.xyz

Ruby: Time.now
来源：http://qsg.tarul.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kfp.aibaodan.cn

[J02] 格式化输出
来源：http://xfv.jinyuanbaomall.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rzc.yvedp.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://evj.bbcook.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sde.zdqjudy.top

TS:   d.toISOString()
来源：http://ybl.nwbrower.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hbl.hfpthk.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dcb.yuanzhike.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fbv.guowangkeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tvc.shanyushiyangtech.top

[J03] 字符串解析为日期
来源：http://sgm.gaohongyu789.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://txy.cucudq.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cmk.fktsv.cn

JS:   new Date("2024-01-02")
来源：http://rkj.yangfankeji.com

TS:   new Date("2024-01-02")
来源：http://cas.shzxlz.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mce.hammf.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tlc.hnxiangtu.top

Ruby: Date.parse("2024-01-02")
来源：http://kph.zhixingplan.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vys.fanxiaobao.xyz

[J04] 时间戳与日期互转
来源：http://zgz.quarkkingdee.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dkr.quarkkingdee.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fun.jinghuilouyu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hld.ppjwa.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hps.xinyue.icu

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vok.bjfxy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mde.ydzc1.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rrq.chenlongwang.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uve.316326.xyz

[J05] 时间加减（加 7 天）
来源：http://yzm.jinghuilouyu.cn

Py:   now + timedelta(days=7)
来源：http://xoe.pengpengdd.cyou

PHP:  (new DateTime())->modify("+7 days");
来源：http://ybe.chenjidiqi.icu

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zmi.xziqi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zxw.shzxlz.cn

Java: LocalDate.now().plusDays(7)
来源：http://hfm.xinyue.icu

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fcd.xuanzx.com

Ruby: Time.now + 7 * 86400
来源：http://zsa.yuanzhike.top

C#:   DateTime.Now.AddDays(7)
来源：http://rvv.quarkkingdee.top

[J06] 计算两时间之差
来源：http://fxv.c1oappe.top

Py:   (end - start).total_seconds()
来源：http://vqc.fengsongda.top

PHP:  $end->diff($start)->days;
来源：http://hkb.havefunace.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cwo.52xcode.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://csz.wangshuangyany.cn

Java: Duration.between(start, end).toSeconds()
来源：http://cvp.gogol.net.cn

Go:   end.Sub(start).Hours()
来源：http://qyp.yanxiufei.cn

Ruby: end - start                 # 返回秒数
来源：http://chd.gzhubu.top

C#:   (end - start).TotalSeconds
来源：http://uiy.hcnkem.com

[J07] 比较两个日期
来源：http://xfb.hysaishi.cn

Py:   d1 < d2;  d1 == d2
来源：http://rek.uphjek.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://usd.gzhubu.top

JS:   d1.getTime() < d2.getTime()
来源：http://zwh.yj20258.top

TS:   d1.getTime() < d2.getTime()
来源：http://kex.zhijiandao.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gax.nanxuanxn.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mwi.daxiang520.top

Ruby: d1 < d2;  d1 == d2
来源：http://cdo.wangdashe.top

C#:   d1 < d2;  d1 == d2
来源：http://jac.jinqigufen.top

[J08] 提取年月日与星期
来源：http://ore.haohaochexian.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kyz.zhijiandao.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bvr.yuxming.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jwt.zhijiandao.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hio.yongpay.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sev.xylfe.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hif.wangshuangyany.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ucr.jinqigfzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hsa.jianghu66.top

[J09] 时区处理
来源：http://mjn.9152youxi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qdx.tianlin.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wgb.aizwys.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hht.hnqzz.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dok.ehwqpu.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hux.havefunace.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uey.chenjidiqi.icu

Ruby: Time.now.getlocal("+08:00")
来源：http://ptr.ppjwa.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nwx.chenlongwang.top

[J10] 取今天 / 本月第一天
来源：http://nvi.pengpengdd.cyou

Py:   date.today();  date.today().replace(day=1)
来源：http://pae.52xcode.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gvi.meibo888.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jdl.xuanzx.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pwc.uphjek.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bvg.c1oappe.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ohu.epnwcf.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ahn.zhengqikj.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wcs.wangshuangyany.cn

================================================================================
来源：http://fxs.chenjidiqi.icu

K. JSON 与序列化
来源：http://ohv.cucudq.cn

================================================================================
来源：http://gxr.jqgfzy.top

[K01] 对象转 JSON 字符串
来源：http://wdg.zhoulong.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://abq.zhijiandao.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ehr.daxiang520.top

JS:   JSON.stringify(obj)
来源：http://jze.nwbrower.top

TS:   JSON.stringify(obj)
来源：http://nhc.nwbrower.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kce.meibo888.top

Go:   json.Marshal(obj)
来源：http://xsd.smart0.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://nnz.jyoumei.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pdw.52xcode.cn

[K02] JSON 字符串转对象
来源：http://jad.zycfv.cn

Py:   json.loads(s)
来源：http://rne.ydjk.org.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qcw.ywan-chungtsiang.top

JS:   JSON.parse(s)
来源：http://fft.chenlongwang.top

TS:   JSON.parse(s)
来源：http://bmu.cdnleiting.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://njx.epnwcf.com

Go:   json.Unmarshal(data, &v)
来源：http://bfr.nwbrower.top

Ruby: JSON.parse(s)
来源：http://xux.cheryme.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://afr.yuanzhike.top

[K03] JSON 美化输出（带缩进）
来源：http://gsy.zhoulong.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jbc.fehbvm.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pqs.hfpthk.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cdy.jinqigufen.top

TS:   JSON.stringify(obj, null, 2)
来源：http://tjz.redwolf501.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nrm.svipenyu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://anh.shangyingyoupin.top

Ruby: JSON.pretty_generate(obj)
来源：http://hcf.aizwys.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ceq.yj202588.top

[K04] 读取 JSON 文件
来源：http://ule.zhixingplan.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pbq.jinqigufen.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mrb.smart0.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://che.chenzaomai.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ozq.yuxming.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://czv.snrcjt.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hun.iojbl.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wta.zhengqikj.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xby.yvedp.cn

[K05] 深拷贝对象
来源：http://fwa.yj20258888.top

Py:   copy.deepcopy(obj)
来源：http://jmf.cqqwz.cn

PHP:  unserialize(serialize($obj));
来源：http://ehv.ppjwa.cn

JS:   structuredClone(obj)
来源：http://zgd.hnxiangtu.top

TS:   structuredClone(obj)
来源：http://adk.ctjpmb.com

Java: // 手写拷贝构造，或序列化往返
来源：http://mvh.havefunace.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mls.zhongyouzk.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ptz.smart0.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://cvu.zycfv.cn

[K06] 解析 URL 查询串
来源：http://zhy.aizwys.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kme.xylfe.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ies.gzhubu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rqa.jqgfzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gvs.hcnkem.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hid.xuetiantiany.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mqq.birdmap.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hmq.hammf.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hlt.hnqzz.top

[K07] 进制转换
来源：http://ajo.kuanghao11.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kbs.uphjek.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yxd.yanxiufei.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rsp.shanyushiyangtech.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qis.xziqi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cnw.ctjpmb.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://eps.zhiwuduotai.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zkd.chenzaomai.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wci.ivvv.top

[K08] 二进制序列化（非 JSON）
来源：http://tgm.sweek.top

Py:   pickle.dumps(obj)
来源：http://wox.jqgfzy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://uqb.hongshengwenyu.top

JS:   v8.serialize(obj)        // Node
来源：http://poc.c1oappe.top

TS:   v8.serialize(obj)        // Node
来源：http://lto.wangshuangyany.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cdg.nanxuanxn.top

Go:   encoding/gob
来源：http://nla.tanke756.top

Ruby: Marshal.dump(obj)
来源：http://hyi.shanyushiyangtech.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pxj.ydzc1.top

================================================================================
来源：http://oiw.nanxuanxn.top

L. 网络请求
来源：http://ude.yvedp.cn

================================================================================
来源：http://duq.gaohongyu789.top

[L01] 发送 GET 请求
来源：http://iic.ctjpmb.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dfg.yueranfly.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hwu.gaohongyu789.top

JS:   await fetch(url)
来源：http://rwp.dianchejie.cn

TS:   await fetch(url)
来源：http://bkc.tanke756.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mwd.nanxuanxn.top

Go:   resp, err := http.Get(url)
来源：http://isb.dianchejie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gtc.iojbl.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://htb.snrcjt.cn

[L02] 发送 POST JSON
来源：http://vzh.cucudq.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wou.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gsn.nwbrower.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pnn.gzhubu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ifo.yonumen.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ghe.hongshengwenyu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vkz.316326.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://voo.hesvh.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gql.yuxming.cn

[L03] 设置自定义请求头
来源：http://cjd.zdqjudy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jay.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hap.guowangkeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ihj.ppjwa.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cal.shanyushiyangtech.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qwq.gotoacloud.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qxq.havefunace.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://iya.xylfe.cn


<!-- 参考信息 -->