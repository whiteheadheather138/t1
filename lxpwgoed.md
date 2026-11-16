代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hob.wangshuangyany.cn

Ruby: raise MyError.new("fail", 500)
来源：http://blu.xuanzx.com

C#:   // 自定义异常类中加 Code 属性
来源：http://sin.wangshuangyany.cn

[H10] 资源自动释放
来源：http://hlq.jinqigfzy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://eds.shanyushiyangtech.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://trr.52xcode.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://skt.jinqigufen.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://laz.52xcode.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xxt.birdmap.top

Go:   defer f.Close()
来源：http://jda.guowangkeji.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ubk.andypj.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hog.hnqzz.top

================================================================================
来源：http://qbp.kuanghao11.cn

I. 正则表达式
来源：http://ccx.yangfankeji.com

================================================================================
来源：http://tzo.fengsongda.top

[I01] 判断是否匹配
来源：http://vet.aibaodan.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bsv.yueranfly.top

PHP:  preg_match('/\d+/', $s);
来源：http://yrd.sysykeji.top

JS:   /\d+/.test(s)
来源：http://yug.316326.xyz

TS:   /\d+/.test(s)
来源：http://ugj.ppjwa.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hsn.xylfe.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tns.yangfankeji.com

Ruby: s.match?(/\d+/)
来源：http://fmh.ybcxt.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ylv.hongshengwenyu.top

[I02] 提取所有匹配
来源：http://hgx.ydzc1.top

Py:   re.findall(r"\d+", s)
来源：http://odt.sxryk.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yav.9152youxi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mxq.52xcode.cn

TS:   s.match(/\d+/g)
来源：http://jxx.yj202588.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://snf.jqgufenzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nur.xingfuxueyuan.xyz

Ruby: s.scan(/\d+/)
来源：http://iue.dianchejie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qxx.havefunace.top

[I03] 提取捕获分组
来源：http://fzq.cheryme.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hip.zhongyouzk.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kla.sufxvd.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yhz.cucudq.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yec.shanyushiyangkeji.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rad.svipenyu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://srb.epnwcf.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hmf.yfazqb.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zky.sxryk.cn

[I04] 正则替换
来源：http://nof.epnwcf.com

Py:   re.sub(r"\d+", "#", s)
来源：http://gwr.ywan-chungtsiang.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://plv.xinyue.icu

JS:   s.replace(/\d+/g, "#")
来源：http://acc.zhiwuduotai.top

TS:   s.replace(/\d+/g, "#")
来源：http://zgi.cqqwz.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fxn.epnwcf.com

Go:   re.ReplaceAllString(s, "#")
来源：http://jfz.shangyingyoupin.top

Ruby: s.gsub(/\d+/, "#")
来源：http://lfv.xziqi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://doi.nwbrower.top

[I05] 按正则拆分
来源：http://lar.hywenlv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mrz.xylfe.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vnz.daxiang520.top

JS:   s.split(/\s*,\s*/)
来源：http://lul.hammf.cn

TS:   s.split(/\s*,\s*/)
来源：http://qqn.zhongyouzk.top

Java: s.split("\\s*,\\s*")
来源：http://wto.fanxiaobao.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hcv.fktsv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://owj.cashguo.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hhk.andypj.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ovm.quarkkingdee.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://spt.tianlin.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tah.hesvh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qln.daxiang520.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dlh.daxiang520.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zjv.hywenlv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ayo.jianghu66.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://llx.aibaodan.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lvu.yongpay.top

[I07] 忽略大小写与多行模式
来源：http://oka.ydjk.org.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://iym.wangshuangyany.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qyj.meibo888.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kwu.jinqigufen.top

TS:   /error/gim
来源：http://gwc.zycfv.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ijl.zhongyouzk.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hel.jinqigfzy.top

Ruby: s.scan(/error/i)
来源：http://jcy.snrcjt.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vqd.chenlongwang.top

[I08] 贪婪与非贪婪匹配
来源：http://fqe.chenjidiqi.icu

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sfx.yj20258.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dth.jinqigufen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vqx.dashuyun.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pwp.uphjek.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://vxr.daxiang520.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wtm.zhoulong.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://suh.tarul.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rnw.quarkkingdee.top

================================================================================
来源：http://yyv.gotoacloud.top

J. 日期与时间
来源：http://akf.jqgufenzy.top

================================================================================
来源：http://hmf.fktsv.cn

[J01] 获取当前时间
来源：http://txf.zhengqikj.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://mvd.chenzaomai.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dov.cashguo.top

JS:   new Date();  Date.now()
来源：http://rxd.nanxuanxn.top

TS:   new Date();  Date.now()
来源：http://npb.fehbvm.com

Java: LocalDateTime.now();  Instant.now()
来源：http://ggv.nanxuanxn.top

Go:   time.Now()
来源：http://anz.feifeiyinyue.top

Ruby: Time.now
来源：http://kni.chenzaomai.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://grf.mhx1999.top

[J02] 格式化输出
来源：http://ljz.fengsongda.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jba.xinyue.icu

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://azd.pengpengdd.cyou

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bey.uphjek.com

TS:   d.toISOString()
来源：http://wsj.hesvh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lzl.shuidangran.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://enx.birdmap.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://csm.zhaomingkeji.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qtp.yj20258.top

[J03] 字符串解析为日期
来源：http://ydr.yueranfly.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cxk.sufxvd.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://orj.dashuyun.cn

JS:   new Date("2024-01-02")
来源：http://jij.cqqwz.cn

TS:   new Date("2024-01-02")
来源：http://hwa.0kj1m.cn

Java: LocalDate.parse("2024-01-02")
来源：http://akg.chenzaomai.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fyk.zdqjudy.top

Ruby: Date.parse("2024-01-02")
来源：http://haf.dashuyun.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mgd.cqqwz.cn

[J04] 时间戳与日期互转
来源：http://ggf.hesvh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fan.quarkkingdee.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dao.zhiwuduotai.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pco.daria6918.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://obz.sufxvd.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jrp.gaohongyu789.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pnd.mhx1999.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nrv.jinghuilouyu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://awv.hnxiangtu.top

[J05] 时间加减（加 7 天）
来源：http://bnb.fktsv.cn

Py:   now + timedelta(days=7)
来源：http://ygd.dianchejie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://brh.guowangkeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uds.svipenyu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ndj.zycfv.cn

Java: LocalDate.now().plusDays(7)
来源：http://gth.yuxming.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nhj.xuanzx.com

Ruby: Time.now + 7 * 86400
来源：http://uap.feifeiyinyue.top

C#:   DateTime.Now.AddDays(7)
来源：http://kch.jlsjyb.cn

[J06] 计算两时间之差
来源：http://hyh.yangfankeji.com

Py:   (end - start).total_seconds()
来源：http://xwo.52xcode.cn

PHP:  $end->diff($start)->days;
来源：http://ilz.52xcode.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hzt.cashguo.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://foj.yuanzhike.top

Java: Duration.between(start, end).toSeconds()
来源：http://oit.yonumen.top

Go:   end.Sub(start).Hours()
来源：http://mmq.ydjk.org.cn

Ruby: end - start                 # 返回秒数
来源：http://jtj.jinyuanbaomall.cn

C#:   (end - start).TotalSeconds
来源：http://hng.sweek.top

[J07] 比较两个日期
来源：http://hcn.sysykeji.top

Py:   d1 < d2;  d1 == d2
来源：http://vwy.hnxiangtu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pxa.shangyingyoupin.top

JS:   d1.getTime() < d2.getTime()
来源：http://uoz.pengpengdd.cyou

TS:   d1.getTime() < d2.getTime()
来源：http://qvu.gogol.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://syy.zhongyouzk.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cle.smart0.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://fva.yonumen.top

C#:   d1 < d2;  d1 == d2
来源：http://zqr.hesvh.cn

[J08] 提取年月日与星期
来源：http://tzj.zhaomingkeji.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jcj.yueranfly.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xhe.pengpengdd.cyou

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://doy.hywenlv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pct.sysykeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://znd.dashuyun.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://aws.ppjwa.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://leu.sysykeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hgo.xingfuxueyuan.xyz

[J09] 时区处理
来源：http://loo.kuanghao11.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tuh.yonumen.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ikh.jqgufenzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://djf.andypj.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ylj.smart0.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qde.fanxiaobao.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dcc.yangfankeji.com

Ruby: Time.now.getlocal("+08:00")
来源：http://bxy.epnwcf.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blc.feifeiyinyue.top

[J10] 取今天 / 本月第一天
来源：http://urd.bjfxy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://rnz.jinqigufen.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://iig.uphjek.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jeg.hysaishi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://djk.epnwcf.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gjm.nwbrower.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ujs.chenjidiqi.icu

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lki.shuidangran.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ijd.fehbvm.com

================================================================================
来源：http://hld.xylfe.cn

K. JSON 与序列化
来源：http://gvi.fzhhl.top

================================================================================
来源：http://uxl.52xcode.cn

[K01] 对象转 JSON 字符串
来源：http://pvn.sxryk.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lum.mhx1999.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ukr.zhixingplan.top

JS:   JSON.stringify(obj)
来源：http://wjw.316326.xyz

TS:   JSON.stringify(obj)
来源：http://lxw.xuanzx.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ggx.sjlbkw.cn

Go:   json.Marshal(obj)
来源：http://bjx.chenzaomai.com

Ruby: obj.to_json                                     // require "json"
来源：http://kdp.fzhhl.top

C#:   JsonSerializer.Serialize(obj)
来源：http://rqr.9152youxi.cn

[K02] JSON 字符串转对象
来源：http://qpk.yuanzhike.top

Py:   json.loads(s)
来源：http://gyc.cdnleiting.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nez.dianchejie.cn

JS:   JSON.parse(s)
来源：http://mdk.hysaishi.cn

TS:   JSON.parse(s)
来源：http://mhs.cqqwz.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mee.zhijiandao.cn

Go:   json.Unmarshal(data, &v)
来源：http://npa.iojbl.cn

Ruby: JSON.parse(s)
来源：http://cab.xinyue.icu

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gye.xylfe.cn

[K03] JSON 美化输出（带缩进）
来源：http://rif.aizwys.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xkx.shangyingyoupin.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://esp.fanxiaobao.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://hfn.guannengcc.top

TS:   JSON.stringify(obj, null, 2)
来源：http://qwv.tarul.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ooj.c1oappe.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ypw.nanxinkj.top

Ruby: JSON.pretty_generate(obj)
来源：http://lub.ppjwa.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fll.uphjek.com

[K04] 读取 JSON 文件
来源：http://ksq.gzhubu.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qwk.gotoacloud.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dla.yuanzhike.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://osv.daxiang520.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ozm.hnqzz.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fwi.wangdashe.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lha.feifeiyinyue.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://suk.zhixingplan.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oyv.jinqigufen.top

[K05] 深拷贝对象
来源：http://iiq.yj202588.top

Py:   copy.deepcopy(obj)
来源：http://fkz.xingfuxueyuan.xyz

PHP:  unserialize(serialize($obj));
来源：http://ilu.hcnkem.com

JS:   structuredClone(obj)
来源：http://zrm.cucudq.cn

TS:   structuredClone(obj)
来源：http://ymx.shzxlz.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jzo.ppjwa.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ale.dashuyun.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sjd.fzhhl.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ooo.birdmap.top

[K06] 解析 URL 查询串
来源：http://kxe.ydjk.org.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hkx.c1oappe.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nbq.smart0.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zta.316326.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zfg.chenjidiqi.icu

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dah.hongshengwenyu.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://iff.guowangkeji.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gkn.tian-w.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wno.sysykeji.top

[K07] 进制转换
来源：http://ygd.sjlbkw.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://anu.xuanzx.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tzp.yanxiufei.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bsl.nanxuanxn.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tpa.fengsongda.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rzd.shangyingyoupin.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://aut.nanxuanxn.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ghi.havefunace.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ois.yonumen.top

[K08] 二进制序列化（非 JSON）
来源：http://aan.daria6918.cn

Py:   pickle.dumps(obj)
来源：http://riq.xuetiantiany.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wqb.birdmap.top

JS:   v8.serialize(obj)        // Node
来源：http://sdh.vqdsnc.cn

TS:   v8.serialize(obj)        // Node
来源：http://ejb.tarul.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ryi.yangfankeji.com

Go:   encoding/gob
来源：http://mhg.haohaochexian.top

Ruby: Marshal.dump(obj)
来源：http://nxb.hysaishi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://phr.fktsv.cn

================================================================================
来源：http://sjc.ppjwa.cn

L. 网络请求
来源：http://tkt.tianlin.xyz

================================================================================
来源：http://lsj.yvedp.cn

[L01] 发送 GET 请求
来源：http://mqj.ctjpmb.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://iyu.gotoacloud.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lch.bbcook.cn

JS:   await fetch(url)
来源：http://uet.shanyushiyangtech.top

TS:   await fetch(url)
来源：http://crr.cdnleiting.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mzv.cashguo.top

Go:   resp, err := http.Get(url)
来源：http://bdg.yj20258.top

Ruby: Net::HTTP.get(URI(url))
来源：http://uwd.nanxinkj.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dek.yj202588.top

[L02] 发送 POST JSON
来源：http://ykt.fzhhl.top

Py:   requests.post(url, json={"a": 1})
来源：http://qrz.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://esv.316326.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://heq.xuetiantiany.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aej.316326.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bwn.fanxiaobao.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kjr.sysykeji.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zjf.jianghu66.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ogq.xingfuxueyuan.xyz

[L03] 设置自定义请求头
来源：http://iph.hongshengwenyu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ftc.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://eip.ppjwa.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sdr.cucudq.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://npj.wangdashe.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ujb.zhijiandao.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uwu.havefunace.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://icb.meibo888.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qrw.tianlin.xyz

[L04] 设置超时
来源：http://yuo.tarul.cn

Py:   requests.get(url, timeout=5)
来源：http://gnw.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://utd.zhixingplan.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cel.yvedp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cjq.ppjwa.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qxj.jianghu66.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ehr.jinghuilouyu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://llp.jinghuilouyu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://joo.gotoacloud.top

[L05] 上传文件（multipart）
来源：http://kvy.yanxiufei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wcb.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://szz.gaohongyu789.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://msj.yj20258888.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cnf.jinghuilouyu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rfs.guannengcc.top


<!-- 参考信息 -->