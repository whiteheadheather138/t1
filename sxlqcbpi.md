代发 wailian999

JS:   e.message;  e.stack
来源：http://ghl.xinyue.icu

TS:   e instanceof Error ? e.message : String(e)
来源：http://akc.yj20258888.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ugh.shzxlz.cn

Go:   err.Error()
来源：http://bbj.cucudq.cn

Ruby: e.message;  e.backtrace
来源：http://guc.cucudq.cn

C#:   e.Message;  e.StackTrace
来源：http://qtp.shanyushiyangtech.top

[H09] 带错误码的异常
来源：http://zyv.smart0.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xpg.cdnleiting.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://hei.fktsv.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sxj.sxryk.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bcf.birdmap.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ykn.yuxming.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zuz.jinghuilouyu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zao.hesvh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://jtp.cqqwz.cn

[H10] 资源自动释放
来源：http://akw.ehwqpu.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://cdn.bjfxy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://guv.yuxming.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tmp.jiagoushi.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tcw.cdnleiting.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://klv.jqgufenzy.top

Go:   defer f.Close()
来源：http://zax.hysaishi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ffs.yuanzhike.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ume.wangdashe.top

================================================================================
来源：http://nze.pengpengdd.cyou

I. 正则表达式
来源：http://tve.xuetiantiany.cn

================================================================================
来源：http://aaf.ehwqpu.com

[I01] 判断是否匹配
来源：http://fjo.gzhubu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ktx.hcnkem.com

PHP:  preg_match('/\d+/', $s);
来源：http://qqc.chenlongwang.top

JS:   /\d+/.test(s)
来源：http://krv.dianchejie.cn

TS:   /\d+/.test(s)
来源：http://uat.daxiang520.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zfj.jinqigufen.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://owm.vqdsnc.cn

Ruby: s.match?(/\d+/)
来源：http://qyu.uphjek.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gyc.meibo888.top

[I02] 提取所有匹配
来源：http://gql.jianghu66.top

Py:   re.findall(r"\d+", s)
来源：http://kgl.9152youxi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qmz.cdnleiting.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://iqx.cdnleiting.top

TS:   s.match(/\d+/g)
来源：http://ocp.c1oappe.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://egj.wangdashe.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ozn.zycfv.cn

Ruby: s.scan(/\d+/)
来源：http://fcn.ydjk.org.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wmg.svipenyu.cn

[I03] 提取捕获分组
来源：http://apx.ywan-chungtsiang.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ead.fehbvm.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://szs.zhongyouzk.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gxp.jyoumei.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uxs.jinghuilouyu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://awi.jqgfzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://chg.nanxinkj.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wkz.pengpengdd.cyou

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qou.shuidangran.top

[I04] 正则替换
来源：http://gdt.zhiwuduotai.top

Py:   re.sub(r"\d+", "#", s)
来源：http://erz.yonumen.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zut.yfazqb.com

JS:   s.replace(/\d+/g, "#")
来源：http://niv.ywan-chungtsiang.top

TS:   s.replace(/\d+/g, "#")
来源：http://isi.zhoulong.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://wqi.yuxming.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gtr.cheryme.top

Ruby: s.gsub(/\d+/, "#")
来源：http://dea.ctjpmb.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bjh.fzhhl.top

[I05] 按正则拆分
来源：http://meu.jianghu66.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ezv.xylfe.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lds.yj20258.top

JS:   s.split(/\s*,\s*/)
来源：http://jfa.fengsongda.top

TS:   s.split(/\s*,\s*/)
来源：http://qht.dianchejie.cn

Java: s.split("\\s*,\\s*")
来源：http://nrm.birdmap.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vty.epnwcf.com

Ruby: s.split(/\s*,\s*/)
来源：http://wne.jianghu66.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vds.yuxming.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ddo.chenzaomai.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nsh.dashuyun.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nbd.chenlongwang.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hdm.chenlongwang.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xpn.daria6918.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://scf.pycfn.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nob.zhengqikj.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ues.dashuyun.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://olg.shangyingyoupin.top

[I07] 忽略大小写与多行模式
来源：http://aym.gogol.net.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lbz.9152youxi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qfx.vehdjk.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yzh.guowangkeji.top

TS:   /error/gim
来源：http://uum.zhaomingkeji.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dbg.shzxlz.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://eix.aizwys.cn

Ruby: s.scan(/error/i)
来源：http://rin.fehbvm.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qhb.hywenlv.cn

[I08] 贪婪与非贪婪匹配
来源：http://qhz.chenjidiqi.icu

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nvz.hnxiangtu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lob.cheryme.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vus.yj20258.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cct.epnwcf.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://vfd.vehdjk.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ngw.pycfn.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fiw.yvedp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nee.gzhubu.top

================================================================================
来源：http://nlv.jianghu66.top

J. 日期与时间
来源：http://ito.yonumen.top

================================================================================
来源：http://zwa.hongshengwenyu.top

[J01] 获取当前时间
来源：http://ovm.daxiang520.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://jqn.shzxlz.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jpa.hfpthk.cn

JS:   new Date();  Date.now()
来源：http://xic.kuanghao11.cn

TS:   new Date();  Date.now()
来源：http://zck.jqgfzy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://jhv.xylfe.cn

Go:   time.Now()
来源：http://abl.andypj.xyz

Ruby: Time.now
来源：http://mvr.daxiang520.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tfm.ybcxt.top

[J02] 格式化输出
来源：http://yda.yuxming.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://slc.wangdashe.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ixe.sxryk.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bnc.yj20258.top

TS:   d.toISOString()
来源：http://qjj.cqqwz.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vbd.zhijiandao.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bob.ivvv.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uuu.shzxlz.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hcx.nanxuanxn.top

[J03] 字符串解析为日期
来源：http://kke.jqgufenzy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qdb.yueranfly.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hew.tanke756.top

JS:   new Date("2024-01-02")
来源：http://eqn.jlsjyb.cn

TS:   new Date("2024-01-02")
来源：http://ixe.havefunace.top

Java: LocalDate.parse("2024-01-02")
来源：http://ctx.cashguo.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nab.cdnleiting.top

Ruby: Date.parse("2024-01-02")
来源：http://dom.hesvh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sli.jinyuanbaomall.cn

[J04] 时间戳与日期互转
来源：http://lyc.svipenyu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mjt.ctjpmb.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kcx.pengpengdd.cyou

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://czp.shangyingyoupin.top

TS:   Math.floor(Date.now() / 1000)
来源：http://dbf.zhengqikj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dus.epnwcf.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rbv.yj20258888.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xnb.gaohongyu789.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://iun.yj20258888.top

[J05] 时间加减（加 7 天）
来源：http://qmw.ctjpmb.com

Py:   now + timedelta(days=7)
来源：http://dag.xuanzx.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://jrx.fktsv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ueg.feifeiyinyue.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gfn.birdmap.top

Java: LocalDate.now().plusDays(7)
来源：http://hzb.daria6918.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ztd.aibaodan.cn

Ruby: Time.now + 7 * 86400
来源：http://mgv.cdnleiting.top

C#:   DateTime.Now.AddDays(7)
来源：http://zln.jianghu66.top

[J06] 计算两时间之差
来源：http://sif.svipenyu.cn

Py:   (end - start).total_seconds()
来源：http://xug.kuanghao11.cn

PHP:  $end->diff($start)->days;
来源：http://mvk.cashguo.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fmb.pycfn.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://epw.jlsjyb.cn

Java: Duration.between(start, end).toSeconds()
来源：http://cte.jyoumei.cn

Go:   end.Sub(start).Hours()
来源：http://iop.feifeiyinyue.top

Ruby: end - start                 # 返回秒数
来源：http://kyn.0kj1m.cn

C#:   (end - start).TotalSeconds
来源：http://mxc.yanxiufei.cn

[J07] 比较两个日期
来源：http://dmg.yueranfly.top

Py:   d1 < d2;  d1 == d2
来源：http://neh.hnxiangtu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cfo.fanxiaobao.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://hek.uphjek.com

TS:   d1.getTime() < d2.getTime()
来源：http://zwz.hesvh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ohg.birdmap.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://omx.jinyuanbaomall.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xqy.bjfxy.top

C#:   d1 < d2;  d1 == d2
来源：http://ikv.xinyue.icu

[J08] 提取年月日与星期
来源：http://aec.shanyushiyangkeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://oeq.zhongyouzk.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://odb.hywenlv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://woq.xinyue.icu

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://skl.ehwqpu.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://awh.yvedp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tag.gzhubu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://euu.yfazqb.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sql.nanxinkj.top

[J09] 时区处理
来源：http://ftk.yj20258.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tpv.jinqigufen.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lxr.guowangkeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yav.gotoacloud.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://emp.yj202588.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://udc.ivvv.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nsy.vehdjk.com

Ruby: Time.now.getlocal("+08:00")
来源：http://aen.fanxiaobao.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xnk.wangdashe.top

[J10] 取今天 / 本月第一天
来源：http://mrl.jinqigufen.top

Py:   date.today();  date.today().replace(day=1)
来源：http://mjb.zhaomingkeji.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ult.shanyushiyangtech.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rmw.gogol.net.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://djf.vehdjk.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wvl.pycfn.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dnk.yj202588.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mvt.c1oappe.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bia.9152youxi.cn

================================================================================
来源：http://ysg.epnwcf.com

K. JSON 与序列化
来源：http://iiy.jyoumei.cn

================================================================================
来源：http://czf.jinqigufen.top

[K01] 对象转 JSON 字符串
来源：http://ndq.pycfn.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mkf.xuanzx.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mzh.bjfxy.top

JS:   JSON.stringify(obj)
来源：http://csd.jiagoushi.top

TS:   JSON.stringify(obj)
来源：http://jxq.guowangkeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://obk.gaohongyu789.top

Go:   json.Marshal(obj)
来源：http://eaf.jinyuanbaomall.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ovq.ppjwa.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://eil.pengpengdd.cyou

[K02] JSON 字符串转对象
来源：http://lyo.pengpengdd.cyou

Py:   json.loads(s)
来源：http://dhx.c1oappe.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pcb.yonumen.top

JS:   JSON.parse(s)
来源：http://oka.yvedp.cn

TS:   JSON.parse(s)
来源：http://cus.wangdashe.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qbo.chenlongwang.top

Go:   json.Unmarshal(data, &v)
来源：http://ubf.daxiang520.top

Ruby: JSON.parse(s)
来源：http://hxp.dianchejie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pxf.hcnkem.com

[K03] JSON 美化输出（带缩进）
来源：http://dyd.cucudq.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://udy.xuetiantiany.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mpx.vqdsnc.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://whv.xingfuxueyuan.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://qhm.kuanghao11.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hrh.fzhhl.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qgj.xylfe.cn

Ruby: JSON.pretty_generate(obj)
来源：http://abs.hysaishi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rmd.yj20258888.top

[K04] 读取 JSON 文件
来源：http://xrr.yuxming.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://klp.jianghu66.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tvy.fengsongda.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lsx.52xcode.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://erb.316326.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qhq.guannengcc.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vyj.ctjpmb.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://cai.c1oappe.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gtn.yanxiufei.cn

[K05] 深拷贝对象
来源：http://vqg.hfpthk.cn

Py:   copy.deepcopy(obj)
来源：http://bps.jinqigufen.top

PHP:  unserialize(serialize($obj));
来源：http://mhz.xziqi.cn

JS:   structuredClone(obj)
来源：http://xij.tarul.cn

TS:   structuredClone(obj)
来源：http://cmi.yuanzhike.top

Java: // 手写拷贝构造，或序列化往返
来源：http://foi.jinqigufen.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uea.yuxming.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jyu.hnxiangtu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://mfw.yuxming.cn

[K06] 解析 URL 查询串
来源：http://yuf.vqdsnc.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fnz.hnqzz.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wbd.sysykeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zql.jlsjyb.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rdf.yueranfly.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hah.316326.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://yts.zhengqikj.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wlb.sxryk.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hol.iojbl.cn

[K07] 进制转换
来源：http://mpw.hnxiangtu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dsz.quarkkingdee.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://stz.haohaochexian.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yup.jinyuanbaomall.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://umg.tian-w.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fbs.ywan-chungtsiang.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hjc.nanxuanxn.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rkx.meibo888.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qfg.zhaomingkeji.xyz

[K08] 二进制序列化（非 JSON）
来源：http://qvt.tian-w.cn

Py:   pickle.dumps(obj)
来源：http://uut.9152youxi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ywz.hywenlv.cn

JS:   v8.serialize(obj)        // Node
来源：http://xup.yj20258888.top

TS:   v8.serialize(obj)        // Node
来源：http://spi.ctjpmb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tje.yvedp.cn

Go:   encoding/gob
来源：http://nwv.9152youxi.cn

Ruby: Marshal.dump(obj)
来源：http://zrr.shuidangran.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://guq.quarkkingdee.top

================================================================================
来源：http://cil.hongshengwenyu.top

L. 网络请求
来源：http://tkp.vqdsnc.cn

================================================================================
来源：http://auz.ydzc1.top

[L01] 发送 GET 请求
来源：http://vqj.daria6918.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kfp.yvedp.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kun.chenjidiqi.icu

JS:   await fetch(url)
来源：http://krg.jianghu66.top

TS:   await fetch(url)
来源：http://aef.zdqjudy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://usq.xziqi.cn

Go:   resp, err := http.Get(url)
来源：http://pqa.uphjek.com

Ruby: Net::HTTP.get(URI(url))
来源：http://pxp.yj20258888.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uyy.vqdsnc.cn

[L02] 发送 POST JSON
来源：http://tra.zhengqikj.top

Py:   requests.post(url, json={"a": 1})
来源：http://klc.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vxr.shanyushiyangkeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ptm.andypj.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lka.kuanghao11.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ixn.jinqigufen.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qaa.zhiwuduotai.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yhm.gzhubu.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vdv.ivvv.top

[L03] 设置自定义请求头
来源：http://mly.sysykeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zet.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lwj.zhoulong.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wvk.nwbrower.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mwk.gaohongyu789.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bvq.dianchejie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://eoz.c1oappe.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://adx.chenlongwang.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mrs.fzhhl.top

[L04] 设置超时
来源：http://vyd.xingfuxueyuan.xyz

Py:   requests.get(url, timeout=5)
来源：http://igg.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dhb.gotoacloud.top


<!-- 参考信息 -->