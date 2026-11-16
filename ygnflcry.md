代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://rve.yuanzhike.top

C#:   e.Message;  e.StackTrace
来源：http://vea.bjfxy.top

[H09] 带错误码的异常
来源：http://blo.bjfxy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rzp.yvedp.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ibg.jiagoushi.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ipd.sxryk.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kcj.ctjpmb.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://eqy.uphjek.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kud.zhijiandao.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ztw.ybcxt.top

C#:   // 自定义异常类中加 Code 属性
来源：http://jdv.smart0.xyz

[H10] 资源自动释放
来源：http://pah.zhiwuduotai.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ufv.svipenyu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://per.yj20258.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vpt.zhaomingkeji.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bas.ivvv.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gch.jqgufenzy.top

Go:   defer f.Close()
来源：http://pdq.uphjek.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mmi.cdnleiting.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://syd.epnwcf.com

================================================================================
来源：http://tiu.quarkkingdee.top

I. 正则表达式
来源：http://pdj.daxiang520.top

================================================================================
来源：http://okx.zhaomingkeji.xyz

[I01] 判断是否匹配
来源：http://opk.yfazqb.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vze.dashuyun.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qib.zhoulong.xyz

JS:   /\d+/.test(s)
来源：http://jem.guowangkeji.top

TS:   /\d+/.test(s)
来源：http://tij.xylfe.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://iur.daxiang520.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dvh.pengpengdd.cyou

Ruby: s.match?(/\d+/)
来源：http://uxc.meibo888.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lyu.fengsongda.top

[I02] 提取所有匹配
来源：http://iyv.fzhhl.top

Py:   re.findall(r"\d+", s)
来源：http://njn.cucudq.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ewe.ppjwa.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mqy.sjlbkw.cn

TS:   s.match(/\d+/g)
来源：http://fzo.hnxiangtu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://krm.yuxming.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://atz.jqgufenzy.top

Ruby: s.scan(/\d+/)
来源：http://gbo.hnxiangtu.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rbw.mhx1999.top

[I03] 提取捕获分组
来源：http://kok.xuetiantiany.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xnb.52xcode.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://szt.yvedp.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zqo.mhx1999.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://neb.hesvh.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://krz.zhengqikj.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bgi.nanxuanxn.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ebp.haohaochexian.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wqm.gotoacloud.top

[I04] 正则替换
来源：http://sbt.ywan-chungtsiang.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ide.jyoumei.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://knj.andypj.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://sdq.snrcjt.cn

TS:   s.replace(/\d+/g, "#")
来源：http://pco.zycfv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://nbv.shangyingyoupin.top

Go:   re.ReplaceAllString(s, "#")
来源：http://jwk.fehbvm.com

Ruby: s.gsub(/\d+/, "#")
来源：http://azb.zdbjq.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tco.jianghu66.top

[I05] 按正则拆分
来源：http://fcn.9152youxi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://vvo.shuidangran.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qxi.cdnleiting.top

JS:   s.split(/\s*,\s*/)
来源：http://suf.yueranfly.top

TS:   s.split(/\s*,\s*/)
来源：http://rbm.iojbl.cn

Java: s.split("\\s*,\\s*")
来源：http://kvn.svipenyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kfn.yj20258.top

Ruby: s.split(/\s*,\s*/)
来源：http://cwp.ydzc1.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kbj.jqgufenzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ehx.0kj1m.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mke.feifeiyinyue.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ghk.dashuyun.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yaf.sxryk.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dpb.havefunace.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zzt.nanxuanxn.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zhs.tian-w.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vhy.chenjidiqi.icu

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bop.cqqwz.cn

[I07] 忽略大小写与多行模式
来源：http://cnz.mhx1999.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xcm.cashguo.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bpj.jinyuanbaomall.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://aga.tian-w.cn

TS:   /error/gim
来源：http://nlp.jinqigufen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dwi.andypj.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://htl.sxryk.cn

Ruby: s.scan(/error/i)
来源：http://fyq.cheryme.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rww.ehwqpu.com

[I08] 贪婪与非贪婪匹配
来源：http://iyt.cucudq.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oht.tarul.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sut.c1oappe.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mgm.zhijiandao.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vby.quarkkingdee.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://qzz.jqgufenzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mzo.sjlbkw.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://eej.aizwys.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lya.cqqwz.cn

================================================================================
来源：http://xlx.nwbrower.top

J. 日期与时间
来源：http://ahg.zhiwuduotai.top

================================================================================
来源：http://ihy.feifeiyinyue.top

[J01] 获取当前时间
来源：http://vji.jinyuanbaomall.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lml.svipenyu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yug.xuanzx.com

JS:   new Date();  Date.now()
来源：http://jvo.havefunace.top

TS:   new Date();  Date.now()
来源：http://pft.yj20258888.top

Java: LocalDateTime.now();  Instant.now()
来源：http://xav.tian-w.cn

Go:   time.Now()
来源：http://wqz.yvedp.cn

Ruby: Time.now
来源：http://fwu.yuanzhike.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nox.uphjek.com

[J02] 格式化输出
来源：http://ooc.zhijiandao.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://chk.vehdjk.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hlv.hywenlv.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ziy.gaohongyu789.top

TS:   d.toISOString()
来源：http://sid.chenjidiqi.icu

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ebi.zhixingplan.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ntt.gogol.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ixn.fanxiaobao.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ugj.shanyushiyangtech.top

[J03] 字符串解析为日期
来源：http://ogw.yvedp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://upf.birdmap.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://net.sysykeji.top

JS:   new Date("2024-01-02")
来源：http://pzt.jyoumei.cn

TS:   new Date("2024-01-02")
来源：http://csy.zhongyouzk.top

Java: LocalDate.parse("2024-01-02")
来源：http://rkt.jinyuanbaomall.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rhb.hcnkem.com

Ruby: Date.parse("2024-01-02")
来源：http://vay.316326.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://krv.ydzc1.top

[J04] 时间戳与日期互转
来源：http://uqt.zdqjudy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rsk.guowangkeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cgz.xuetiantiany.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wns.jinghuilouyu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vkj.xylfe.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pvo.sysykeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mbf.wangshuangyany.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fvb.fengsongda.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hru.chenzaomai.com

[J05] 时间加减（加 7 天）
来源：http://cpa.shanyushiyangtech.top

Py:   now + timedelta(days=7)
来源：http://vrt.quarkkingdee.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://lvq.xziqi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lym.kuanghao11.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jsf.jinqigfzy.top

Java: LocalDate.now().plusDays(7)
来源：http://qre.zhaomingkeji.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dbx.zhiwuduotai.top

Ruby: Time.now + 7 * 86400
来源：http://krm.guowangkeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://dnb.hammf.cn

[J06] 计算两时间之差
来源：http://pdm.cheryme.top

Py:   (end - start).total_seconds()
来源：http://xld.xylfe.cn

PHP:  $end->diff($start)->days;
来源：http://ejq.meibo888.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nka.fzhhl.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tog.pengpengdd.cyou

Java: Duration.between(start, end).toSeconds()
来源：http://aji.hongshengwenyu.top

Go:   end.Sub(start).Hours()
来源：http://lyr.sweek.top

Ruby: end - start                 # 返回秒数
来源：http://aex.gaohongyu789.top

C#:   (end - start).TotalSeconds
来源：http://kie.dashuyun.cn

[J07] 比较两个日期
来源：http://jfg.chenlongwang.top

Py:   d1 < d2;  d1 == d2
来源：http://jjx.ydzc1.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nje.hongshengwenyu.top

JS:   d1.getTime() < d2.getTime()
来源：http://aiw.pycfn.com

TS:   d1.getTime() < d2.getTime()
来源：http://osl.dashuyun.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ozt.hfpthk.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pxr.snrcjt.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kla.sweek.top

C#:   d1 < d2;  d1 == d2
来源：http://qjn.jyoumei.cn

[J08] 提取年月日与星期
来源：http://fkg.hywenlv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lzl.gotoacloud.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nvx.jinghuilouyu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rel.hnxiangtu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dpe.mhx1999.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ftx.kuanghao11.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://obi.yj202588.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gly.iojbl.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wei.jqgufenzy.top

[J09] 时区处理
来源：http://fgu.yuanzhike.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mux.haohaochexian.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fpq.yfazqb.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://crx.vehdjk.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xgc.xylfe.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pmp.yonumen.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://shm.sufxvd.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://olb.xingfuxueyuan.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vki.sufxvd.cn

[J10] 取今天 / 本月第一天
来源：http://kln.316326.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://nsa.pengpengdd.cyou

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tdl.shzxlz.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rya.aibaodan.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://thw.nanxinkj.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://inb.mhx1999.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://brm.fanxiaobao.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://aae.c1oappe.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dxu.pengpengdd.cyou

================================================================================
来源：http://pdb.hcnkem.com

K. JSON 与序列化
来源：http://cug.shuidangran.top

================================================================================
来源：http://alt.shzxlz.cn

[K01] 对象转 JSON 字符串
来源：http://zpe.shangyingyoupin.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jsk.jianghu66.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xhq.nanxinkj.top

JS:   JSON.stringify(obj)
来源：http://kfe.quarkkingdee.top

TS:   JSON.stringify(obj)
来源：http://pmx.fzhhl.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fav.zhijiandao.cn

Go:   json.Marshal(obj)
来源：http://zcd.daxiang520.top

Ruby: obj.to_json                                     // require "json"
来源：http://mye.shuidangran.top

C#:   JsonSerializer.Serialize(obj)
来源：http://dcx.shanyushiyangkeji.top

[K02] JSON 字符串转对象
来源：http://mkm.hammf.cn

Py:   json.loads(s)
来源：http://iuz.hywenlv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ecn.ctjpmb.com

JS:   JSON.parse(s)
来源：http://ovt.gotoacloud.top

TS:   JSON.parse(s)
来源：http://rzc.gotoacloud.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rhz.xylfe.cn

Go:   json.Unmarshal(data, &v)
来源：http://qcv.ppjwa.cn

Ruby: JSON.parse(s)
来源：http://uft.gogol.net.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nba.yuanzhike.top

[K03] JSON 美化输出（带缩进）
来源：http://scp.ydzc1.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cnx.bbcook.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://twd.shzxlz.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://sbs.jqgfzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://gvj.jinqigufen.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ues.nanxinkj.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hpv.havefunace.top

Ruby: JSON.pretty_generate(obj)
来源：http://ypu.daria6918.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vur.aizwys.cn

[K04] 读取 JSON 文件
来源：http://sqy.sysykeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xxh.dashuyun.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xaa.yvedp.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://irq.xuanzx.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pic.tianlin.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cgc.yuanzhike.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lje.xziqi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://iny.nwbrower.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hqp.c1oappe.top

[K05] 深拷贝对象
来源：http://rpl.shuidangran.top

Py:   copy.deepcopy(obj)
来源：http://jxx.zdqjudy.top

PHP:  unserialize(serialize($obj));
来源：http://haa.hnqzz.top

JS:   structuredClone(obj)
来源：http://tjk.chenjidiqi.icu

TS:   structuredClone(obj)
来源：http://ruc.ctjpmb.com

Java: // 手写拷贝构造，或序列化往返
来源：http://vup.xinyue.icu

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xbs.yonumen.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vfp.jyoumei.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://sei.sufxvd.cn

[K06] 解析 URL 查询串
来源：http://tif.tarul.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vxu.snrcjt.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yjf.guowangkeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://elv.shzxlz.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wzc.redwolf501.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wvh.fehbvm.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://qbq.yj20258888.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://alc.epnwcf.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://trr.chenlongwang.top

[K07] 进制转换
来源：http://uki.jqgufenzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vkd.vqdsnc.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kgf.yvedp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xgs.cqqwz.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qmw.nwbrower.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hhd.havefunace.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ppg.sufxvd.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://evo.guowangkeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vgy.sysykeji.top

[K08] 二进制序列化（非 JSON）
来源：http://ccq.ywan-chungtsiang.top

Py:   pickle.dumps(obj)
来源：http://vem.316326.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://ynj.yvedp.cn

JS:   v8.serialize(obj)        // Node
来源：http://tla.9152youxi.cn

TS:   v8.serialize(obj)        // Node
来源：http://dqa.52xcode.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wts.zhongyouzk.top

Go:   encoding/gob
来源：http://nad.epnwcf.com

Ruby: Marshal.dump(obj)
来源：http://bcg.dianchejie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kec.gzhubu.top

================================================================================
来源：http://ulq.gotoacloud.top

L. 网络请求
来源：http://hay.jinqigufen.top

================================================================================
来源：http://pqz.quarkkingdee.top

[L01] 发送 GET 请求
来源：http://rpo.ppjwa.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wsz.dianchejie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rbx.xziqi.cn

JS:   await fetch(url)
来源：http://cqx.xziqi.cn

TS:   await fetch(url)
来源：http://wgz.fzhhl.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vwf.xingfuxueyuan.xyz

Go:   resp, err := http.Get(url)
来源：http://jmy.dashuyun.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dyq.ywan-chungtsiang.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kud.dashuyun.cn

[L02] 发送 POST JSON
来源：http://aot.yongpay.top

Py:   requests.post(url, json={"a": 1})
来源：http://zvs.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://apx.jianghu66.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rzz.zhiwuduotai.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lwb.chenzaomai.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vrb.shuidangran.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://okj.yongpay.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vkc.xuetiantiany.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ufy.yangfankeji.com

[L03] 设置自定义请求头
来源：http://zrl.hesvh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qxe.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cts.fanxiaobao.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vsv.hongshengwenyu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pjb.xuanzx.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ulh.shanyushiyangtech.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://myk.svipenyu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://efk.yfazqb.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://egr.sxryk.cn

[L04] 设置超时
来源：http://oso.yueranfly.top

Py:   requests.get(url, timeout=5)
来源：http://jdd.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zge.yuanzhike.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xyc.fanxiaobao.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qxd.tianlin.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jpa.svipenyu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lka.jinqigfzy.top


<!-- 参考信息 -->