代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zbc.aizwys.cn

Ruby: raise MyError.new("fail", 500)
来源：http://faj.zhoulong.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://ikw.jinghuilouyu.cn

[H10] 资源自动释放
来源：http://lwg.nanxinkj.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://jbj.sjlbkw.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jqg.ydzc1.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://okp.redwolf501.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kii.zhengqikj.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hwj.fzhhl.top

Go:   defer f.Close()
来源：http://szb.andypj.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rxa.hcnkem.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fhd.guowangkeji.top

================================================================================
来源：http://lnp.haohaochexian.top

I. 正则表达式
来源：http://fgh.hfpthk.cn

================================================================================
来源：http://tit.cdnleiting.top

[I01] 判断是否匹配
来源：http://tmh.andypj.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tsz.ywan-chungtsiang.top

PHP:  preg_match('/\d+/', $s);
来源：http://nai.nanxuanxn.top

JS:   /\d+/.test(s)
来源：http://bzs.zhongyouzk.top

TS:   /\d+/.test(s)
来源：http://alm.9152youxi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://aud.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nxm.cucudq.cn

Ruby: s.match?(/\d+/)
来源：http://gih.yangfankeji.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fel.jlsjyb.cn

[I02] 提取所有匹配
来源：http://bvi.bjfxy.top

Py:   re.findall(r"\d+", s)
来源：http://zhd.zycfv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pue.smart0.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pxd.hcnkem.com

TS:   s.match(/\d+/g)
来源：http://try.yj20258888.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bkv.0kj1m.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pld.nwbrower.top

Ruby: s.scan(/\d+/)
来源：http://rwd.ivvv.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cxh.pycfn.com

[I03] 提取捕获分组
来源：http://pby.hongshengwenyu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uph.jlsjyb.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dsp.haohaochexian.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hbs.jinghuilouyu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://snl.ydzc1.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gnx.tianlin.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bwe.jyoumei.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bte.jianghu66.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zgi.yanxiufei.cn

[I04] 正则替换
来源：http://nuj.hfpthk.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://tvd.xinyue.icu

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ohv.yfazqb.com

JS:   s.replace(/\d+/g, "#")
来源：http://enq.ydjk.org.cn

TS:   s.replace(/\d+/g, "#")
来源：http://uhi.svipenyu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dxv.jlsjyb.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://khw.bbcook.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ymt.nwbrower.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jdp.dashuyun.cn

[I05] 按正则拆分
来源：http://jrh.zhongyouzk.top

Py:   re.split(r"\s*,\s*", s)
来源：http://mso.gaohongyu789.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ksj.nanxuanxn.top

JS:   s.split(/\s*,\s*/)
来源：http://bqg.cucudq.cn

TS:   s.split(/\s*,\s*/)
来源：http://cpv.ivvv.top

Java: s.split("\\s*,\\s*")
来源：http://vzd.xinyue.icu

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jwb.cqqwz.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jtp.vqdsnc.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://knu.epnwcf.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cbl.jiagoushi.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://joj.daria6918.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://otb.ydzc1.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rre.0kj1m.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qku.xuetiantiany.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ory.gzhubu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://akv.zhaomingkeji.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mzx.cashguo.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zwk.hnqzz.top

[I07] 忽略大小写与多行模式
来源：http://ilh.feifeiyinyue.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bch.yfazqb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fqe.jianghu66.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mgk.meibo888.top

TS:   /error/gim
来源：http://lya.cqqwz.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://msj.fktsv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sdm.jinqigfzy.top

Ruby: s.scan(/error/i)
来源：http://abd.chenlongwang.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bow.hammf.cn

[I08] 贪婪与非贪婪匹配
来源：http://jlp.xuetiantiany.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://let.0kj1m.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yre.yonumen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nqs.xziqi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yfq.snrcjt.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lru.haohaochexian.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kbm.quarkkingdee.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vvs.gaohongyu789.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zij.yj20258888.top

================================================================================
来源：http://uoz.0kj1m.cn

J. 日期与时间
来源：http://pjw.kuanghao11.cn

================================================================================
来源：http://bbm.xingfuxueyuan.xyz

[J01] 获取当前时间
来源：http://vjj.zhoulong.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://zum.yvedp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mhu.ehwqpu.com

JS:   new Date();  Date.now()
来源：http://qiv.shzxlz.cn

TS:   new Date();  Date.now()
来源：http://bpb.bjfxy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://lef.jqgufenzy.top

Go:   time.Now()
来源：http://ybq.zhixingplan.top

Ruby: Time.now
来源：http://aow.redwolf501.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ejm.tanke756.top

[J02] 格式化输出
来源：http://dzk.kuanghao11.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lun.hongshengwenyu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bfv.nanxuanxn.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ruk.yfazqb.com

TS:   d.toISOString()
来源：http://pps.zhixingplan.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qtz.tianlin.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://uso.xuanzx.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nof.gogol.net.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gze.xziqi.cn

[J03] 字符串解析为日期
来源：http://elv.shanyushiyangtech.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://njf.yvedp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://npq.gotoacloud.top

JS:   new Date("2024-01-02")
来源：http://idd.0kj1m.cn

TS:   new Date("2024-01-02")
来源：http://qnv.yangfankeji.com

Java: LocalDate.parse("2024-01-02")
来源：http://hwx.sxryk.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://aql.tanke756.top

Ruby: Date.parse("2024-01-02")
来源：http://evs.zhaomingkeji.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xbs.xziqi.cn

[J04] 时间戳与日期互转
来源：http://msq.yuxming.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://huv.dashuyun.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wad.ydjk.org.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zne.ctjpmb.com

TS:   Math.floor(Date.now() / 1000)
来源：http://cqp.0kj1m.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fcv.zhongyouzk.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dyi.yuanzhike.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kla.jiagoushi.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vwy.vehdjk.com

[J05] 时间加减（加 7 天）
来源：http://ngy.sxryk.cn

Py:   now + timedelta(days=7)
来源：http://mse.bbcook.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vmi.chenlongwang.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bsz.meibo888.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mki.yanxiufei.cn

Java: LocalDate.now().plusDays(7)
来源：http://mvm.sjlbkw.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tqy.vehdjk.com

Ruby: Time.now + 7 * 86400
来源：http://kmo.sjlbkw.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ntp.sweek.top

[J06] 计算两时间之差
来源：http://lyl.vqdsnc.cn

Py:   (end - start).total_seconds()
来源：http://sqt.hesvh.cn

PHP:  $end->diff($start)->days;
来源：http://fja.cheryme.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://svl.sysykeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://saz.jiagoushi.top

Java: Duration.between(start, end).toSeconds()
来源：http://bie.fanxiaobao.xyz

Go:   end.Sub(start).Hours()
来源：http://jir.vqdsnc.cn

Ruby: end - start                 # 返回秒数
来源：http://wyu.sxryk.cn

C#:   (end - start).TotalSeconds
来源：http://pnl.yj20258.top

[J07] 比较两个日期
来源：http://wav.gzhubu.top

Py:   d1 < d2;  d1 == d2
来源：http://ebc.sxryk.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nvv.epnwcf.com

JS:   d1.getTime() < d2.getTime()
来源：http://vnm.zycfv.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vzn.tarul.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vgk.hongshengwenyu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zwm.cdnleiting.top

Ruby: d1 < d2;  d1 == d2
来源：http://nhl.nwbrower.top

C#:   d1 < d2;  d1 == d2
来源：http://tlt.zhongyouzk.top

[J08] 提取年月日与星期
来源：http://ylz.havefunace.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tjz.316326.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lmo.vqdsnc.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ldh.guowangkeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tka.gotoacloud.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jkx.xylfe.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qwk.havefunace.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pct.9152youxi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://miw.ywan-chungtsiang.top

[J09] 时区处理
来源：http://wfw.zhaomingkeji.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://syj.tian-w.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cwl.chenzaomai.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ubk.zycfv.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dom.guannengcc.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ywv.shuidangran.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cbg.52xcode.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wnt.yonumen.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://oee.yj202588.top

[J10] 取今天 / 本月第一天
来源：http://dgw.fehbvm.com

Py:   date.today();  date.today().replace(day=1)
来源：http://qms.bbcook.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dix.hnqzz.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nsy.snrcjt.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://chd.xuetiantiany.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yvo.jinghuilouyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://eoy.hywenlv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tnb.zhengqikj.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tvl.vehdjk.com

================================================================================
来源：http://hdt.hnqzz.top

K. JSON 与序列化
来源：http://klt.dianchejie.cn

================================================================================
来源：http://che.guowangkeji.top

[K01] 对象转 JSON 字符串
来源：http://sxq.zhengqikj.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tjr.shanyushiyangtech.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xwj.ydzc1.top

JS:   JSON.stringify(obj)
来源：http://mpx.smart0.xyz

TS:   JSON.stringify(obj)
来源：http://qff.c1oappe.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ktq.ivvv.top

Go:   json.Marshal(obj)
来源：http://slg.gaohongyu789.top

Ruby: obj.to_json                                     // require "json"
来源：http://cix.cucudq.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zcd.jianghu66.top

[K02] JSON 字符串转对象
来源：http://shi.guannengcc.top

Py:   json.loads(s)
来源：http://jfa.xinyue.icu

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ggk.sysykeji.top

JS:   JSON.parse(s)
来源：http://apv.316326.xyz

TS:   JSON.parse(s)
来源：http://tgn.yueranfly.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wxs.smart0.xyz

Go:   json.Unmarshal(data, &v)
来源：http://ndf.aizwys.cn

Ruby: JSON.parse(s)
来源：http://gpf.chenzaomai.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://csc.aibaodan.cn

[K03] JSON 美化输出（带缩进）
来源：http://tuz.jyoumei.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vop.nanxuanxn.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gfi.xuetiantiany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vsa.dianchejie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fxu.wangdashe.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gqp.ctjpmb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fkn.shanyushiyangkeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://bdj.bbcook.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hpy.xylfe.cn

[K04] 读取 JSON 文件
来源：http://zum.zhaomingkeji.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bec.gzhubu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://njk.hysaishi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ltd.aibaodan.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zvl.zhoulong.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://iie.pengpengdd.cyou

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://htf.jinyuanbaomall.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ytv.hammf.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://aur.meibo888.top

[K05] 深拷贝对象
来源：http://rtx.chenzaomai.com

Py:   copy.deepcopy(obj)
来源：http://exm.fengsongda.top

PHP:  unserialize(serialize($obj));
来源：http://lzu.xziqi.cn

JS:   structuredClone(obj)
来源：http://mpv.cucudq.cn

TS:   structuredClone(obj)
来源：http://qny.zhongyouzk.top

Java: // 手写拷贝构造，或序列化往返
来源：http://vet.epnwcf.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fjy.jlsjyb.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zwb.xylfe.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tub.yongpay.top

[K06] 解析 URL 查询串
来源：http://ure.yfazqb.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xeu.uphjek.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wne.hnxiangtu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://drp.jiagoushi.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kgn.tian-w.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hyj.ivvv.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://cfi.yongpay.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://eqc.aizwys.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xxe.redwolf501.top

[K07] 进制转换
来源：http://bnn.zhiwuduotai.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tsp.shuidangran.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ppj.hysaishi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jwm.feifeiyinyue.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mir.ywan-chungtsiang.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dak.zhoulong.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wwu.hywenlv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ign.yuxming.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fgr.yj20258.top

[K08] 二进制序列化（非 JSON）
来源：http://nme.tian-w.cn

Py:   pickle.dumps(obj)
来源：http://xmq.hongshengwenyu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://yag.zycfv.cn

JS:   v8.serialize(obj)        // Node
来源：http://ojt.dashuyun.cn

TS:   v8.serialize(obj)        // Node
来源：http://rsq.xylfe.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yhj.9152youxi.cn

Go:   encoding/gob
来源：http://zzh.ybcxt.top

Ruby: Marshal.dump(obj)
来源：http://gwb.yuxming.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yeo.yuanzhike.top

================================================================================
来源：http://tvp.hcnkem.com

L. 网络请求
来源：http://qws.quarkkingdee.top

================================================================================
来源：http://agc.fzhhl.top

[L01] 发送 GET 请求
来源：http://fzl.ppjwa.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jxz.shuidangran.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jpa.zhengqikj.top

JS:   await fetch(url)
来源：http://wpb.hammf.cn

TS:   await fetch(url)
来源：http://lyw.tian-w.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qkv.jinqigufen.top

Go:   resp, err := http.Get(url)
来源：http://ftm.zhixingplan.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dwp.0kj1m.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vum.ydzc1.top

[L02] 发送 POST JSON
来源：http://cmi.jqgufenzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://fsl.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pzg.fehbvm.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vpi.haohaochexian.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ufn.zhijiandao.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hzq.haohaochexian.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://czb.jinqigufen.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ugs.shzxlz.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sga.mhx1999.top

[L03] 设置自定义请求头
来源：http://umr.vehdjk.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://una.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vdi.jqgufenzy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fsk.sysykeji.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hrg.jinqigufen.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pxy.yfazqb.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pzg.yj20258888.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gnu.jqgfzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jik.yuanzhike.top

[L04] 设置超时
来源：http://ois.tanke756.top

Py:   requests.get(url, timeout=5)
来源：http://jyc.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://huk.jianghu66.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yxf.gaohongyu789.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fbi.jiagoushi.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yev.zhoulong.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rnp.shanyushiyangkeji.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://geo.chenjidiqi.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uuy.tanke756.top

[L05] 上传文件（multipart）
来源：http://hyg.quarkkingdee.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tmy.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://owy.yfazqb.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pae.fzhhl.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sei.c1oappe.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gps.hnxiangtu.top


<!-- 参考信息 -->