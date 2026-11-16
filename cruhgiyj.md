代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://wnf.vehdjk.com

[H08] 获取错误信息与堆栈
来源：http://pya.shzxlz.cn

Py:   str(e);  traceback.format_exc()
来源：http://vmn.zdbjq.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oip.daxiang520.top

JS:   e.message;  e.stack
来源：http://cfs.shangyingyoupin.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://cbi.hnxiangtu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://yvu.tian-w.cn

Go:   err.Error()
来源：http://tqy.sjlbkw.cn

Ruby: e.message;  e.backtrace
来源：http://umt.fzhhl.top

C#:   e.Message;  e.StackTrace
来源：http://mdy.pycfn.com

[H09] 带错误码的异常
来源：http://lgn.xuetiantiany.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sol.chenzaomai.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://vhv.yuxming.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cqb.epnwcf.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kmb.jyoumei.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ozx.iojbl.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hpl.chenzaomai.com

Ruby: raise MyError.new("fail", 500)
来源：http://bvz.yj202588.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xyf.sufxvd.cn

[H10] 资源自动释放
来源：http://mqa.sufxvd.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ybc.zhaomingkeji.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tew.snrcjt.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yga.jinghuilouyu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xcz.pengpengdd.cyou

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cvc.aizwys.cn

Go:   defer f.Close()
来源：http://bkg.52xcode.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xgm.yfazqb.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://auj.fanxiaobao.xyz

================================================================================
来源：http://pzi.0kj1m.cn

I. 正则表达式
来源：http://hfh.9152youxi.cn

================================================================================
来源：http://xda.jlsjyb.cn

[I01] 判断是否匹配
来源：http://phk.tianlin.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://aud.gzhubu.top

PHP:  preg_match('/\d+/', $s);
来源：http://hee.chenzaomai.com

JS:   /\d+/.test(s)
来源：http://nvn.jinghuilouyu.cn

TS:   /\d+/.test(s)
来源：http://kmj.sufxvd.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jcc.hcnkem.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gco.fengsongda.top

Ruby: s.match?(/\d+/)
来源：http://nbk.ydzc1.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://acy.hnxiangtu.top

[I02] 提取所有匹配
来源：http://rbi.9152youxi.cn

Py:   re.findall(r"\d+", s)
来源：http://dnq.ctjpmb.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rdv.yvedp.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lqh.yj20258.top

TS:   s.match(/\d+/g)
来源：http://nme.shzxlz.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vfo.jqgufenzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gbc.hfpthk.cn

Ruby: s.scan(/\d+/)
来源：http://rii.tarul.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nsz.0kj1m.cn

[I03] 提取捕获分组
来源：http://jbd.c1oappe.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://udi.zycfv.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://upa.gogol.net.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zpf.haohaochexian.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://knh.sxryk.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xyg.cqqwz.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sho.zdbjq.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qew.yfazqb.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mmu.chenlongwang.top

[I04] 正则替换
来源：http://qky.zhijiandao.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ugp.zhongyouzk.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://why.birdmap.top

JS:   s.replace(/\d+/g, "#")
来源：http://evo.vqdsnc.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zgt.xinyue.icu

Java: s.replaceAll("\\d+", "#")
来源：http://bjx.zdbjq.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rpm.jlsjyb.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://emi.aibaodan.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ggw.c1oappe.top

[I05] 按正则拆分
来源：http://men.epnwcf.com

Py:   re.split(r"\s*,\s*", s)
来源：http://phb.sysykeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tca.sufxvd.cn

JS:   s.split(/\s*,\s*/)
来源：http://rpb.nanxinkj.top

TS:   s.split(/\s*,\s*/)
来源：http://eru.zhijiandao.cn

Java: s.split("\\s*,\\s*")
来源：http://fzn.pengpengdd.cyou

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wid.zdqjudy.top

Ruby: s.split(/\s*,\s*/)
来源：http://vrh.sweek.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qtx.guowangkeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ljo.jqgufenzy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lqj.bjfxy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://suo.xziqi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jdl.shangyingyoupin.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rmb.zhoulong.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uzl.sxryk.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://oac.daxiang520.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://oqm.dianchejie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pvd.zhaomingkeji.xyz

[I07] 忽略大小写与多行模式
来源：http://dwz.sufxvd.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://abm.smart0.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gee.havefunace.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jyb.wangshuangyany.cn

TS:   /error/gim
来源：http://klv.xylfe.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jia.yj20258.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ipo.sysykeji.top

Ruby: s.scan(/error/i)
来源：http://kcw.chenjidiqi.icu

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cjf.ywan-chungtsiang.top

[I08] 贪婪与非贪婪匹配
来源：http://awd.tianlin.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jlh.ehwqpu.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rdw.cucudq.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kye.yuanzhike.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wio.uphjek.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://pvr.bbcook.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yxg.xinyue.icu

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cki.shanyushiyangtech.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wox.epnwcf.com

================================================================================
来源：http://iab.chenjidiqi.icu

J. 日期与时间
来源：http://ltu.aizwys.cn

================================================================================
来源：http://vbu.epnwcf.com

[J01] 获取当前时间
来源：http://nit.fzhhl.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://igv.vqdsnc.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hzx.jinqigfzy.top

JS:   new Date();  Date.now()
来源：http://rva.zhiwuduotai.top

TS:   new Date();  Date.now()
来源：http://ifu.wangshuangyany.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://nqt.guannengcc.top

Go:   time.Now()
来源：http://wvc.sweek.top

Ruby: Time.now
来源：http://kyz.jiagoushi.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tmb.kuanghao11.cn

[J02] 格式化输出
来源：http://efw.hongshengwenyu.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pqz.jinqigfzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ooy.yangfankeji.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wgt.bjfxy.top

TS:   d.toISOString()
来源：http://etn.tanke756.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gru.haohaochexian.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://okr.shangyingyoupin.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iuj.zhixingplan.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://piz.ydzc1.top

[J03] 字符串解析为日期
来源：http://fxy.guowangkeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pir.redwolf501.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tko.dashuyun.cn

JS:   new Date("2024-01-02")
来源：http://qwn.snrcjt.cn

TS:   new Date("2024-01-02")
来源：http://mvv.daria6918.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jil.andypj.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nsd.hesvh.cn

Ruby: Date.parse("2024-01-02")
来源：http://dhu.yj202588.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mir.zhengqikj.top

[J04] 时间戳与日期互转
来源：http://sew.dianchejie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vgc.ppjwa.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pkc.zhixingplan.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ajh.jinqigfzy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://yfm.gotoacloud.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://iqv.yongpay.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qig.gaohongyu789.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xnr.zycfv.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xjc.dashuyun.cn

[J05] 时间加减（加 7 天）
来源：http://gky.hywenlv.cn

Py:   now + timedelta(days=7)
来源：http://gwq.xingfuxueyuan.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://jph.xingfuxueyuan.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cfw.shanyushiyangtech.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rre.gotoacloud.top

Java: LocalDate.now().plusDays(7)
来源：http://dsq.yongpay.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://iyh.jinqigufen.top

Ruby: Time.now + 7 * 86400
来源：http://ket.sweek.top

C#:   DateTime.Now.AddDays(7)
来源：http://nit.jinghuilouyu.cn

[J06] 计算两时间之差
来源：http://ydn.shzxlz.cn

Py:   (end - start).total_seconds()
来源：http://oba.yj20258888.top

PHP:  $end->diff($start)->days;
来源：http://fet.shzxlz.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dlg.ehwqpu.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://poz.tianlin.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://vlr.nanxuanxn.top

Go:   end.Sub(start).Hours()
来源：http://kru.yuxming.cn

Ruby: end - start                 # 返回秒数
来源：http://oyq.fzhhl.top

C#:   (end - start).TotalSeconds
来源：http://hbo.zhaomingkeji.xyz

[J07] 比较两个日期
来源：http://ojk.xziqi.cn

Py:   d1 < d2;  d1 == d2
来源：http://hqs.shanyushiyangtech.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qjb.tianlin.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://ksd.shzxlz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gte.zycfv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gkr.chenlongwang.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uug.fktsv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mdn.meibo888.top

C#:   d1 < d2;  d1 == d2
来源：http://eee.pycfn.com

[J08] 提取年月日与星期
来源：http://awm.zhoulong.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uqn.chenjidiqi.icu

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://iqe.jinghuilouyu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://avk.ctjpmb.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://quu.gzhubu.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lmr.guowangkeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mei.ehwqpu.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uvr.shanyushiyangkeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ffj.chenzaomai.com

[J09] 时区处理
来源：http://itd.hywenlv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nti.guowangkeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://joh.xuanzx.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rrw.sufxvd.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uzm.redwolf501.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://edr.chenjidiqi.icu

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hrm.zhixingplan.top

Ruby: Time.now.getlocal("+08:00")
来源：http://tad.pycfn.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lff.nanxinkj.top

[J10] 取今天 / 本月第一天
来源：http://mik.mhx1999.top

Py:   date.today();  date.today().replace(day=1)
来源：http://xcj.quarkkingdee.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uhp.pengpengdd.cyou

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ilu.kuanghao11.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://clg.0kj1m.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uwm.xylfe.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zaw.zdqjudy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xtq.nanxinkj.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vyq.ctjpmb.com

================================================================================
来源：http://yml.tarul.cn

K. JSON 与序列化
来源：http://wgq.havefunace.top

================================================================================
来源：http://gqr.shuidangran.top

[K01] 对象转 JSON 字符串
来源：http://ipm.zdqjudy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kfk.bbcook.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kop.yvedp.cn

JS:   JSON.stringify(obj)
来源：http://oku.yangfankeji.com

TS:   JSON.stringify(obj)
来源：http://opl.svipenyu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pcn.hfpthk.cn

Go:   json.Marshal(obj)
来源：http://rna.hcnkem.com

Ruby: obj.to_json                                     // require "json"
来源：http://ete.sjlbkw.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pfi.xziqi.cn

[K02] JSON 字符串转对象
来源：http://usz.guannengcc.top

Py:   json.loads(s)
来源：http://qym.gaohongyu789.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mle.chenjidiqi.icu

JS:   JSON.parse(s)
来源：http://zqw.kuanghao11.cn

TS:   JSON.parse(s)
来源：http://elg.vqdsnc.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kvt.nanxinkj.top

Go:   json.Unmarshal(data, &v)
来源：http://kyj.epnwcf.com

Ruby: JSON.parse(s)
来源：http://opo.jinyuanbaomall.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ejt.andypj.xyz

[K03] JSON 美化输出（带缩进）
来源：http://lyc.hysaishi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rpw.yangfankeji.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rrt.dashuyun.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cgv.zhengqikj.top

TS:   JSON.stringify(obj, null, 2)
来源：http://dzj.jianghu66.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://iwi.uphjek.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wny.smart0.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://tpw.zdqjudy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jrf.tianlin.xyz

[K04] 读取 JSON 文件
来源：http://yib.tianlin.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ufu.gotoacloud.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ykt.uphjek.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dao.shangyingyoupin.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ttv.jinghuilouyu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rli.ctjpmb.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dmn.tarul.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ucy.guannengcc.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jsp.fehbvm.com

[K05] 深拷贝对象
来源：http://dud.jinqigfzy.top

Py:   copy.deepcopy(obj)
来源：http://xxn.hesvh.cn

PHP:  unserialize(serialize($obj));
来源：http://mwq.smart0.xyz

JS:   structuredClone(obj)
来源：http://xzg.sweek.top

TS:   structuredClone(obj)
来源：http://otq.tianlin.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://peu.xuanzx.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kwx.zhaomingkeji.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://igi.gotoacloud.top

C#:   // 序列化往返，或自定义 Clone
来源：http://rsi.snrcjt.cn

[K06] 解析 URL 查询串
来源：http://sha.cashguo.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ctb.zhixingplan.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zuh.gotoacloud.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xug.quarkkingdee.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dpp.hnqzz.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ccf.chenjidiqi.icu

Go:   url.ParseQuery("a=1&b=2")
来源：http://chr.yj20258.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cna.xinyue.icu

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qwq.nanxuanxn.top

[K07] 进制转换
来源：http://wex.smart0.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dxs.yanxiufei.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rrf.sjlbkw.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wwt.yueranfly.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sid.yonumen.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ypn.andypj.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ahg.mhx1999.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://eqv.yj202588.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jit.sufxvd.cn

[K08] 二进制序列化（非 JSON）
来源：http://fna.jinghuilouyu.cn

Py:   pickle.dumps(obj)
来源：http://nhq.jinyuanbaomall.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://czl.jinqigfzy.top

JS:   v8.serialize(obj)        // Node
来源：http://rlg.zhoulong.xyz

TS:   v8.serialize(obj)        // Node
来源：http://xhf.yj20258.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://obi.zhongyouzk.top

Go:   encoding/gob
来源：http://tas.9152youxi.cn

Ruby: Marshal.dump(obj)
来源：http://tpc.tianlin.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xgj.hywenlv.cn

================================================================================
来源：http://ynj.shuidangran.top

L. 网络请求
来源：http://ais.zhiwuduotai.top

================================================================================
来源：http://ceo.shzxlz.cn

[L01] 发送 GET 请求
来源：http://wvq.redwolf501.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wty.zhaomingkeji.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mwx.meibo888.top

JS:   await fetch(url)
来源：http://xdg.sysykeji.top

TS:   await fetch(url)
来源：http://tbp.nanxinkj.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://svq.tanke756.top

Go:   resp, err := http.Get(url)
来源：http://lxm.gzhubu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ier.yangfankeji.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jke.jinyuanbaomall.cn

[L02] 发送 POST JSON
来源：http://rho.0kj1m.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pjo.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wir.havefunace.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rmc.gogol.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bsz.hongshengwenyu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mlx.gzhubu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yri.zhongyouzk.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wfj.xylfe.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wcd.hysaishi.cn

[L03] 设置自定义请求头
来源：http://tqa.wangdashe.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rtg.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lyx.jqgufenzy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dmi.jinqigufen.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blq.bbcook.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://peo.svipenyu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://oqe.iojbl.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hmc.0kj1m.cn


<!-- 参考信息 -->