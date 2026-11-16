代发 wailian999

JS:   e.message;  e.stack
来源：http://bjs.fzhhl.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://dhu.chenjidiqi.icu

Java: e.getMessage();  e.printStackTrace()
来源：http://usn.cashguo.top

Go:   err.Error()
来源：http://fki.9152youxi.cn

Ruby: e.message;  e.backtrace
来源：http://yox.tian-w.cn

C#:   e.Message;  e.StackTrace
来源：http://hva.aizwys.cn

[H09] 带错误码的异常
来源：http://nvt.yfazqb.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pgt.cqqwz.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://idv.fktsv.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uov.wangshuangyany.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ogn.zhaomingkeji.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hfo.cqqwz.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://aqb.c1oappe.top

Ruby: raise MyError.new("fail", 500)
来源：http://nec.feifeiyinyue.top

C#:   // 自定义异常类中加 Code 属性
来源：http://kuj.yj20258.top

[H10] 资源自动释放
来源：http://lub.ydjk.org.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hoy.nanxinkj.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://swj.yuxming.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://amc.yj20258888.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vmh.hfpthk.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://eez.kuanghao11.cn

Go:   defer f.Close()
来源：http://pnt.hywenlv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ggf.sxryk.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xme.xingfuxueyuan.xyz

================================================================================
来源：http://gib.yfazqb.com

I. 正则表达式
来源：http://wjp.tianlin.xyz

================================================================================
来源：http://dfz.zhongyouzk.top

[I01] 判断是否匹配
来源：http://llv.aizwys.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tbl.yanxiufei.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gxv.hnxiangtu.top

JS:   /\d+/.test(s)
来源：http://pxo.vehdjk.com

TS:   /\d+/.test(s)
来源：http://knx.vqdsnc.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ily.hesvh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://spu.shuidangran.top

Ruby: s.match?(/\d+/)
来源：http://dnu.9152youxi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mob.yuxming.cn

[I02] 提取所有匹配
来源：http://oxy.tian-w.cn

Py:   re.findall(r"\d+", s)
来源：http://rlo.wangdashe.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qsh.yj202588.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rrv.haohaochexian.top

TS:   s.match(/\d+/g)
来源：http://rup.gogol.net.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://stf.9152youxi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qxz.hammf.cn

Ruby: s.scan(/\d+/)
来源：http://koo.jinqigfzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jac.quarkkingdee.top

[I03] 提取捕获分组
来源：http://fad.haohaochexian.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://unq.dashuyun.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kgk.yanxiufei.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mtm.shanyushiyangkeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fic.yuanzhike.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rgb.xuetiantiany.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tmf.nwbrower.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rfs.fzhhl.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ztm.yj20258.top

[I04] 正则替换
来源：http://mgk.havefunace.top

Py:   re.sub(r"\d+", "#", s)
来源：http://oey.cdnleiting.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jjv.ywan-chungtsiang.top

JS:   s.replace(/\d+/g, "#")
来源：http://zhm.yj20258888.top

TS:   s.replace(/\d+/g, "#")
来源：http://akc.yangfankeji.com

Java: s.replaceAll("\\d+", "#")
来源：http://uvt.shzxlz.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://svh.yj20258.top

Ruby: s.gsub(/\d+/, "#")
来源：http://wiq.shanyushiyangkeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sfy.hammf.cn

[I05] 按正则拆分
来源：http://qhs.yonumen.top

Py:   re.split(r"\s*,\s*", s)
来源：http://wwk.feifeiyinyue.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vbr.jyoumei.cn

JS:   s.split(/\s*,\s*/)
来源：http://ief.yangfankeji.com

TS:   s.split(/\s*,\s*/)
来源：http://vub.smart0.xyz

Java: s.split("\\s*,\\s*")
来源：http://khv.cqqwz.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ajn.bjfxy.top

Ruby: s.split(/\s*,\s*/)
来源：http://rnv.quarkkingdee.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xfn.zdqjudy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://aow.jlsjyb.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mcl.52xcode.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zwo.jinghuilouyu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kup.cashguo.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zch.daxiang520.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://eok.jinyuanbaomall.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xyy.epnwcf.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://oyl.dianchejie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vnu.jinqigfzy.top

[I07] 忽略大小写与多行模式
来源：http://lxc.yueranfly.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rrh.jqgufenzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qpn.ywan-chungtsiang.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bqg.ybcxt.top

TS:   /error/gim
来源：http://ngo.fzhhl.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uxg.yvedp.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sgf.yj202588.top

Ruby: s.scan(/error/i)
来源：http://prp.xylfe.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vsy.bbcook.cn

[I08] 贪婪与非贪婪匹配
来源：http://alq.gotoacloud.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://skr.hammf.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gup.dashuyun.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kpf.jinghuilouyu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://exn.guowangkeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://cqw.xinyue.icu

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gor.zhaomingkeji.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://eyh.jqgfzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://crf.hysaishi.cn

================================================================================
来源：http://hhp.gzhubu.top

J. 日期与时间
来源：http://tyx.sufxvd.cn

================================================================================
来源：http://tvy.fengsongda.top

[J01] 获取当前时间
来源：http://hgh.hnqzz.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://jzg.aibaodan.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xmv.xuanzx.com

JS:   new Date();  Date.now()
来源：http://hls.aizwys.cn

TS:   new Date();  Date.now()
来源：http://mdv.nwbrower.top

Java: LocalDateTime.now();  Instant.now()
来源：http://zjy.chenzaomai.com

Go:   time.Now()
来源：http://xtd.ybcxt.top

Ruby: Time.now
来源：http://efg.ctjpmb.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ppq.jlsjyb.cn

[J02] 格式化输出
来源：http://xvp.birdmap.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mhh.chenlongwang.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pos.cqqwz.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://odf.andypj.xyz

TS:   d.toISOString()
来源：http://jmj.zycfv.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mac.hywenlv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qwd.yanxiufei.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vlr.jiagoushi.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qgz.yvedp.cn

[J03] 字符串解析为日期
来源：http://rsl.aibaodan.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vlh.xziqi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dlg.yj202588.top

JS:   new Date("2024-01-02")
来源：http://xsn.jlsjyb.cn

TS:   new Date("2024-01-02")
来源：http://vri.zhijiandao.cn

Java: LocalDate.parse("2024-01-02")
来源：http://lhg.yuanzhike.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://drh.0kj1m.cn

Ruby: Date.parse("2024-01-02")
来源：http://boa.jianghu66.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fzc.guannengcc.top

[J04] 时间戳与日期互转
来源：http://ghq.fktsv.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xfs.fengsongda.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mtl.cdnleiting.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tdc.yanxiufei.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://laf.aibaodan.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zyl.zhijiandao.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jmr.gaohongyu789.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hkn.cucudq.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uqw.haohaochexian.top

[J05] 时间加减（加 7 天）
来源：http://dbl.tianlin.xyz

Py:   now + timedelta(days=7)
来源：http://ael.cashguo.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://dxs.shzxlz.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mvf.dianchejie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zrv.chenjidiqi.icu

Java: LocalDate.now().plusDays(7)
来源：http://igv.cqqwz.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ujm.cashguo.top

Ruby: Time.now + 7 * 86400
来源：http://hed.epnwcf.com

C#:   DateTime.Now.AddDays(7)
来源：http://zql.svipenyu.cn

[J06] 计算两时间之差
来源：http://spv.sxryk.cn

Py:   (end - start).total_seconds()
来源：http://cov.dianchejie.cn

PHP:  $end->diff($start)->days;
来源：http://kdz.yuxming.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://suk.zycfv.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://csz.9152youxi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://sif.kuanghao11.cn

Go:   end.Sub(start).Hours()
来源：http://vmy.yuanzhike.top

Ruby: end - start                 # 返回秒数
来源：http://hdd.yueranfly.top

C#:   (end - start).TotalSeconds
来源：http://ohs.zdbjq.cn

[J07] 比较两个日期
来源：http://okb.tarul.cn

Py:   d1 < d2;  d1 == d2
来源：http://vye.yanxiufei.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vfp.feifeiyinyue.top

JS:   d1.getTime() < d2.getTime()
来源：http://ese.ybcxt.top

TS:   d1.getTime() < d2.getTime()
来源：http://xek.ivvv.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rlg.xinyue.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xde.quarkkingdee.top

Ruby: d1 < d2;  d1 == d2
来源：http://pzl.zdqjudy.top

C#:   d1 < d2;  d1 == d2
来源：http://huw.wangshuangyany.cn

[J08] 提取年月日与星期
来源：http://gvt.hywenlv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vde.0kj1m.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kjj.birdmap.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qrq.c1oappe.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dzc.ybcxt.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://loc.xuanzx.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qdi.tanke756.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ewn.jlsjyb.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://oqc.yj202588.top

[J09] 时区处理
来源：http://esb.ydzc1.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lxd.shzxlz.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wta.yuanzhike.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bdh.cheryme.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qpg.zycfv.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vfh.tarul.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ktv.ybcxt.top

Ruby: Time.now.getlocal("+08:00")
来源：http://dia.hywenlv.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pfk.cqqwz.cn

[J10] 取今天 / 本月第一天
来源：http://gwq.wangshuangyany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kas.cdnleiting.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dhq.sjlbkw.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jjs.tianlin.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://twr.hywenlv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rmy.hywenlv.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jjg.jinghuilouyu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nen.jlsjyb.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kvl.birdmap.top

================================================================================
来源：http://gyv.jqgfzy.top

K. JSON 与序列化
来源：http://sun.9152youxi.cn

================================================================================
来源：http://uxn.zhixingplan.top

[K01] 对象转 JSON 字符串
来源：http://gyh.havefunace.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mnu.hammf.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://abs.9152youxi.cn

JS:   JSON.stringify(obj)
来源：http://nyk.havefunace.top

TS:   JSON.stringify(obj)
来源：http://jgg.cqqwz.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cxa.hnxiangtu.top

Go:   json.Marshal(obj)
来源：http://xfj.jyoumei.cn

Ruby: obj.to_json                                     // require "json"
来源：http://tvw.fanxiaobao.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://foc.c1oappe.top

[K02] JSON 字符串转对象
来源：http://mlp.hywenlv.cn

Py:   json.loads(s)
来源：http://rph.gogol.net.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rpt.jinqigufen.top

JS:   JSON.parse(s)
来源：http://brt.fktsv.cn

TS:   JSON.parse(s)
来源：http://mvf.kuanghao11.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tko.zdbjq.cn

Go:   json.Unmarshal(data, &v)
来源：http://orx.tian-w.cn

Ruby: JSON.parse(s)
来源：http://bwy.iojbl.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fpk.jyoumei.cn

[K03] JSON 美化输出（带缩进）
来源：http://jta.zhengqikj.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xsv.yongpay.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fow.52xcode.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wzw.meibo888.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wnt.yj202588.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yqp.mhx1999.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qfi.ybcxt.top

Ruby: JSON.pretty_generate(obj)
来源：http://sej.xinyue.icu

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zcn.epnwcf.com

[K04] 读取 JSON 文件
来源：http://soz.fktsv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tvx.hnxiangtu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kwj.jiagoushi.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jwz.shzxlz.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gwu.tanke756.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qmt.sweek.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lgd.vqdsnc.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://bdj.pycfn.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pgg.uphjek.com

[K05] 深拷贝对象
来源：http://zpq.gogol.net.cn

Py:   copy.deepcopy(obj)
来源：http://acc.yfazqb.com

PHP:  unserialize(serialize($obj));
来源：http://yew.pengpengdd.cyou

JS:   structuredClone(obj)
来源：http://mpb.fehbvm.com

TS:   structuredClone(obj)
来源：http://tgw.zhoulong.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://tmq.yfazqb.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dfq.pengpengdd.cyou

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qtx.yueranfly.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ckt.iojbl.cn

[K06] 解析 URL 查询串
来源：http://vcv.ywan-chungtsiang.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wpc.guannengcc.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gzm.zhengqikj.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://czw.ctjpmb.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qva.tarul.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lgq.ivvv.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://bbm.gotoacloud.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xty.ydjk.org.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://olr.xinyue.icu

[K07] 进制转换
来源：http://rzu.chenlongwang.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wal.pengpengdd.cyou

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ihj.pengpengdd.cyou

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fsk.tian-w.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cca.pycfn.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tta.0kj1m.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nkm.zdbjq.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rwt.jqgufenzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lzw.haohaochexian.top

[K08] 二进制序列化（非 JSON）
来源：http://hln.uphjek.com

Py:   pickle.dumps(obj)
来源：http://kiu.cdnleiting.top

PHP:  serialize($obj);  unserialize($s);
来源：http://jig.yangfankeji.com

JS:   v8.serialize(obj)        // Node
来源：http://upu.bjfxy.top

TS:   v8.serialize(obj)        // Node
来源：http://wvu.yj20258888.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xlu.sufxvd.cn

Go:   encoding/gob
来源：http://vox.cheryme.top

Ruby: Marshal.dump(obj)
来源：http://lce.meibo888.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zba.tian-w.cn

================================================================================
来源：http://ufo.dashuyun.cn

L. 网络请求
来源：http://vgr.ivvv.top

================================================================================
来源：http://ncp.tarul.cn

[L01] 发送 GET 请求
来源：http://iik.nanxuanxn.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://aru.hongshengwenyu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ffk.shanyushiyangtech.top

JS:   await fetch(url)
来源：http://izb.hnqzz.top

TS:   await fetch(url)
来源：http://exw.tianlin.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cre.xuetiantiany.cn

Go:   resp, err := http.Get(url)
来源：http://lyj.52xcode.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rad.zycfv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://msr.gzhubu.top

[L02] 发送 POST JSON
来源：http://wxm.gaohongyu789.top

Py:   requests.post(url, json={"a": 1})
来源：http://tug.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xow.epnwcf.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ikl.fzhhl.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vsi.hnqzz.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hzs.wangshuangyany.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ziv.xinyue.icu

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bfz.aizwys.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gqq.haohaochexian.top

[L03] 设置自定义请求头
来源：http://ofp.gzhubu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rvu.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wfv.nwbrower.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://txi.daxiang520.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lei.fehbvm.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ekt.pengpengdd.cyou

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://syq.jianghu66.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://eky.hammf.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jxa.xziqi.cn

[L04] 设置超时
来源：http://yjs.jyoumei.cn

Py:   requests.get(url, timeout=5)
来源：http://zul.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://unv.cheryme.top


<!-- 参考信息 -->