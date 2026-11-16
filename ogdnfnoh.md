代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://afp.sweek.top

[H08] 获取错误信息与堆栈
来源：http://qgp.quarkkingdee.top

Py:   str(e);  traceback.format_exc()
来源：http://jjd.fengsongda.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://szp.yuxming.cn

JS:   e.message;  e.stack
来源：http://goe.wangdashe.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://zqo.zhaomingkeji.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://vju.kuanghao11.cn

Go:   err.Error()
来源：http://onu.9152youxi.cn

Ruby: e.message;  e.backtrace
来源：http://qlm.yangfankeji.com

C#:   e.Message;  e.StackTrace
来源：http://hsl.ywan-chungtsiang.top

[H09] 带错误码的异常
来源：http://eca.c1oappe.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vrp.zhijiandao.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ybn.bbcook.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dhz.dianchejie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tes.jyoumei.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://plz.yonumen.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mcj.cashguo.top

Ruby: raise MyError.new("fail", 500)
来源：http://gmh.fzhhl.top

C#:   // 自定义异常类中加 Code 属性
来源：http://pvh.9152youxi.cn

[H10] 资源自动释放
来源：http://nps.andypj.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://daq.zhoulong.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ptd.pengpengdd.cyou

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nar.smart0.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rom.jinghuilouyu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://waz.chenlongwang.top

Go:   defer f.Close()
来源：http://lkh.vqdsnc.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://eac.shzxlz.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://roh.zhixingplan.top

================================================================================
来源：http://etc.cdnleiting.top

I. 正则表达式
来源：http://rbu.ivvv.top

================================================================================
来源：http://rov.xylfe.cn

[I01] 判断是否匹配
来源：http://wpo.tarul.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rvn.gaohongyu789.top

PHP:  preg_match('/\d+/', $s);
来源：http://ked.xylfe.cn

JS:   /\d+/.test(s)
来源：http://pua.yuanzhike.top

TS:   /\d+/.test(s)
来源：http://mms.daxiang520.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://taw.gotoacloud.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kon.zdqjudy.top

Ruby: s.match?(/\d+/)
来源：http://tpk.shanyushiyangkeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://urw.tanke756.top

[I02] 提取所有匹配
来源：http://ied.shuidangran.top

Py:   re.findall(r"\d+", s)
来源：http://uuw.wangdashe.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ift.hysaishi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ghw.yuanzhike.top

TS:   s.match(/\d+/g)
来源：http://gwj.yueranfly.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://iqf.52xcode.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nho.daxiang520.top

Ruby: s.scan(/\d+/)
来源：http://jyb.gaohongyu789.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cts.redwolf501.top

[I03] 提取捕获分组
来源：http://xms.fengsongda.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lxn.yonumen.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pvp.sjlbkw.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fhc.yueranfly.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fan.hongshengwenyu.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gqm.jlsjyb.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ttj.snrcjt.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zfy.yj20258.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gkd.iojbl.cn

[I04] 正则替换
来源：http://miz.yangfankeji.com

Py:   re.sub(r"\d+", "#", s)
来源：http://wzk.vehdjk.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vkw.zhijiandao.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kxo.xziqi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rln.fktsv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://uda.iojbl.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://sit.jinyuanbaomall.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zjw.pengpengdd.cyou

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wky.zhongyouzk.top

[I05] 按正则拆分
来源：http://jaq.xuetiantiany.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fnu.feifeiyinyue.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lvd.chenlongwang.top

JS:   s.split(/\s*,\s*/)
来源：http://pji.nanxinkj.top

TS:   s.split(/\s*,\s*/)
来源：http://byd.hysaishi.cn

Java: s.split("\\s*,\\s*")
来源：http://afi.jiagoushi.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wpq.cucudq.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mrq.quarkkingdee.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ntm.hcnkem.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bdy.cqqwz.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xhh.daxiang520.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vif.aibaodan.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xew.bbcook.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rxt.yj20258.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kqw.wangdashe.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://akm.hywenlv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vwp.zycfv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://htw.yj20258888.top

[I07] 忽略大小写与多行模式
来源：http://yhf.gzhubu.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rkl.hywenlv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rwt.0kj1m.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nfp.zdbjq.cn

TS:   /error/gim
来源：http://ffp.xinyue.icu

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ewa.ydjk.org.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xsx.uphjek.com

Ruby: s.scan(/error/i)
来源：http://ura.zycfv.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oxy.fengsongda.top

[I08] 贪婪与非贪婪匹配
来源：http://nta.shangyingyoupin.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hzz.jianghu66.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zes.sweek.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gju.cashguo.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kwx.birdmap.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://eaw.birdmap.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hca.gogol.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uvh.316326.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xcn.316326.xyz

================================================================================
来源：http://yiq.hnxiangtu.top

J. 日期与时间
来源：http://kvl.nwbrower.top

================================================================================
来源：http://gpi.zhoulong.xyz

[J01] 获取当前时间
来源：http://knw.tian-w.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gyt.yuxming.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cfh.svipenyu.cn

JS:   new Date();  Date.now()
来源：http://ngm.hysaishi.cn

TS:   new Date();  Date.now()
来源：http://zzo.fzhhl.top

Java: LocalDateTime.now();  Instant.now()
来源：http://yfj.316326.xyz

Go:   time.Now()
来源：http://jcu.0kj1m.cn

Ruby: Time.now
来源：http://mcx.hfpthk.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fty.meibo888.top

[J02] 格式化输出
来源：http://gds.yuanzhike.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ftg.chenlongwang.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uas.yanxiufei.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nls.cheryme.top

TS:   d.toISOString()
来源：http://pmt.pengpengdd.cyou

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pjr.bbcook.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://njk.0kj1m.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cyi.jianghu66.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pwk.tanke756.top

[J03] 字符串解析为日期
来源：http://yoj.yuanzhike.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ozf.yj20258.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gqs.hywenlv.cn

JS:   new Date("2024-01-02")
来源：http://rnh.hywenlv.cn

TS:   new Date("2024-01-02")
来源：http://mwq.ydjk.org.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gvz.chenlongwang.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://laz.jqgufenzy.top

Ruby: Date.parse("2024-01-02")
来源：http://uzr.pycfn.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://biu.tarul.cn

[J04] 时间戳与日期互转
来源：http://klx.0kj1m.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vtw.hammf.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hyr.meibo888.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qec.jiagoushi.top

TS:   Math.floor(Date.now() / 1000)
来源：http://edh.c1oappe.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ahk.c1oappe.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pbr.yongpay.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pbe.andypj.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nnl.yongpay.top

[J05] 时间加减（加 7 天）
来源：http://ezn.daria6918.cn

Py:   now + timedelta(days=7)
来源：http://nhu.birdmap.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://zls.haohaochexian.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kev.ctjpmb.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lmj.hesvh.cn

Java: LocalDate.now().plusDays(7)
来源：http://hvk.jlsjyb.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://omc.fehbvm.com

Ruby: Time.now + 7 * 86400
来源：http://voc.zhoulong.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://sxd.zdqjudy.top

[J06] 计算两时间之差
来源：http://ini.hysaishi.cn

Py:   (end - start).total_seconds()
来源：http://iqw.daria6918.cn

PHP:  $end->diff($start)->days;
来源：http://zdk.smart0.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dey.zhengqikj.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gvy.iojbl.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mft.ydzc1.top

Go:   end.Sub(start).Hours()
来源：http://nrc.ywan-chungtsiang.top

Ruby: end - start                 # 返回秒数
来源：http://uzo.birdmap.top

C#:   (end - start).TotalSeconds
来源：http://jpz.epnwcf.com

[J07] 比较两个日期
来源：http://ant.cucudq.cn

Py:   d1 < d2;  d1 == d2
来源：http://wer.yanxiufei.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gpr.epnwcf.com

JS:   d1.getTime() < d2.getTime()
来源：http://zki.xinyue.icu

TS:   d1.getTime() < d2.getTime()
来源：http://rjb.haohaochexian.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zzy.yueranfly.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://eox.fehbvm.com

Ruby: d1 < d2;  d1 == d2
来源：http://foy.smart0.xyz

C#:   d1 < d2;  d1 == d2
来源：http://kbq.gotoacloud.top

[J08] 提取年月日与星期
来源：http://ssj.yfazqb.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bbr.chenjidiqi.icu

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xhd.jqgfzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xqi.jiagoushi.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gku.hnxiangtu.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://agw.jianghu66.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dhi.havefunace.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dol.hammf.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kgf.sjlbkw.cn

[J09] 时区处理
来源：http://axz.pengpengdd.cyou

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tte.yongpay.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ypx.snrcjt.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lyy.daxiang520.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tli.cucudq.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sri.mhx1999.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bnh.sxryk.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vul.ctjpmb.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://aex.fanxiaobao.xyz

[J10] 取今天 / 本月第一天
来源：http://byn.yuanzhike.top

Py:   date.today();  date.today().replace(day=1)
来源：http://oew.daxiang520.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ykh.shangyingyoupin.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vda.ctjpmb.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yri.gogol.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hmq.xuetiantiany.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hhp.xinyue.icu

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mqw.hnqzz.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kza.9152youxi.cn

================================================================================
来源：http://nlz.dianchejie.cn

K. JSON 与序列化
来源：http://pdv.gotoacloud.top

================================================================================
来源：http://olp.ybcxt.top

[K01] 对象转 JSON 字符串
来源：http://qio.shangyingyoupin.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vhi.zhengqikj.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://auy.ppjwa.cn

JS:   JSON.stringify(obj)
来源：http://rmt.quarkkingdee.top

TS:   JSON.stringify(obj)
来源：http://yzs.hnqzz.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://esu.hesvh.cn

Go:   json.Marshal(obj)
来源：http://tgn.ctjpmb.com

Ruby: obj.to_json                                     // require "json"
来源：http://ksb.feifeiyinyue.top

C#:   JsonSerializer.Serialize(obj)
来源：http://asa.cashguo.top

[K02] JSON 字符串转对象
来源：http://lbj.aibaodan.cn

Py:   json.loads(s)
来源：http://fpd.sufxvd.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fvb.nwbrower.top

JS:   JSON.parse(s)
来源：http://qpp.0kj1m.cn

TS:   JSON.parse(s)
来源：http://cbo.fanxiaobao.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wok.shzxlz.cn

Go:   json.Unmarshal(data, &v)
来源：http://kyz.gzhubu.top

Ruby: JSON.parse(s)
来源：http://ktk.ehwqpu.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lca.jiagoushi.top

[K03] JSON 美化输出（带缩进）
来源：http://vbl.xinyue.icu

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pnt.cqqwz.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ceu.hongshengwenyu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://xrd.yangfankeji.com

TS:   JSON.stringify(obj, null, 2)
来源：http://vvi.hnqzz.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dco.hesvh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kxv.feifeiyinyue.top

Ruby: JSON.pretty_generate(obj)
来源：http://hio.yvedp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uue.feifeiyinyue.top

[K04] 读取 JSON 文件
来源：http://yji.hfpthk.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://eno.fktsv.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iup.xylfe.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xli.hongshengwenyu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hqn.haohaochexian.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gia.hysaishi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://iyx.hywenlv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://imj.hesvh.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mjk.zhoulong.xyz

[K05] 深拷贝对象
来源：http://bri.xziqi.cn

Py:   copy.deepcopy(obj)
来源：http://lld.andypj.xyz

PHP:  unserialize(serialize($obj));
来源：http://agc.zdbjq.cn

JS:   structuredClone(obj)
来源：http://mdf.tian-w.cn

TS:   structuredClone(obj)
来源：http://yrq.jinyuanbaomall.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cif.jqgufenzy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ccv.chenlongwang.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uyy.shuidangran.top

C#:   // 序列化往返，或自定义 Clone
来源：http://xak.yj20258888.top

[K06] 解析 URL 查询串
来源：http://ask.shanyushiyangtech.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pgp.daxiang520.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://phu.svipenyu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dnp.jlsjyb.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ptt.shuidangran.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bdj.quarkkingdee.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://utj.redwolf501.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sky.zhongyouzk.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hcl.ydjk.org.cn

[K07] 进制转换
来源：http://pmf.hongshengwenyu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ktd.fanxiaobao.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cgw.nwbrower.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ebd.jlsjyb.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vai.yonumen.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nvi.ppjwa.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bbx.zhengqikj.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ggo.shanyushiyangtech.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://eto.yfazqb.com

[K08] 二进制序列化（非 JSON）
来源：http://nqc.xingfuxueyuan.xyz

Py:   pickle.dumps(obj)
来源：http://fqr.chenzaomai.com

PHP:  serialize($obj);  unserialize($s);
来源：http://kzy.jinqigfzy.top

JS:   v8.serialize(obj)        // Node
来源：http://zyg.aibaodan.cn

TS:   v8.serialize(obj)        // Node
来源：http://iwp.guannengcc.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uan.gaohongyu789.top

Go:   encoding/gob
来源：http://iek.tarul.cn

Ruby: Marshal.dump(obj)
来源：http://yzq.52xcode.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qqv.nanxuanxn.top

================================================================================
来源：http://zra.dianchejie.cn

L. 网络请求
来源：http://mxn.hongshengwenyu.top

================================================================================
来源：http://iue.hysaishi.cn

[L01] 发送 GET 请求
来源：http://cbh.cheryme.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xos.vehdjk.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wjm.ehwqpu.com

JS:   await fetch(url)
来源：http://pah.snrcjt.cn

TS:   await fetch(url)
来源：http://gfd.daria6918.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wbl.yj20258888.top

Go:   resp, err := http.Get(url)
来源：http://tek.aizwys.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://mbb.tarul.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sot.quarkkingdee.top

[L02] 发送 POST JSON
来源：http://jfs.hfpthk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://esw.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://smc.zycfv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iae.mhx1999.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lki.aizwys.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yvs.chenjidiqi.icu

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rse.tanke756.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qwz.ehwqpu.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pod.jyoumei.cn

[L03] 设置自定义请求头
来源：http://xrz.dianchejie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bku.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uok.hesvh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jpl.zhiwuduotai.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pyt.pengpengdd.cyou

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://agr.guannengcc.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uay.316326.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kbf.daxiang520.top


<!-- 参考信息 -->