代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://cpb.sysykeji.top

[H08] 获取错误信息与堆栈
来源：http://dvs.ybcxt.top

Py:   str(e);  traceback.format_exc()
来源：http://bro.52xcode.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://whd.jinghuilouyu.cn

JS:   e.message;  e.stack
来源：http://fvi.hammf.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://emk.mhx1999.top

Java: e.getMessage();  e.printStackTrace()
来源：http://rvi.hysaishi.cn

Go:   err.Error()
来源：http://fvm.fzhhl.top

Ruby: e.message;  e.backtrace
来源：http://lly.xuetiantiany.cn

C#:   e.Message;  e.StackTrace
来源：http://ism.yj20258.top

[H09] 带错误码的异常
来源：http://syp.shangyingyoupin.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zxs.ywan-chungtsiang.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://euy.zhixingplan.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pte.yanxiufei.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://okc.redwolf501.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pxc.ppjwa.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fvi.52xcode.cn

Ruby: raise MyError.new("fail", 500)
来源：http://kgd.hcnkem.com

C#:   // 自定义异常类中加 Code 属性
来源：http://kvk.dashuyun.cn

[H10] 资源自动释放
来源：http://uzv.birdmap.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://uek.gotoacloud.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qgx.jlsjyb.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ovq.uphjek.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://myi.hnxiangtu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bmp.gotoacloud.top

Go:   defer f.Close()
来源：http://jhn.wangdashe.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bmg.chenjidiqi.icu

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gjc.ctjpmb.com

================================================================================
来源：http://ocr.daria6918.cn

I. 正则表达式
来源：http://pft.aizwys.cn

================================================================================
来源：http://bts.cheryme.top

[I01] 判断是否匹配
来源：http://zte.xziqi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ukg.birdmap.top

PHP:  preg_match('/\d+/', $s);
来源：http://lha.vehdjk.com

JS:   /\d+/.test(s)
来源：http://uqu.yongpay.top

TS:   /\d+/.test(s)
来源：http://fgg.sufxvd.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xyf.chenzaomai.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gdx.hongshengwenyu.top

Ruby: s.match?(/\d+/)
来源：http://rat.yvedp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://evc.pengpengdd.cyou

[I02] 提取所有匹配
来源：http://pqh.iojbl.cn

Py:   re.findall(r"\d+", s)
来源：http://vcr.yvedp.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tqq.hcnkem.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://srt.sweek.top

TS:   s.match(/\d+/g)
来源：http://whk.wangdashe.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bgl.cashguo.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://afv.shanyushiyangtech.top

Ruby: s.scan(/\d+/)
来源：http://lbj.hongshengwenyu.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bhg.andypj.xyz

[I03] 提取捕获分组
来源：http://mgn.jinyuanbaomall.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://iml.jqgfzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zox.cdnleiting.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yli.zdqjudy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qdp.zycfv.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bzi.vehdjk.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wkl.jyoumei.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hod.aibaodan.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vev.xinyue.icu

[I04] 正则替换
来源：http://elg.andypj.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://vil.ydjk.org.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://aur.hesvh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kye.xuetiantiany.cn

TS:   s.replace(/\d+/g, "#")
来源：http://owh.kuanghao11.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wpc.jyoumei.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xfr.hcnkem.com

Ruby: s.gsub(/\d+/, "#")
来源：http://tvv.yj20258.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://skb.ydzc1.top

[I05] 按正则拆分
来源：http://gaa.fktsv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ofi.havefunace.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dst.chenjidiqi.icu

JS:   s.split(/\s*,\s*/)
来源：http://pzm.bjfxy.top

TS:   s.split(/\s*,\s*/)
来源：http://kyk.cheryme.top

Java: s.split("\\s*,\\s*")
来源：http://gww.yangfankeji.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ddo.tanke756.top

Ruby: s.split(/\s*,\s*/)
来源：http://woc.tarul.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://eoc.aibaodan.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://umm.havefunace.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dfy.hysaishi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tzl.cqqwz.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uii.pycfn.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rwv.gogol.net.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yoh.gzhubu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tsp.chenjidiqi.icu

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vrj.fktsv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vzm.jqgufenzy.top

[I07] 忽略大小写与多行模式
来源：http://met.cheryme.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://oet.hywenlv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jvv.fehbvm.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ggs.feifeiyinyue.top

TS:   /error/gim
来源：http://quo.zdbjq.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vnh.sjlbkw.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zle.hesvh.cn

Ruby: s.scan(/error/i)
来源：http://zeb.jqgfzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kgn.mhx1999.top

[I08] 贪婪与非贪婪匹配
来源：http://jos.sufxvd.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kxi.guannengcc.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nut.yvedp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ljx.ybcxt.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://emj.hfpthk.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://kvv.jyoumei.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nbr.tarul.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fqn.quarkkingdee.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zoj.sysykeji.top

================================================================================
来源：http://gkl.kuanghao11.cn

J. 日期与时间
来源：http://uue.hnxiangtu.top

================================================================================
来源：http://pad.zhijiandao.cn

[J01] 获取当前时间
来源：http://mpc.tanke756.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://doe.jinqigufen.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://onm.yuanzhike.top

JS:   new Date();  Date.now()
来源：http://owg.epnwcf.com

TS:   new Date();  Date.now()
来源：http://zuo.shanyushiyangtech.top

Java: LocalDateTime.now();  Instant.now()
来源：http://hgr.ehwqpu.com

Go:   time.Now()
来源：http://uzy.tian-w.cn

Ruby: Time.now
来源：http://bdo.jqgufenzy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://llp.shuidangran.top

[J02] 格式化输出
来源：http://cbl.cashguo.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lde.c1oappe.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://oro.tianlin.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jvs.yuxming.cn

TS:   d.toISOString()
来源：http://czu.316326.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nsd.smart0.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rbc.tarul.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hfc.zdqjudy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pph.xingfuxueyuan.xyz

[J03] 字符串解析为日期
来源：http://qqa.xuetiantiany.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gia.xziqi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rwq.shzxlz.cn

JS:   new Date("2024-01-02")
来源：http://qdv.shanyushiyangtech.top

TS:   new Date("2024-01-02")
来源：http://ugn.tian-w.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hos.zycfv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ojb.hammf.cn

Ruby: Date.parse("2024-01-02")
来源：http://nky.birdmap.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vym.hesvh.cn

[J04] 时间戳与日期互转
来源：http://izw.guannengcc.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zwp.ybcxt.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zcx.xylfe.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jpo.zhoulong.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://dcg.ctjpmb.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ffv.birdmap.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cka.hfpthk.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pzm.kuanghao11.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rzm.xylfe.cn

[J05] 时间加减（加 7 天）
来源：http://uob.kuanghao11.cn

Py:   now + timedelta(days=7)
来源：http://sij.gogol.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://iau.hfpthk.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bbj.52xcode.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cfw.uphjek.com

Java: LocalDate.now().plusDays(7)
来源：http://aoh.vqdsnc.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jgj.nanxinkj.top

Ruby: Time.now + 7 * 86400
来源：http://sqj.chenzaomai.com

C#:   DateTime.Now.AddDays(7)
来源：http://ndn.meibo888.top

[J06] 计算两时间之差
来源：http://gni.sysykeji.top

Py:   (end - start).total_seconds()
来源：http://jlv.shuidangran.top

PHP:  $end->diff($start)->days;
来源：http://hps.yangfankeji.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ptu.mhx1999.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ner.pengpengdd.cyou

Java: Duration.between(start, end).toSeconds()
来源：http://zhq.hesvh.cn

Go:   end.Sub(start).Hours()
来源：http://jgw.xinyue.icu

Ruby: end - start                 # 返回秒数
来源：http://ysy.ppjwa.cn

C#:   (end - start).TotalSeconds
来源：http://xfi.zhengqikj.top

[J07] 比较两个日期
来源：http://iqs.tarul.cn

Py:   d1 < d2;  d1 == d2
来源：http://inb.zhongyouzk.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ocx.tian-w.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ksq.hcnkem.com

TS:   d1.getTime() < d2.getTime()
来源：http://wcl.yongpay.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://etm.ydjk.org.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tsz.guannengcc.top

Ruby: d1 < d2;  d1 == d2
来源：http://gqj.hysaishi.cn

C#:   d1 < d2;  d1 == d2
来源：http://dfo.zhiwuduotai.top

[J08] 提取年月日与星期
来源：http://chv.yj202588.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://puj.zhengqikj.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tga.vqdsnc.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nlj.ctjpmb.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ukz.yvedp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bdw.yj202588.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gye.svipenyu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hgy.xuetiantiany.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://oaz.cheryme.top

[J09] 时区处理
来源：http://gmx.nanxuanxn.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nww.zdbjq.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ujs.yanxiufei.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lns.zhengqikj.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rgn.yuanzhike.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gas.jinqigufen.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ddg.shuidangran.top

Ruby: Time.now.getlocal("+08:00")
来源：http://fvj.316326.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://luo.cashguo.top

[J10] 取今天 / 本月第一天
来源：http://znq.fengsongda.top

Py:   date.today();  date.today().replace(day=1)
来源：http://sgm.jinqigufen.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vhk.aizwys.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://edi.tian-w.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://eyc.meibo888.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gnh.sxryk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uzn.xingfuxueyuan.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pdx.tarul.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gfn.zycfv.cn

================================================================================
来源：http://wog.yfazqb.com

K. JSON 与序列化
来源：http://ruk.shanyushiyangkeji.top

================================================================================
来源：http://osh.quarkkingdee.top

[K01] 对象转 JSON 字符串
来源：http://maa.zycfv.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lmn.vehdjk.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fez.hfpthk.cn

JS:   JSON.stringify(obj)
来源：http://hyv.havefunace.top

TS:   JSON.stringify(obj)
来源：http://doe.ehwqpu.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://msc.sxryk.cn

Go:   json.Marshal(obj)
来源：http://bjl.tianlin.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://uyt.hnqzz.top

C#:   JsonSerializer.Serialize(obj)
来源：http://loc.snrcjt.cn

[K02] JSON 字符串转对象
来源：http://lla.sufxvd.cn

Py:   json.loads(s)
来源：http://ciu.jlsjyb.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://eob.hfpthk.cn

JS:   JSON.parse(s)
来源：http://kvu.iojbl.cn

TS:   JSON.parse(s)
来源：http://ojn.haohaochexian.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yue.ydjk.org.cn

Go:   json.Unmarshal(data, &v)
来源：http://zdr.jinghuilouyu.cn

Ruby: JSON.parse(s)
来源：http://vyc.aizwys.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wbv.gogol.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://skp.cdnleiting.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jhz.quarkkingdee.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hoa.aizwys.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ond.meibo888.top

TS:   JSON.stringify(obj, null, 2)
来源：http://hus.vehdjk.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wil.cqqwz.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cbj.hammf.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vtx.meibo888.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bex.redwolf501.top

[K04] 读取 JSON 文件
来源：http://dlx.iojbl.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cjv.jyoumei.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uzz.yongpay.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gmu.bbcook.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vma.gogol.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://onm.xziqi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uda.hcnkem.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://jct.aizwys.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qcz.dianchejie.cn

[K05] 深拷贝对象
来源：http://xyf.smart0.xyz

Py:   copy.deepcopy(obj)
来源：http://suw.chenjidiqi.icu

PHP:  unserialize(serialize($obj));
来源：http://vxn.bbcook.cn

JS:   structuredClone(obj)
来源：http://ucv.haohaochexian.top

TS:   structuredClone(obj)
来源：http://qbs.zhijiandao.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vpu.epnwcf.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kod.yj202588.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zrr.ybcxt.top

C#:   // 序列化往返，或自定义 Clone
来源：http://szg.316326.xyz

[K06] 解析 URL 查询串
来源：http://poz.fehbvm.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ggs.jqgufenzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xcp.sufxvd.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xzg.cqqwz.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qsc.c1oappe.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kpe.sweek.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://puq.ehwqpu.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vmu.yfazqb.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vvn.yvedp.cn

[K07] 进制转换
来源：http://sjh.shanyushiyangkeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sav.tianlin.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gjt.shangyingyoupin.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://khq.chenlongwang.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dja.bjfxy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cfk.xuetiantiany.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bak.cqqwz.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ibj.tianlin.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://isj.zhijiandao.cn

[K08] 二进制序列化（非 JSON）
来源：http://qwd.0kj1m.cn

Py:   pickle.dumps(obj)
来源：http://zqg.ppjwa.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wli.zhongyouzk.top

JS:   v8.serialize(obj)        // Node
来源：http://idj.epnwcf.com

TS:   v8.serialize(obj)        // Node
来源：http://ygg.xuetiantiany.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wic.yj20258.top

Go:   encoding/gob
来源：http://rng.havefunace.top

Ruby: Marshal.dump(obj)
来源：http://xcv.fzhhl.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tls.sxryk.cn

================================================================================
来源：http://eqc.andypj.xyz

L. 网络请求
来源：http://gkf.zdqjudy.top

================================================================================
来源：http://fwz.hywenlv.cn

[L01] 发送 GET 请求
来源：http://hhq.sweek.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pzw.chenzaomai.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gde.ybcxt.top

JS:   await fetch(url)
来源：http://dxh.yj20258.top

TS:   await fetch(url)
来源：http://cuy.meibo888.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nqw.yonumen.top

Go:   resp, err := http.Get(url)
来源：http://gky.yangfankeji.com

Ruby: Net::HTTP.get(URI(url))
来源：http://lbf.cashguo.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fit.ydjk.org.cn

[L02] 发送 POST JSON
来源：http://myb.gzhubu.top

Py:   requests.post(url, json={"a": 1})
来源：http://gfy.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://oxk.zdqjudy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kjb.sweek.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gde.hnxiangtu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lid.birdmap.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://imr.fengsongda.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qjw.316326.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xyc.sxryk.cn

[L03] 设置自定义请求头
来源：http://bsa.shangyingyoupin.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yye.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yfn.yj20258888.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hmp.yongpay.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ffo.vqdsnc.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tnt.meibo888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ace.tarul.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dlh.shanyushiyangkeji.top


<!-- 参考信息 -->