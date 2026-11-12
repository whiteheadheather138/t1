代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://qpz.andypj.xyz

C#:   e.Message;  e.StackTrace
来源：http://qiv.wangshuangyany.cn

[H09] 带错误码的异常
来源：http://quf.ydjk.org.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zqc.yfazqb.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://qjn.pycfn.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bqs.hfpthk.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ksi.ydzc1.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zvp.yuxming.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yrh.ydjk.org.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mmu.9152youxi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xcl.wangdashe.top

[H10] 资源自动释放
来源：http://wlm.kuanghao11.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rjg.sysykeji.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vlt.guowangkeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://uop.sweek.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bat.uphjek.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://edi.jinqigfzy.top

Go:   defer f.Close()
来源：http://xaj.shangyingyoupin.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://iqm.jyoumei.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hos.cheryme.top

================================================================================
来源：http://nxg.havefunace.top

I. 正则表达式
来源：http://uhw.birdmap.top

================================================================================
来源：http://iiu.tanke756.top

[I01] 判断是否匹配
来源：http://jat.zdqjudy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://akh.jyoumei.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fdp.jiagoushi.top

JS:   /\d+/.test(s)
来源：http://nla.daxiang520.top

TS:   /\d+/.test(s)
来源：http://jiz.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://aak.iojbl.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wsc.iojbl.cn

Ruby: s.match?(/\d+/)
来源：http://hfs.gotoacloud.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tzk.hammf.cn

[I02] 提取所有匹配
来源：http://tlj.wangdashe.top

Py:   re.findall(r"\d+", s)
来源：http://xbi.tian-w.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gdp.jinqigfzy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pyk.smart0.xyz

TS:   s.match(/\d+/g)
来源：http://tkv.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xfk.yuanzhike.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uhi.zhixingplan.top

Ruby: s.scan(/\d+/)
来源：http://btw.tian-w.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lle.xuanzx.com

[I03] 提取捕获分组
来源：http://nfy.ctjpmb.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jvo.yj20258888.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vbw.jinyuanbaomall.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ffz.hnqzz.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wmw.pengpengdd.cyou

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dfy.dashuyun.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xdk.andypj.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cur.xingfuxueyuan.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://apl.kuanghao11.cn

[I04] 正则替换
来源：http://dhp.fzhhl.top

Py:   re.sub(r"\d+", "#", s)
来源：http://xfj.sweek.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kok.xingfuxueyuan.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://vhi.daria6918.cn

TS:   s.replace(/\d+/g, "#")
来源：http://man.tian-w.cn

Java: s.replaceAll("\\d+", "#")
来源：http://voz.iojbl.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qmp.cqqwz.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wkk.snrcjt.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zcr.chenjidiqi.icu

[I05] 按正则拆分
来源：http://rzw.yonumen.top

Py:   re.split(r"\s*,\s*", s)
来源：http://sss.fanxiaobao.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bhq.ydzc1.top

JS:   s.split(/\s*,\s*/)
来源：http://rau.redwolf501.top

TS:   s.split(/\s*,\s*/)
来源：http://wfv.fanxiaobao.xyz

Java: s.split("\\s*,\\s*")
来源：http://era.zhijiandao.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kii.9152youxi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://myn.daria6918.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qyp.havefunace.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kzp.hnqzz.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ikz.xinyue.icu

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zqz.haohaochexian.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wpc.zdbjq.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yks.gzhubu.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hdi.sweek.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sbv.ywan-chungtsiang.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ixx.hnxiangtu.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lhz.svipenyu.cn

[I07] 忽略大小写与多行模式
来源：http://brg.hesvh.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dyc.yj20258.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mhs.jianghu66.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oxp.epnwcf.com

TS:   /error/gim
来源：http://leg.meibo888.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lss.316326.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nzk.aibaodan.cn

Ruby: s.scan(/error/i)
来源：http://aso.shangyingyoupin.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jks.hammf.cn

[I08] 贪婪与非贪婪匹配
来源：http://zek.mhx1999.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bwm.shanyushiyangkeji.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xse.cdnleiting.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lxp.guannengcc.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rgo.hammf.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nnr.aizwys.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://oql.fzhhl.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cjb.jiagoushi.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bdc.fzhhl.top

================================================================================
来源：http://qcw.gzhubu.top

J. 日期与时间
来源：http://ydm.zhongyouzk.top

================================================================================
来源：http://ybs.hfpthk.cn

[J01] 获取当前时间
来源：http://iar.shanyushiyangtech.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://guj.shzxlz.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zoh.wangshuangyany.cn

JS:   new Date();  Date.now()
来源：http://kxj.cucudq.cn

TS:   new Date();  Date.now()
来源：http://dls.tianlin.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://crl.cqqwz.cn

Go:   time.Now()
来源：http://uwb.jinyuanbaomall.cn

Ruby: Time.now
来源：http://hoi.fehbvm.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ogq.yanxiufei.cn

[J02] 格式化输出
来源：http://eyd.hywenlv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uco.hywenlv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nuk.sxryk.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bii.birdmap.top

TS:   d.toISOString()
来源：http://iao.nwbrower.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lxf.shangyingyoupin.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kkm.xylfe.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tlw.xinyue.icu

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kbu.sufxvd.cn

[J03] 字符串解析为日期
来源：http://dgr.cucudq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gam.gzhubu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tph.nanxinkj.top

JS:   new Date("2024-01-02")
来源：http://ktj.smart0.xyz

TS:   new Date("2024-01-02")
来源：http://vhu.jinghuilouyu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://src.zhengqikj.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kbe.xingfuxueyuan.xyz

Ruby: Date.parse("2024-01-02")
来源：http://lqz.yonumen.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cer.snrcjt.cn

[J04] 时间戳与日期互转
来源：http://ked.yj20258.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wsx.shzxlz.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dnq.nwbrower.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bpp.smart0.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://dlb.zdbjq.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://njl.hongshengwenyu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vkf.hammf.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vsb.vqdsnc.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tyw.jiagoushi.top

[J05] 时间加减（加 7 天）
来源：http://kms.tarul.cn

Py:   now + timedelta(days=7)
来源：http://trj.yangfankeji.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://aku.chenlongwang.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qxh.yuxming.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jah.havefunace.top

Java: LocalDate.now().plusDays(7)
来源：http://lpj.cucudq.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vuz.ydjk.org.cn

Ruby: Time.now + 7 * 86400
来源：http://fbm.snrcjt.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dxh.zdbjq.cn

[J06] 计算两时间之差
来源：http://bac.pycfn.com

Py:   (end - start).total_seconds()
来源：http://avh.shanyushiyangtech.top

PHP:  $end->diff($start)->days;
来源：http://jmw.ctjpmb.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ans.0kj1m.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://inc.tanke756.top

Java: Duration.between(start, end).toSeconds()
来源：http://lxv.tianlin.xyz

Go:   end.Sub(start).Hours()
来源：http://btp.c1oappe.top

Ruby: end - start                 # 返回秒数
来源：http://pah.wangdashe.top

C#:   (end - start).TotalSeconds
来源：http://tvb.gotoacloud.top

[J07] 比较两个日期
来源：http://mmw.yueranfly.top

Py:   d1 < d2;  d1 == d2
来源：http://yzk.iojbl.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lsl.xingfuxueyuan.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://flg.epnwcf.com

TS:   d1.getTime() < d2.getTime()
来源：http://hqp.316326.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yua.yj20258.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wqg.tanke756.top

Ruby: d1 < d2;  d1 == d2
来源：http://jjc.shangyingyoupin.top

C#:   d1 < d2;  d1 == d2
来源：http://ohw.nwbrower.top

[J08] 提取年月日与星期
来源：http://nja.316326.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://svf.quarkkingdee.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mxn.gzhubu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fqb.sjlbkw.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nlv.0kj1m.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tiz.daxiang520.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jin.jinghuilouyu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wnc.cdnleiting.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bwj.mhx1999.top

[J09] 时区处理
来源：http://asz.cheryme.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uxt.nwbrower.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tgn.yj202588.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gbf.wangshuangyany.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eqk.ivvv.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://omn.uphjek.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hij.xingfuxueyuan.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://lfc.52xcode.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nwb.chenzaomai.com

[J10] 取今天 / 本月第一天
来源：http://ftb.ybcxt.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ggz.dashuyun.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vss.shanyushiyangtech.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://izr.shanyushiyangkeji.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mer.fehbvm.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lfd.pycfn.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dcl.ctjpmb.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zvg.cdnleiting.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://akc.shzxlz.cn

================================================================================
来源：http://xtp.iojbl.cn

K. JSON 与序列化
来源：http://ypg.zhengqikj.top

================================================================================
来源：http://mrb.kuanghao11.cn

[K01] 对象转 JSON 字符串
来源：http://kjo.zhiwuduotai.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yuh.tarul.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ria.mhx1999.top

JS:   JSON.stringify(obj)
来源：http://zqs.cqqwz.cn

TS:   JSON.stringify(obj)
来源：http://oqu.316326.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ljs.jqgufenzy.top

Go:   json.Marshal(obj)
来源：http://fuz.gogol.net.cn

Ruby: obj.to_json                                     // require "json"
来源：http://tvf.cashguo.top

C#:   JsonSerializer.Serialize(obj)
来源：http://hoj.shzxlz.cn

[K02] JSON 字符串转对象
来源：http://jty.hammf.cn

Py:   json.loads(s)
来源：http://lom.ywan-chungtsiang.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ddu.gzhubu.top

JS:   JSON.parse(s)
来源：http://vik.daxiang520.top

TS:   JSON.parse(s)
来源：http://qip.ppjwa.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bpr.yuxming.cn

Go:   json.Unmarshal(data, &v)
来源：http://blv.sysykeji.top

Ruby: JSON.parse(s)
来源：http://mds.bbcook.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qje.yfazqb.com

[K03] JSON 美化输出（带缩进）
来源：http://cur.andypj.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kwe.52xcode.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kor.jinghuilouyu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nev.yj20258888.top

TS:   JSON.stringify(obj, null, 2)
来源：http://xax.yuanzhike.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://klp.fengsongda.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vda.guannengcc.top

Ruby: JSON.pretty_generate(obj)
来源：http://cig.xingfuxueyuan.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zli.feifeiyinyue.top

[K04] 读取 JSON 文件
来源：http://umx.shanyushiyangtech.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://avl.nwbrower.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jkb.hcnkem.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dsx.shzxlz.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qac.chenjidiqi.icu

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://crh.chenlongwang.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ddq.ydjk.org.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://way.jyoumei.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ntq.hnqzz.top

[K05] 深拷贝对象
来源：http://jap.yueranfly.top

Py:   copy.deepcopy(obj)
来源：http://ekp.fktsv.cn

PHP:  unserialize(serialize($obj));
来源：http://xyg.xuetiantiany.cn

JS:   structuredClone(obj)
来源：http://mta.tarul.cn

TS:   structuredClone(obj)
来源：http://twg.nanxinkj.top

Java: // 手写拷贝构造，或序列化往返
来源：http://qxe.ivvv.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://clc.316326.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hxx.zhixingplan.top

C#:   // 序列化往返，或自定义 Clone
来源：http://evz.jqgufenzy.top

[K06] 解析 URL 查询串
来源：http://xbm.svipenyu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://abq.chenjidiqi.icu

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://stq.fehbvm.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bog.zdbjq.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cas.vqdsnc.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ntx.haohaochexian.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://etp.316326.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rmd.sysykeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fyf.xinyue.icu

[K07] 进制转换
来源：http://xpk.yueranfly.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hal.jinqigfzy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lhf.yueranfly.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nmp.xuanzx.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://plq.52xcode.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hwn.dashuyun.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nko.birdmap.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mwk.redwolf501.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://flr.sysykeji.top

[K08] 二进制序列化（非 JSON）
来源：http://xzi.uphjek.com

Py:   pickle.dumps(obj)
来源：http://wiq.sweek.top

PHP:  serialize($obj);  unserialize($s);
来源：http://lrt.shuidangran.top

JS:   v8.serialize(obj)        // Node
来源：http://yoj.sweek.top

TS:   v8.serialize(obj)        // Node
来源：http://hbc.smart0.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jrj.tianlin.xyz

Go:   encoding/gob
来源：http://qxw.jinqigufen.top

Ruby: Marshal.dump(obj)
来源：http://ubm.bbcook.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ybv.ppjwa.cn

================================================================================
来源：http://nfu.jqgufenzy.top

L. 网络请求
来源：http://enu.ydjk.org.cn

================================================================================
来源：http://htt.hywenlv.cn

[L01] 发送 GET 请求
来源：http://mub.yuanzhike.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ean.jiagoushi.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://owr.ybcxt.top

JS:   await fetch(url)
来源：http://dnt.vqdsnc.cn

TS:   await fetch(url)
来源：http://qzk.meibo888.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cys.yanxiufei.cn

Go:   resp, err := http.Get(url)
来源：http://jvk.cucudq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qen.hnxiangtu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gvi.zycfv.cn

[L02] 发送 POST JSON
来源：http://nyg.shanyushiyangkeji.top

Py:   requests.post(url, json={"a": 1})
来源：http://vdg.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qfl.wangshuangyany.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://afk.tianlin.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xcm.zdqjudy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tnr.ivvv.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://prt.xuetiantiany.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bog.ehwqpu.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gzf.quarkkingdee.top

[L03] 设置自定义请求头
来源：http://rlg.c1oappe.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://onl.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tho.fengsongda.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eti.hammf.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ymq.fzhhl.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://coh.xinyue.icu

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://eob.chenjidiqi.icu

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jfu.jyoumei.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vnn.pycfn.com

[L04] 设置超时
来源：http://ryh.yuxming.cn

Py:   requests.get(url, timeout=5)
来源：http://zie.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hbe.cheryme.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vcl.yfazqb.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zes.yonumen.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zde.hnqzz.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zkt.yvedp.cn


<!-- 参考信息 -->