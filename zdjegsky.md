代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://yts.yonumen.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tmn.xylfe.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vva.pycfn.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mfc.hongshengwenyu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ncq.yanxiufei.cn

Ruby: raise MyError.new("fail", 500)
来源：http://nvr.tanke756.top

C#:   // 自定义异常类中加 Code 属性
来源：http://tie.epnwcf.com

[H10] 资源自动释放
来源：http://pzz.bjfxy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://xfo.meibo888.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xxa.hfpthk.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xst.hysaishi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kks.jinyuanbaomall.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://emb.cqqwz.cn

Go:   defer f.Close()
来源：http://vaf.kuanghao11.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://swr.tanke756.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tlp.gzhubu.top

================================================================================
来源：http://opu.sweek.top

I. 正则表达式
来源：http://egd.sufxvd.cn

================================================================================
来源：http://hkx.iojbl.cn

[I01] 判断是否匹配
来源：http://oow.tianlin.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kkx.zdqjudy.top

PHP:  preg_match('/\d+/', $s);
来源：http://mvq.52xcode.cn

JS:   /\d+/.test(s)
来源：http://ilk.sweek.top

TS:   /\d+/.test(s)
来源：http://thh.cqqwz.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zme.wangshuangyany.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qlm.tanke756.top

Ruby: s.match?(/\d+/)
来源：http://xwx.quarkkingdee.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://atd.zhiwuduotai.top

[I02] 提取所有匹配
来源：http://aep.nwbrower.top

Py:   re.findall(r"\d+", s)
来源：http://nts.yanxiufei.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rde.wangdashe.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ieu.vqdsnc.cn

TS:   s.match(/\d+/g)
来源：http://hle.fanxiaobao.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://typ.yueranfly.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zxn.zhijiandao.cn

Ruby: s.scan(/\d+/)
来源：http://omp.cdnleiting.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dfc.wangdashe.top

[I03] 提取捕获分组
来源：http://epk.pengpengdd.cyou

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jjt.gotoacloud.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wzq.jyoumei.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tqt.hfpthk.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ehl.xuanzx.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sah.xziqi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ywd.ydjk.org.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qxh.tianlin.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rmt.jqgfzy.top

[I04] 正则替换
来源：http://pyo.zdbjq.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zuc.xylfe.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://isq.hfpthk.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jsb.ctjpmb.com

TS:   s.replace(/\d+/g, "#")
来源：http://yno.316326.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://sgp.zycfv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zdw.jinqigufen.top

Ruby: s.gsub(/\d+/, "#")
来源：http://opa.ydzc1.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yaj.nwbrower.top

[I05] 按正则拆分
来源：http://bet.yj20258888.top

Py:   re.split(r"\s*,\s*", s)
来源：http://hiy.yuxming.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zdb.9152youxi.cn

JS:   s.split(/\s*,\s*/)
来源：http://eqo.tianlin.xyz

TS:   s.split(/\s*,\s*/)
来源：http://xer.zdqjudy.top

Java: s.split("\\s*,\\s*")
来源：http://obb.cucudq.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gyz.sufxvd.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nmz.xinyue.icu

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uvl.ywan-chungtsiang.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wpf.nwbrower.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zxp.sysykeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yqi.bbcook.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aoa.yuanzhike.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tra.svipenyu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vxv.nwbrower.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qhh.sxryk.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tsr.nanxuanxn.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jln.zycfv.cn

[I07] 忽略大小写与多行模式
来源：http://gxt.hongshengwenyu.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://owx.zdbjq.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xpf.ydjk.org.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://phl.shuidangran.top

TS:   /error/gim
来源：http://ziw.shzxlz.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ebp.ywan-chungtsiang.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://diu.zhongyouzk.top

Ruby: s.scan(/error/i)
来源：http://smh.andypj.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tka.shzxlz.cn

[I08] 贪婪与非贪婪匹配
来源：http://peb.dianchejie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gjr.yangfankeji.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kyy.hnqzz.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gem.zhoulong.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jec.zhijiandao.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ynx.sweek.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sqd.zdqjudy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rwe.xinyue.icu

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sjp.yfazqb.com

================================================================================
来源：http://jye.gogol.net.cn

J. 日期与时间
来源：http://lco.jlsjyb.cn

================================================================================
来源：http://rot.pycfn.com

[J01] 获取当前时间
来源：http://ixk.aibaodan.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://eka.bbcook.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gap.bbcook.cn

JS:   new Date();  Date.now()
来源：http://riv.hnqzz.top

TS:   new Date();  Date.now()
来源：http://gvh.guowangkeji.top

Java: LocalDateTime.now();  Instant.now()
来源：http://kfi.zhiwuduotai.top

Go:   time.Now()
来源：http://yqo.jyoumei.cn

Ruby: Time.now
来源：http://cid.gzhubu.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tyy.jlsjyb.cn

[J02] 格式化输出
来源：http://vzt.yanxiufei.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uam.bjfxy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nxn.fehbvm.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hup.snrcjt.cn

TS:   d.toISOString()
来源：http://qye.ivvv.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ugn.ivvv.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://aqn.birdmap.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oir.chenlongwang.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kzc.pengpengdd.cyou

[J03] 字符串解析为日期
来源：http://fkn.nanxinkj.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sfy.xziqi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ibk.fengsongda.top

JS:   new Date("2024-01-02")
来源：http://ryz.daxiang520.top

TS:   new Date("2024-01-02")
来源：http://abo.fehbvm.com

Java: LocalDate.parse("2024-01-02")
来源：http://obv.yuxming.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dft.c1oappe.top

Ruby: Date.parse("2024-01-02")
来源：http://nod.nwbrower.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kve.xingfuxueyuan.xyz

[J04] 时间戳与日期互转
来源：http://jvn.gzhubu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lem.andypj.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yhg.vqdsnc.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sfk.yfazqb.com

TS:   Math.floor(Date.now() / 1000)
来源：http://ymb.nanxinkj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lye.uphjek.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://scq.ppjwa.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://znw.daxiang520.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://woh.aibaodan.cn

[J05] 时间加减（加 7 天）
来源：http://bqe.haohaochexian.top

Py:   now + timedelta(days=7)
来源：http://phl.ydzc1.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://tqe.zdbjq.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wod.birdmap.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rzl.hnqzz.top

Java: LocalDate.now().plusDays(7)
来源：http://svj.mhx1999.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://emg.jinghuilouyu.cn

Ruby: Time.now + 7 * 86400
来源：http://fbg.uphjek.com

C#:   DateTime.Now.AddDays(7)
来源：http://qjh.jyoumei.cn

[J06] 计算两时间之差
来源：http://ykt.snrcjt.cn

Py:   (end - start).total_seconds()
来源：http://tkq.zhixingplan.top

PHP:  $end->diff($start)->days;
来源：http://scu.jqgfzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://goh.hywenlv.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fyu.xingfuxueyuan.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://qqv.jyoumei.cn

Go:   end.Sub(start).Hours()
来源：http://woe.yanxiufei.cn

Ruby: end - start                 # 返回秒数
来源：http://efd.xylfe.cn

C#:   (end - start).TotalSeconds
来源：http://nkn.kuanghao11.cn

[J07] 比较两个日期
来源：http://vie.yonumen.top

Py:   d1 < d2;  d1 == d2
来源：http://tsv.daria6918.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ipm.daxiang520.top

JS:   d1.getTime() < d2.getTime()
来源：http://lne.yongpay.top

TS:   d1.getTime() < d2.getTime()
来源：http://mjc.9152youxi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uyw.hesvh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jmo.shanyushiyangkeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://fvk.9152youxi.cn

C#:   d1 < d2;  d1 == d2
来源：http://ozw.yj20258.top

[J08] 提取年月日与星期
来源：http://jqc.yj202588.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dlv.ivvv.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nai.meibo888.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://por.chenlongwang.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mbq.xingfuxueyuan.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ctv.c1oappe.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mqe.aibaodan.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tqe.hcnkem.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ybe.shangyingyoupin.top

[J09] 时区处理
来源：http://xpc.zdbjq.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zbi.zhengqikj.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mze.ywan-chungtsiang.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://laj.cucudq.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ycv.svipenyu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lto.nanxuanxn.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ron.zhijiandao.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pnr.yvedp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zaw.yuxming.cn

[J10] 取今天 / 本月第一天
来源：http://wwz.gaohongyu789.top

Py:   date.today();  date.today().replace(day=1)
来源：http://vjx.aibaodan.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qif.havefunace.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mca.fanxiaobao.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pfr.jinghuilouyu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bru.zdbjq.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yiz.cucudq.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zya.jqgfzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tfw.chenjidiqi.icu

================================================================================
来源：http://vhg.cucudq.cn

K. JSON 与序列化
来源：http://sxb.feifeiyinyue.top

================================================================================
来源：http://qpj.jinghuilouyu.cn

[K01] 对象转 JSON 字符串
来源：http://yka.havefunace.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uuu.xylfe.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ygu.iojbl.cn

JS:   JSON.stringify(obj)
来源：http://uzd.zhaomingkeji.xyz

TS:   JSON.stringify(obj)
来源：http://mcz.9152youxi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://reb.hfpthk.cn

Go:   json.Marshal(obj)
来源：http://ckl.hysaishi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://blb.hnqzz.top

C#:   JsonSerializer.Serialize(obj)
来源：http://yxn.hongshengwenyu.top

[K02] JSON 字符串转对象
来源：http://asv.zhijiandao.cn

Py:   json.loads(s)
来源：http://dau.vqdsnc.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jbr.wangshuangyany.cn

JS:   JSON.parse(s)
来源：http://utz.xziqi.cn

TS:   JSON.parse(s)
来源：http://cld.hywenlv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://plz.shanyushiyangkeji.top

Go:   json.Unmarshal(data, &v)
来源：http://ios.yj20258.top

Ruby: JSON.parse(s)
来源：http://lmk.guannengcc.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mgd.cashguo.top

[K03] JSON 美化输出（带缩进）
来源：http://osj.meibo888.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jgi.epnwcf.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hlj.haohaochexian.top

JS:   JSON.stringify(obj, null, 2)
来源：http://icr.haohaochexian.top

TS:   JSON.stringify(obj, null, 2)
来源：http://dbw.yuanzhike.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gxd.jinyuanbaomall.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ddf.shuidangran.top

Ruby: JSON.pretty_generate(obj)
来源：http://cbe.zhaomingkeji.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ikm.yonumen.top

[K04] 读取 JSON 文件
来源：http://nps.cqqwz.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rii.vehdjk.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xny.zdbjq.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gdk.zhengqikj.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pfo.pengpengdd.cyou

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wck.birdmap.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zew.jinqigfzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://lio.shanyushiyangkeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://icg.jyoumei.cn

[K05] 深拷贝对象
来源：http://yaz.nanxinkj.top

Py:   copy.deepcopy(obj)
来源：http://cke.dashuyun.cn

PHP:  unserialize(serialize($obj));
来源：http://vzo.9152youxi.cn

JS:   structuredClone(obj)
来源：http://kee.hongshengwenyu.top

TS:   structuredClone(obj)
来源：http://dgd.smart0.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://ozq.xuetiantiany.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://igk.vehdjk.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ged.sysykeji.top

C#:   // 序列化往返，或自定义 Clone
来源：http://vra.shanyushiyangtech.top

[K06] 解析 URL 查询串
来源：http://usl.jinqigufen.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zby.sjlbkw.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dej.yanxiufei.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lkq.cucudq.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iku.epnwcf.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ztn.9152youxi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://imr.sufxvd.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xjv.fengsongda.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dus.cheryme.top

[K07] 进制转换
来源：http://oma.sufxvd.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cku.bbcook.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cfb.zdbjq.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vpe.zdqjudy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uso.xuanzx.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bdv.sxryk.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lpy.gogol.net.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hrq.cdnleiting.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qdv.nanxuanxn.top

[K08] 二进制序列化（非 JSON）
来源：http://ena.xuanzx.com

Py:   pickle.dumps(obj)
来源：http://fdx.0kj1m.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gsy.fehbvm.com

JS:   v8.serialize(obj)        // Node
来源：http://suk.shanyushiyangtech.top

TS:   v8.serialize(obj)        // Node
来源：http://epo.xylfe.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rhn.ydzc1.top

Go:   encoding/gob
来源：http://frt.nwbrower.top

Ruby: Marshal.dump(obj)
来源：http://thq.hfpthk.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cft.jinqigfzy.top

================================================================================
来源：http://tmv.ctjpmb.com

L. 网络请求
来源：http://jaa.wangdashe.top

================================================================================
来源：http://nxm.guowangkeji.top

[L01] 发送 GET 请求
来源：http://eir.gotoacloud.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jkk.jinqigfzy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kap.yongpay.top

JS:   await fetch(url)
来源：http://vot.daria6918.cn

TS:   await fetch(url)
来源：http://nrl.zdbjq.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gxx.jinqigufen.top

Go:   resp, err := http.Get(url)
来源：http://zoh.vehdjk.com

Ruby: Net::HTTP.get(URI(url))
来源：http://xld.shanyushiyangkeji.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vcm.wangshuangyany.cn

[L02] 发送 POST JSON
来源：http://fzz.dashuyun.cn

Py:   requests.post(url, json={"a": 1})
来源：http://neb.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gqr.vqdsnc.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yit.daria6918.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aks.9152youxi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://brc.zhongyouzk.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://roy.xziqi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ykf.haohaochexian.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://svj.snrcjt.cn

[L03] 设置自定义请求头
来源：http://mpv.hysaishi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ege.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://eaz.ivvv.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ars.shangyingyoupin.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://agy.shzxlz.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://axy.dashuyun.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hwa.yongpay.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xbh.yfazqb.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sng.zhaomingkeji.xyz

[L04] 设置超时
来源：http://wme.ydzc1.top

Py:   requests.get(url, timeout=5)
来源：http://idq.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cgj.svipenyu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qvd.redwolf501.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dzb.yueranfly.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xay.iojbl.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://aql.zdqjudy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://itk.fengsongda.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://eln.jinghuilouyu.cn

[L05] 上传文件（multipart）
来源：http://iuq.tanke756.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zfs.redwolf501.top


<!-- 参考信息 -->