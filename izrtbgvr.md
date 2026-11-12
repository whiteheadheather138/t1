代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://jgh.feifeiyinyue.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ufi.pengpengdd.cyou

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pvq.aizwys.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ebk.hfpthk.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sbp.jinghuilouyu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gyr.zhoulong.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://qwa.guannengcc.top

[H10] 资源自动释放
来源：http://afy.tanke756.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://zvm.0kj1m.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mtx.birdmap.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nay.zhixingplan.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jyw.epnwcf.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jad.epnwcf.com

Go:   defer f.Close()
来源：http://ckv.yanxiufei.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tgb.tian-w.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rsx.tianlin.xyz

================================================================================
来源：http://pqu.ydzc1.top

I. 正则表达式
来源：http://uzy.yonumen.top

================================================================================
来源：http://oay.hnqzz.top

[I01] 判断是否匹配
来源：http://dbi.gotoacloud.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lbw.dianchejie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vpj.yj20258.top

JS:   /\d+/.test(s)
来源：http://umk.yvedp.cn

TS:   /\d+/.test(s)
来源：http://gxk.ydjk.org.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zgr.yfazqb.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://aao.nanxinkj.top

Ruby: s.match?(/\d+/)
来源：http://obz.9152youxi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://try.jqgufenzy.top

[I02] 提取所有匹配
来源：http://txg.aizwys.cn

Py:   re.findall(r"\d+", s)
来源：http://prq.cdnleiting.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://eso.yuanzhike.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lrb.9152youxi.cn

TS:   s.match(/\d+/g)
来源：http://xrd.ctjpmb.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ycs.redwolf501.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zql.cqqwz.cn

Ruby: s.scan(/\d+/)
来源：http://rmp.ywan-chungtsiang.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://huu.zhongyouzk.top

[I03] 提取捕获分组
来源：http://ikf.cashguo.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xja.hongshengwenyu.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rat.tianlin.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yvw.xuanzx.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dwz.yangfankeji.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://adl.chenlongwang.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tkp.jqgfzy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://urf.bjfxy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://icg.dashuyun.cn

[I04] 正则替换
来源：http://eiu.sxryk.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://tvs.smart0.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bwk.sysykeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://lff.cashguo.top

TS:   s.replace(/\d+/g, "#")
来源：http://ocd.hcnkem.com

Java: s.replaceAll("\\d+", "#")
来源：http://krx.jianghu66.top

Go:   re.ReplaceAllString(s, "#")
来源：http://hya.xziqi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://chh.shzxlz.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qoj.bjfxy.top

[I05] 按正则拆分
来源：http://ppi.sufxvd.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hfp.ydzc1.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jgk.tarul.cn

JS:   s.split(/\s*,\s*/)
来源：http://vjg.birdmap.top

TS:   s.split(/\s*,\s*/)
来源：http://paa.sxryk.cn

Java: s.split("\\s*,\\s*")
来源：http://hmw.shuidangran.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yxl.xziqi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://crd.tianlin.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mqs.mhx1999.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zvq.hesvh.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cjj.daria6918.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ojc.ydjk.org.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ovo.yfazqb.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xyt.uphjek.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ord.epnwcf.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://djh.guannengcc.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yye.cheryme.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rmi.mhx1999.top

[I07] 忽略大小写与多行模式
来源：http://foh.jqgfzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://uls.sjlbkw.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fgn.shuidangran.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jiq.fehbvm.com

TS:   /error/gim
来源：http://fze.ehwqpu.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ksn.redwolf501.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sgg.hongshengwenyu.top

Ruby: s.scan(/error/i)
来源：http://ctl.havefunace.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nel.guannengcc.top

[I08] 贪婪与非贪婪匹配
来源：http://fzy.cucudq.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://spz.ivvv.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://njt.yj20258.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hur.ywan-chungtsiang.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://aki.yangfankeji.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://wah.yueranfly.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gai.pycfn.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rfx.jiagoushi.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rba.havefunace.top

================================================================================
来源：http://thh.andypj.xyz

J. 日期与时间
来源：http://gyo.ywan-chungtsiang.top

================================================================================
来源：http://tra.aibaodan.cn

[J01] 获取当前时间
来源：http://tig.svipenyu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yjj.hfpthk.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tkd.shanyushiyangtech.top

JS:   new Date();  Date.now()
来源：http://ldb.redwolf501.top

TS:   new Date();  Date.now()
来源：http://lvf.0kj1m.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rnp.fehbvm.com

Go:   time.Now()
来源：http://tyk.fehbvm.com

Ruby: Time.now
来源：http://kmv.tianlin.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://woy.zhongyouzk.top

[J02] 格式化输出
来源：http://lcu.zhixingplan.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hzv.aizwys.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://peh.daxiang520.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mam.shanyushiyangtech.top

TS:   d.toISOString()
来源：http://ycd.bjfxy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://exr.wangshuangyany.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ige.yfazqb.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qtx.wangshuangyany.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://afs.haohaochexian.top

[J03] 字符串解析为日期
来源：http://ans.meibo888.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://acq.gzhubu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tcx.xuetiantiany.cn

JS:   new Date("2024-01-02")
来源：http://vvu.yj202588.top

TS:   new Date("2024-01-02")
来源：http://uwg.316326.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://mtz.tarul.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uck.tarul.cn

Ruby: Date.parse("2024-01-02")
来源：http://lgm.sysykeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://aor.gzhubu.top

[J04] 时间戳与日期互转
来源：http://fji.ehwqpu.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qow.aizwys.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cyr.jinyuanbaomall.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yje.zhixingplan.top

TS:   Math.floor(Date.now() / 1000)
来源：http://mmv.shangyingyoupin.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://erj.iojbl.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://knh.hesvh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dcz.hywenlv.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zjd.aibaodan.cn

[J05] 时间加减（加 7 天）
来源：http://kbo.meibo888.top

Py:   now + timedelta(days=7)
来源：http://yqg.fktsv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bgr.snrcjt.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bib.ydzc1.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://oju.yueranfly.top

Java: LocalDate.now().plusDays(7)
来源：http://vgj.svipenyu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yxf.havefunace.top

Ruby: Time.now + 7 * 86400
来源：http://ykj.nanxuanxn.top

C#:   DateTime.Now.AddDays(7)
来源：http://lgk.52xcode.cn

[J06] 计算两时间之差
来源：http://tsd.uphjek.com

Py:   (end - start).total_seconds()
来源：http://krk.yj20258.top

PHP:  $end->diff($start)->days;
来源：http://yax.zhaomingkeji.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dkz.svipenyu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yur.pycfn.com

Java: Duration.between(start, end).toSeconds()
来源：http://vco.xylfe.cn

Go:   end.Sub(start).Hours()
来源：http://yec.hnqzz.top

Ruby: end - start                 # 返回秒数
来源：http://ebp.epnwcf.com

C#:   (end - start).TotalSeconds
来源：http://snp.shzxlz.cn

[J07] 比较两个日期
来源：http://xlg.shangyingyoupin.top

Py:   d1 < d2;  d1 == d2
来源：http://zkg.zhongyouzk.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qfx.zycfv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rin.cucudq.cn

TS:   d1.getTime() < d2.getTime()
来源：http://thm.jinyuanbaomall.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gpc.cashguo.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gxu.gogol.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vai.xingfuxueyuan.xyz

C#:   d1 < d2;  d1 == d2
来源：http://ezh.yj20258.top

[J08] 提取年月日与星期
来源：http://izl.aibaodan.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sdm.zhaomingkeji.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vqo.gotoacloud.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ewp.andypj.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fdl.zhiwuduotai.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://irs.tian-w.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rsr.yonumen.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yon.cqqwz.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://phz.tanke756.top

[J09] 时区处理
来源：http://wti.yonumen.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pig.jinyuanbaomall.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://frx.daria6918.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://udz.ybcxt.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yku.316326.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://eop.yonumen.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rmw.xziqi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://nch.hcnkem.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lsh.fengsongda.top

[J10] 取今天 / 本月第一天
来源：http://map.aibaodan.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vvb.jinyuanbaomall.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://etj.yj20258.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wxt.fehbvm.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vcj.vqdsnc.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qgv.jinqigufen.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yom.cqqwz.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jnj.chenjidiqi.icu

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ylo.sjlbkw.cn

================================================================================
来源：http://yii.gzhubu.top

K. JSON 与序列化
来源：http://tpo.tian-w.cn

================================================================================
来源：http://zsb.zhaomingkeji.xyz

[K01] 对象转 JSON 字符串
来源：http://rgi.zhijiandao.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://riz.zhiwuduotai.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gnr.gaohongyu789.top

JS:   JSON.stringify(obj)
来源：http://djw.cashguo.top

TS:   JSON.stringify(obj)
来源：http://gcb.gaohongyu789.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fts.dashuyun.cn

Go:   json.Marshal(obj)
来源：http://kdd.pycfn.com

Ruby: obj.to_json                                     // require "json"
来源：http://ruv.vehdjk.com

C#:   JsonSerializer.Serialize(obj)
来源：http://loc.tianlin.xyz

[K02] JSON 字符串转对象
来源：http://hkv.hcnkem.com

Py:   json.loads(s)
来源：http://hja.meibo888.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bvl.yj20258.top

JS:   JSON.parse(s)
来源：http://qnt.uphjek.com

TS:   JSON.parse(s)
来源：http://juu.zycfv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fws.ybcxt.top

Go:   json.Unmarshal(data, &v)
来源：http://ssd.ppjwa.cn

Ruby: JSON.parse(s)
来源：http://vpg.gaohongyu789.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lpz.ywan-chungtsiang.top

[K03] JSON 美化输出（带缩进）
来源：http://kqo.tian-w.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tip.jianghu66.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xxc.guannengcc.top

JS:   JSON.stringify(obj, null, 2)
来源：http://wrd.ybcxt.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wmc.xziqi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yvw.chenlongwang.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fnp.zhoulong.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://nlf.cdnleiting.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hlj.yj20258888.top

[K04] 读取 JSON 文件
来源：http://lgy.c1oappe.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nko.nwbrower.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xzq.yvedp.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cmb.mhx1999.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qgw.chenjidiqi.icu

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ecc.nwbrower.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bdf.tianlin.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://nqm.gaohongyu789.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mqp.jyoumei.cn

[K05] 深拷贝对象
来源：http://qra.yuanzhike.top

Py:   copy.deepcopy(obj)
来源：http://hsl.fktsv.cn

PHP:  unserialize(serialize($obj));
来源：http://kbo.yongpay.top

JS:   structuredClone(obj)
来源：http://cwo.ivvv.top

TS:   structuredClone(obj)
来源：http://fes.xingfuxueyuan.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://tfd.ctjpmb.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hyq.gaohongyu789.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wdy.vehdjk.com

C#:   // 序列化往返，或自定义 Clone
来源：http://jng.hammf.cn

[K06] 解析 URL 查询串
来源：http://pyx.dianchejie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dqk.tanke756.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zkd.vqdsnc.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eas.haohaochexian.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hbx.hysaishi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://apm.cdnleiting.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://zpo.tanke756.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qcj.yonumen.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mkg.sxryk.cn

[K07] 进制转换
来源：http://qhh.yangfankeji.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tzk.cheryme.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hnt.zhijiandao.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://job.yuxming.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mts.vehdjk.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://evo.pycfn.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gkq.zdbjq.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dcv.zhaomingkeji.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nzg.nanxuanxn.top

[K08] 二进制序列化（非 JSON）
来源：http://ynw.ppjwa.cn

Py:   pickle.dumps(obj)
来源：http://nym.zhiwuduotai.top

PHP:  serialize($obj);  unserialize($s);
来源：http://cxr.xziqi.cn

JS:   v8.serialize(obj)        // Node
来源：http://sof.yj202588.top

TS:   v8.serialize(obj)        // Node
来源：http://dcv.ehwqpu.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dsd.c1oappe.top

Go:   encoding/gob
来源：http://auk.hammf.cn

Ruby: Marshal.dump(obj)
来源：http://fpe.yj202588.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yax.cashguo.top

================================================================================
来源：http://vqn.tanke756.top

L. 网络请求
来源：http://fkk.yj20258888.top

================================================================================
来源：http://vhu.fengsongda.top

[L01] 发送 GET 请求
来源：http://vpx.jinghuilouyu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jkn.sysykeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wua.jqgfzy.top

JS:   await fetch(url)
来源：http://xha.9152youxi.cn

TS:   await fetch(url)
来源：http://scs.xuanzx.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hvu.feifeiyinyue.top

Go:   resp, err := http.Get(url)
来源：http://zjp.ybcxt.top

Ruby: Net::HTTP.get(URI(url))
来源：http://tps.kuanghao11.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://eam.wangshuangyany.cn

[L02] 发送 POST JSON
来源：http://yhg.xingfuxueyuan.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://cif.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fai.nanxuanxn.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jjp.jinyuanbaomall.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pkg.tarul.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://reb.fengsongda.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jaj.yonumen.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hko.cqqwz.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xum.jinyuanbaomall.cn

[L03] 设置自定义请求头
来源：http://bvf.pycfn.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://grh.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gnm.ivvv.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xnj.haohaochexian.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ags.svipenyu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wdz.ivvv.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xci.fehbvm.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://smm.jianghu66.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://quc.zhixingplan.top

[L04] 设置超时
来源：http://mlk.tian-w.cn

Py:   requests.get(url, timeout=5)
来源：http://sdd.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mla.aizwys.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vna.kuanghao11.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cwk.wangshuangyany.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zsd.sysykeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qum.pycfn.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://neh.vqdsnc.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qsd.shuidangran.top

[L05] 上传文件（multipart）
来源：http://dxb.xinyue.icu

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uvg.fktsv.cn


<!-- 参考信息 -->