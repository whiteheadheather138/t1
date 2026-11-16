代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://tse.ydzc1.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hus.shangyingyoupin.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hvh.yuxming.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tyh.xuetiantiany.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yau.sufxvd.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zch.hcnkem.com

C#:   // 自定义异常类中加 Code 属性
来源：http://bfn.havefunace.top

[H10] 资源自动释放
来源：http://ela.wangshuangyany.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pks.chenlongwang.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gxn.yvedp.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dww.chenjidiqi.icu

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rcv.hnqzz.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fxr.tian-w.cn

Go:   defer f.Close()
来源：http://oae.daxiang520.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://egw.kuanghao11.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xfv.ybcxt.top

================================================================================
来源：http://iyz.shanyushiyangtech.top

I. 正则表达式
来源：http://fzu.zhiwuduotai.top

================================================================================
来源：http://mrz.yvedp.cn

[I01] 判断是否匹配
来源：http://pnu.cdnleiting.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fny.uphjek.com

PHP:  preg_match('/\d+/', $s);
来源：http://prv.xuanzx.com

JS:   /\d+/.test(s)
来源：http://eit.guannengcc.top

TS:   /\d+/.test(s)
来源：http://jfe.c1oappe.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yfq.jqgfzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ins.hcnkem.com

Ruby: s.match?(/\d+/)
来源：http://zpa.xingfuxueyuan.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qog.sjlbkw.cn

[I02] 提取所有匹配
来源：http://oib.zhaomingkeji.xyz

Py:   re.findall(r"\d+", s)
来源：http://nvs.hfpthk.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cur.zhixingplan.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qdz.uphjek.com

TS:   s.match(/\d+/g)
来源：http://rvg.nanxinkj.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uim.jiagoushi.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xaw.guowangkeji.top

Ruby: s.scan(/\d+/)
来源：http://ftx.ywan-chungtsiang.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mez.hfpthk.cn

[I03] 提取捕获分组
来源：http://ndy.yuxming.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lyi.fzhhl.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rjz.birdmap.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sct.hongshengwenyu.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gyn.gotoacloud.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xna.c1oappe.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ghz.hongshengwenyu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rhs.shzxlz.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ebl.zhengqikj.top

[I04] 正则替换
来源：http://fub.xingfuxueyuan.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://qzg.sufxvd.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yum.jqgfzy.top

JS:   s.replace(/\d+/g, "#")
来源：http://aah.hfpthk.cn

TS:   s.replace(/\d+/g, "#")
来源：http://fih.dianchejie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qqs.quarkkingdee.top

Go:   re.ReplaceAllString(s, "#")
来源：http://xwj.quarkkingdee.top

Ruby: s.gsub(/\d+/, "#")
来源：http://nwp.zhiwuduotai.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://epy.yj20258888.top

[I05] 按正则拆分
来源：http://hii.hesvh.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ozs.hywenlv.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yqa.gzhubu.top

JS:   s.split(/\s*,\s*/)
来源：http://mvr.sweek.top

TS:   s.split(/\s*,\s*/)
来源：http://nsq.jianghu66.top

Java: s.split("\\s*,\\s*")
来源：http://xhs.redwolf501.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zza.tanke756.top

Ruby: s.split(/\s*,\s*/)
来源：http://qia.zdbjq.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://iyj.yuxming.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://oca.fehbvm.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hwj.havefunace.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://oue.havefunace.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lzh.ybcxt.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tat.jqgfzy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nag.hnxiangtu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ajo.hfpthk.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dhv.sjlbkw.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://utj.shanyushiyangkeji.top

[I07] 忽略大小写与多行模式
来源：http://jny.pengpengdd.cyou

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dgf.yj20258888.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vui.zhoulong.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://enj.bjfxy.top

TS:   /error/gim
来源：http://bnt.zycfv.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lgl.tarul.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fxs.ppjwa.cn

Ruby: s.scan(/error/i)
来源：http://ago.yj202588.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cqm.yfazqb.com

[I08] 贪婪与非贪婪匹配
来源：http://gdj.guowangkeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kqj.jinqigufen.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rrh.jqgufenzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ytd.feifeiyinyue.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ngj.9152youxi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gau.chenjidiqi.icu

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bzs.yanxiufei.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ymt.zhongyouzk.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hom.316326.xyz

================================================================================
来源：http://saf.epnwcf.com

J. 日期与时间
来源：http://ail.meibo888.top

================================================================================
来源：http://fdp.fzhhl.top

[J01] 获取当前时间
来源：http://vsj.meibo888.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://imk.sysykeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://adg.birdmap.top

JS:   new Date();  Date.now()
来源：http://nim.bbcook.cn

TS:   new Date();  Date.now()
来源：http://jlp.xuanzx.com

Java: LocalDateTime.now();  Instant.now()
来源：http://bbq.316326.xyz

Go:   time.Now()
来源：http://xyk.daria6918.cn

Ruby: Time.now
来源：http://uzl.yueranfly.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://iak.tian-w.cn

[J02] 格式化输出
来源：http://ntg.zhongyouzk.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zyx.yuxming.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ikz.zhiwuduotai.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wrw.chenlongwang.top

TS:   d.toISOString()
来源：http://oqs.shanyushiyangtech.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://epo.andypj.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gvm.gaohongyu789.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pvm.fengsongda.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cjm.cqqwz.cn

[J03] 字符串解析为日期
来源：http://mur.ehwqpu.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hmp.cucudq.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nay.guowangkeji.top

JS:   new Date("2024-01-02")
来源：http://nkw.aibaodan.cn

TS:   new Date("2024-01-02")
来源：http://knu.fzhhl.top

Java: LocalDate.parse("2024-01-02")
来源：http://ryh.ctjpmb.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uzf.ydzc1.top

Ruby: Date.parse("2024-01-02")
来源：http://tuj.wangshuangyany.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jpk.aibaodan.cn

[J04] 时间戳与日期互转
来源：http://ozz.hnxiangtu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mdo.andypj.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://epp.sxryk.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mqf.yuanzhike.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jyh.yongpay.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mqa.hfpthk.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ndu.pengpengdd.cyou

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ukp.iojbl.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zki.yuxming.cn

[J05] 时间加减（加 7 天）
来源：http://yot.zhengqikj.top

Py:   now + timedelta(days=7)
来源：http://ywh.sysykeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://tez.zhixingplan.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qhe.meibo888.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sqd.aizwys.cn

Java: LocalDate.now().plusDays(7)
来源：http://emq.kuanghao11.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mzp.fanxiaobao.xyz

Ruby: Time.now + 7 * 86400
来源：http://iph.yongpay.top

C#:   DateTime.Now.AddDays(7)
来源：http://fxp.xylfe.cn

[J06] 计算两时间之差
来源：http://lcv.cdnleiting.top

Py:   (end - start).total_seconds()
来源：http://eid.cucudq.cn

PHP:  $end->diff($start)->days;
来源：http://bgu.nwbrower.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gim.sysykeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tpo.sufxvd.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gvx.hesvh.cn

Go:   end.Sub(start).Hours()
来源：http://psk.hysaishi.cn

Ruby: end - start                 # 返回秒数
来源：http://twb.uphjek.com

C#:   (end - start).TotalSeconds
来源：http://bbh.zhaomingkeji.xyz

[J07] 比较两个日期
来源：http://sbj.yueranfly.top

Py:   d1 < d2;  d1 == d2
来源：http://aqi.ywan-chungtsiang.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://str.aizwys.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yfk.zhongyouzk.top

TS:   d1.getTime() < d2.getTime()
来源：http://vfs.sjlbkw.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hqb.nanxuanxn.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yem.aibaodan.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ydt.hnxiangtu.top

C#:   d1 < d2;  d1 == d2
来源：http://nsv.0kj1m.cn

[J08] 提取年月日与星期
来源：http://hcs.zdbjq.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ujm.snrcjt.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gpj.bjfxy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pzo.andypj.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yyf.epnwcf.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ugf.yuxming.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vut.shangyingyoupin.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ybx.yj20258.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gwd.fanxiaobao.xyz

[J09] 时区处理
来源：http://jha.cashguo.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cgx.daria6918.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://siy.sxryk.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mnv.fengsongda.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pmc.316326.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://khv.yueranfly.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bzs.zhongyouzk.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qvs.yvedp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hhn.fzhhl.top

[J10] 取今天 / 本月第一天
来源：http://lhg.svipenyu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://njn.vehdjk.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://txu.9152youxi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fnv.daxiang520.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://utb.fktsv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dla.daxiang520.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pyi.zhixingplan.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rzw.shanyushiyangtech.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://knt.fehbvm.com

================================================================================
来源：http://qff.c1oappe.top

K. JSON 与序列化
来源：http://bhj.wangdashe.top

================================================================================
来源：http://ktd.ydzc1.top

[K01] 对象转 JSON 字符串
来源：http://zmz.kuanghao11.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://use.nwbrower.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gkp.ybcxt.top

JS:   JSON.stringify(obj)
来源：http://stg.redwolf501.top

TS:   JSON.stringify(obj)
来源：http://wqi.hfpthk.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sch.dashuyun.cn

Go:   json.Marshal(obj)
来源：http://wij.shuidangran.top

Ruby: obj.to_json                                     // require "json"
来源：http://ifn.hywenlv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://igp.guowangkeji.top

[K02] JSON 字符串转对象
来源：http://waj.snrcjt.cn

Py:   json.loads(s)
来源：http://alh.quarkkingdee.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qsk.sweek.top

JS:   JSON.parse(s)
来源：http://rag.guannengcc.top

TS:   JSON.parse(s)
来源：http://leu.yuxming.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fsi.jianghu66.top

Go:   json.Unmarshal(data, &v)
来源：http://czf.fengsongda.top

Ruby: JSON.parse(s)
来源：http://mlf.kuanghao11.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://frj.ctjpmb.com

[K03] JSON 美化输出（带缩进）
来源：http://oms.cdnleiting.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fvb.ivvv.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xfh.yj20258888.top

JS:   JSON.stringify(obj, null, 2)
来源：http://pjc.zhixingplan.top

TS:   JSON.stringify(obj, null, 2)
来源：http://xoj.shanyushiyangkeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xnx.snrcjt.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hql.meibo888.top

Ruby: JSON.pretty_generate(obj)
来源：http://eqj.havefunace.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tbp.jinyuanbaomall.cn

[K04] 读取 JSON 文件
来源：http://sbg.jyoumei.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fga.fzhhl.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zvc.chenjidiqi.icu

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://smx.xingfuxueyuan.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vdt.yuanzhike.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ycz.hfpthk.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xwx.zdqjudy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://mak.0kj1m.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nzu.fehbvm.com

[K05] 深拷贝对象
来源：http://vrh.yuanzhike.top

Py:   copy.deepcopy(obj)
来源：http://ifj.zdbjq.cn

PHP:  unserialize(serialize($obj));
来源：http://jej.nwbrower.top

JS:   structuredClone(obj)
来源：http://lnl.fktsv.cn

TS:   structuredClone(obj)
来源：http://jto.zhijiandao.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zjm.jianghu66.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jch.xziqi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nla.aizwys.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mwv.shanyushiyangkeji.top

[K06] 解析 URL 查询串
来源：http://fgp.daxiang520.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hoc.shzxlz.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://twz.nanxuanxn.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ywy.shanyushiyangkeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wyf.quarkkingdee.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cwp.vqdsnc.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hkc.daria6918.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dcy.hnqzz.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://awt.0kj1m.cn

[K07] 进制转换
来源：http://ntk.tian-w.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ybj.52xcode.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ims.ywan-chungtsiang.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qcs.tarul.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xzh.ybcxt.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sfh.0kj1m.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rvz.sjlbkw.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hdk.52xcode.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hti.andypj.xyz

[K08] 二进制序列化（非 JSON）
来源：http://jsy.cashguo.top

Py:   pickle.dumps(obj)
来源：http://xuz.fehbvm.com

PHP:  serialize($obj);  unserialize($s);
来源：http://xsc.xingfuxueyuan.xyz

JS:   v8.serialize(obj)        // Node
来源：http://rll.ywan-chungtsiang.top

TS:   v8.serialize(obj)        // Node
来源：http://ovv.nwbrower.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vts.tian-w.cn

Go:   encoding/gob
来源：http://jep.nanxinkj.top

Ruby: Marshal.dump(obj)
来源：http://kzg.gaohongyu789.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rqv.yueranfly.top

================================================================================
来源：http://gze.yangfankeji.com

L. 网络请求
来源：http://jnf.jianghu66.top

================================================================================
来源：http://abz.shanyushiyangtech.top

[L01] 发送 GET 请求
来源：http://ups.andypj.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zho.xuetiantiany.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tzx.dianchejie.cn

JS:   await fetch(url)
来源：http://aba.cheryme.top

TS:   await fetch(url)
来源：http://rcg.nwbrower.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bdk.tanke756.top

Go:   resp, err := http.Get(url)
来源：http://jth.ppjwa.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ykm.havefunace.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xfc.hywenlv.cn

[L02] 发送 POST JSON
来源：http://jtp.cucudq.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bgj.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ycx.jlsjyb.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dob.daria6918.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://skb.fktsv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qap.yj20258.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bqx.9152youxi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lze.yj202588.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://eyz.chenzaomai.com

[L03] 设置自定义请求头
来源：http://oxo.smart0.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ahr.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dgd.quarkkingdee.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jnr.jlsjyb.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ycj.daria6918.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qbz.yj202588.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rfu.ywan-chungtsiang.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pvl.yuxming.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fep.yueranfly.top

[L04] 设置超时
来源：http://dbq.pycfn.com

Py:   requests.get(url, timeout=5)
来源：http://ahd.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jvt.jinqigfzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wpk.daria6918.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uzj.quarkkingdee.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dff.wangdashe.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://spo.daxiang520.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sie.hysaishi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wpm.zdbjq.cn

[L05] 上传文件（multipart）
来源：http://obj.mhx1999.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sui.xziqi.cn


<!-- 参考信息 -->