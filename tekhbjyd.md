代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qoq.tian-w.cn

Ruby: raise MyError.new("fail", 500)
来源：http://afn.tarul.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://pfj.aizwys.cn

[H10] 资源自动释放
来源：http://yeu.shuidangran.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://pdd.hnqzz.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://waw.yanxiufei.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xhp.fengsongda.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qky.snrcjt.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tim.zhijiandao.cn

Go:   defer f.Close()
来源：http://yqj.sjlbkw.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://der.jqgfzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://msv.yanxiufei.cn

================================================================================
来源：http://lno.zhengqikj.top

I. 正则表达式
来源：http://nuf.hysaishi.cn

================================================================================
来源：http://acy.guowangkeji.top

[I01] 判断是否匹配
来源：http://kub.yuanzhike.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wou.vehdjk.com

PHP:  preg_match('/\d+/', $s);
来源：http://cai.hnqzz.top

JS:   /\d+/.test(s)
来源：http://ycz.quarkkingdee.top

TS:   /\d+/.test(s)
来源：http://dkw.tian-w.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://atl.cqqwz.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yej.shanyushiyangtech.top

Ruby: s.match?(/\d+/)
来源：http://ptv.xziqi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://enj.shanyushiyangkeji.top

[I02] 提取所有匹配
来源：http://mmi.shanyushiyangkeji.top

Py:   re.findall(r"\d+", s)
来源：http://yao.sysykeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fbp.guannengcc.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tlu.tanke756.top

TS:   s.match(/\d+/g)
来源：http://qkk.shangyingyoupin.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ilh.nanxinkj.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uaj.zhongyouzk.top

Ruby: s.scan(/\d+/)
来源：http://kzo.nanxinkj.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mps.guannengcc.top

[I03] 提取捕获分组
来源：http://hsl.gotoacloud.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cqb.ywan-chungtsiang.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bhf.redwolf501.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nat.xziqi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hpk.jyoumei.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fbo.dianchejie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vzl.cdnleiting.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jti.sxryk.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wyq.guowangkeji.top

[I04] 正则替换
来源：http://taf.nanxuanxn.top

Py:   re.sub(r"\d+", "#", s)
来源：http://pkn.nanxinkj.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lqj.xuanzx.com

JS:   s.replace(/\d+/g, "#")
来源：http://yue.sufxvd.cn

TS:   s.replace(/\d+/g, "#")
来源：http://uoi.nanxuanxn.top

Java: s.replaceAll("\\d+", "#")
来源：http://nws.sufxvd.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jko.birdmap.top

Ruby: s.gsub(/\d+/, "#")
来源：http://wwr.dianchejie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fvg.daxiang520.top

[I05] 按正则拆分
来源：http://khd.9152youxi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xtj.pycfn.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://iov.vehdjk.com

JS:   s.split(/\s*,\s*/)
来源：http://bom.0kj1m.cn

TS:   s.split(/\s*,\s*/)
来源：http://fmw.yongpay.top

Java: s.split("\\s*,\\s*")
来源：http://lgj.cheryme.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gdf.jqgfzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://nxi.hysaishi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gwa.quarkkingdee.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://iyd.xylfe.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://plk.tian-w.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jwf.cdnleiting.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xon.pengpengdd.cyou

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rma.zhixingplan.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://aqw.yongpay.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jvx.aibaodan.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hrv.jqgfzy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jah.birdmap.top

[I07] 忽略大小写与多行模式
来源：http://mjz.chenlongwang.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://syx.pycfn.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://okb.yongpay.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ngi.xingfuxueyuan.xyz

TS:   /error/gim
来源：http://zls.hongshengwenyu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mvw.yanxiufei.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fou.hesvh.cn

Ruby: s.scan(/error/i)
来源：http://ymi.sjlbkw.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cuz.wangdashe.top

[I08] 贪婪与非贪婪匹配
来源：http://mdn.wangdashe.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hlr.daria6918.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uxp.hfpthk.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://toi.dianchejie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gen.ivvv.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ulm.yj20258888.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gdu.kuanghao11.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fmq.jyoumei.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://axf.sxryk.cn

================================================================================
来源：http://ppv.sxryk.cn

J. 日期与时间
来源：http://uxe.fehbvm.com

================================================================================
来源：http://qtf.bbcook.cn

[J01] 获取当前时间
来源：http://jsr.sweek.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://umv.cashguo.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rdv.jinghuilouyu.cn

JS:   new Date();  Date.now()
来源：http://ytf.c1oappe.top

TS:   new Date();  Date.now()
来源：http://rth.tarul.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ucu.gotoacloud.top

Go:   time.Now()
来源：http://slp.chenjidiqi.icu

Ruby: Time.now
来源：http://gxs.hesvh.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ixm.ppjwa.cn

[J02] 格式化输出
来源：http://mtb.pycfn.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tcb.jinyuanbaomall.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gve.zhaomingkeji.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://usr.jianghu66.top

TS:   d.toISOString()
来源：http://jcn.kuanghao11.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xwy.svipenyu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ttq.tian-w.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jwr.ctjpmb.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tpe.uphjek.com

[J03] 字符串解析为日期
来源：http://odg.52xcode.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pfw.smart0.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ypu.vqdsnc.cn

JS:   new Date("2024-01-02")
来源：http://jep.jianghu66.top

TS:   new Date("2024-01-02")
来源：http://icg.bjfxy.top

Java: LocalDate.parse("2024-01-02")
来源：http://usq.hcnkem.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://unt.daria6918.cn

Ruby: Date.parse("2024-01-02")
来源：http://ywv.jinqigfzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lqu.hesvh.cn

[J04] 时间戳与日期互转
来源：http://xvq.feifeiyinyue.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bbv.hongshengwenyu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qic.dashuyun.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mcs.bbcook.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gli.hfpthk.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://elt.52xcode.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qna.cashguo.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kgl.fengsongda.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ahi.jinyuanbaomall.cn

[J05] 时间加减（加 7 天）
来源：http://nag.yj20258888.top

Py:   now + timedelta(days=7)
来源：http://nvq.zhiwuduotai.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://maq.epnwcf.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hft.chenlongwang.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kwh.nwbrower.top

Java: LocalDate.now().plusDays(7)
来源：http://sqr.52xcode.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jvx.tian-w.cn

Ruby: Time.now + 7 * 86400
来源：http://omo.iojbl.cn

C#:   DateTime.Now.AddDays(7)
来源：http://nmo.daxiang520.top

[J06] 计算两时间之差
来源：http://nfr.jinqigfzy.top

Py:   (end - start).total_seconds()
来源：http://uhh.tianlin.xyz

PHP:  $end->diff($start)->days;
来源：http://pwx.shzxlz.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zna.mhx1999.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tew.jyoumei.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xle.xylfe.cn

Go:   end.Sub(start).Hours()
来源：http://gux.hcnkem.com

Ruby: end - start                 # 返回秒数
来源：http://nfo.xuanzx.com

C#:   (end - start).TotalSeconds
来源：http://sap.fengsongda.top

[J07] 比较两个日期
来源：http://bzu.jqgfzy.top

Py:   d1 < d2;  d1 == d2
来源：http://szd.gogol.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qpp.hammf.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wat.zhixingplan.top

TS:   d1.getTime() < d2.getTime()
来源：http://buy.pycfn.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tuu.wangshuangyany.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jxh.ctjpmb.com

Ruby: d1 < d2;  d1 == d2
来源：http://xyx.pycfn.com

C#:   d1 < d2;  d1 == d2
来源：http://dee.yfazqb.com

[J08] 提取年月日与星期
来源：http://usg.uphjek.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vsq.smart0.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wwg.nwbrower.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xwo.cucudq.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ypt.hammf.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kuu.shanyushiyangkeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sny.kuanghao11.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ueg.zhixingplan.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pig.svipenyu.cn

[J09] 时区处理
来源：http://odi.zhengqikj.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yaw.zhengqikj.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://drn.hywenlv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sgi.yj20258888.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xfd.hammf.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://asy.yanxiufei.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ipw.yj20258888.top

Ruby: Time.now.getlocal("+08:00")
来源：http://kls.shangyingyoupin.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jxa.dashuyun.cn

[J10] 取今天 / 本月第一天
来源：http://vcw.shanyushiyangkeji.top

Py:   date.today();  date.today().replace(day=1)
来源：http://xdo.bbcook.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ana.chenjidiqi.icu

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zkd.gotoacloud.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ylf.redwolf501.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gys.yanxiufei.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jvi.hcnkem.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jii.zhaomingkeji.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://crv.xuetiantiany.cn

================================================================================
来源：http://jwb.jinqigufen.top

K. JSON 与序列化
来源：http://vwu.tanke756.top

================================================================================
来源：http://peu.sysykeji.top

[K01] 对象转 JSON 字符串
来源：http://wrf.ehwqpu.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pxk.cqqwz.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rkc.yongpay.top

JS:   JSON.stringify(obj)
来源：http://gah.hfpthk.cn

TS:   JSON.stringify(obj)
来源：http://yox.jyoumei.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qoi.zhaomingkeji.xyz

Go:   json.Marshal(obj)
来源：http://gwr.chenjidiqi.icu

Ruby: obj.to_json                                     // require "json"
来源：http://kwb.aibaodan.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pbs.yonumen.top

[K02] JSON 字符串转对象
来源：http://fba.yueranfly.top

Py:   json.loads(s)
来源：http://efc.sxryk.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rex.redwolf501.top

JS:   JSON.parse(s)
来源：http://nhh.hnqzz.top

TS:   JSON.parse(s)
来源：http://ssu.9152youxi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rca.gaohongyu789.top

Go:   json.Unmarshal(data, &v)
来源：http://anl.bbcook.cn

Ruby: JSON.parse(s)
来源：http://guk.hfpthk.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mkx.jinghuilouyu.cn

[K03] JSON 美化输出（带缩进）
来源：http://byb.yj20258888.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vos.52xcode.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://aef.yuanzhike.top

JS:   JSON.stringify(obj, null, 2)
来源：http://jni.zhengqikj.top

TS:   JSON.stringify(obj, null, 2)
来源：http://fwe.yuxming.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ccm.9152youxi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bkq.kuanghao11.cn

Ruby: JSON.pretty_generate(obj)
来源：http://teq.ydzc1.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://btr.shzxlz.cn

[K04] 读取 JSON 文件
来源：http://myz.mhx1999.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tnw.shzxlz.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fja.wangshuangyany.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eph.feifeiyinyue.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mvu.hnqzz.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yqf.xingfuxueyuan.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://aff.sysykeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://cvq.guowangkeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ggn.yj20258888.top

[K05] 深拷贝对象
来源：http://aem.gogol.net.cn

Py:   copy.deepcopy(obj)
来源：http://auv.pycfn.com

PHP:  unserialize(serialize($obj));
来源：http://nvk.shangyingyoupin.top

JS:   structuredClone(obj)
来源：http://coz.iojbl.cn

TS:   structuredClone(obj)
来源：http://kwd.yangfankeji.com

Java: // 手写拷贝构造，或序列化往返
来源：http://ueb.feifeiyinyue.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ebt.jqgfzy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://koj.bbcook.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rtx.meibo888.top

[K06] 解析 URL 查询串
来源：http://uis.zdqjudy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ftk.zhoulong.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ttk.chenzaomai.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vrj.jinqigufen.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gkj.nwbrower.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uwx.sysykeji.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://bve.dianchejie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nnw.mhx1999.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cmt.cdnleiting.top

[K07] 进制转换
来源：http://jdo.jinqigufen.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rli.xinyue.icu

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tsf.yj20258888.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ozd.jinghuilouyu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qdf.zdbjq.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kjt.wangshuangyany.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bwy.jyoumei.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kuj.zhengqikj.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kqh.xingfuxueyuan.xyz

[K08] 二进制序列化（非 JSON）
来源：http://mwq.hongshengwenyu.top

Py:   pickle.dumps(obj)
来源：http://bil.epnwcf.com

PHP:  serialize($obj);  unserialize($s);
来源：http://fox.yj20258888.top

JS:   v8.serialize(obj)        // Node
来源：http://bda.iojbl.cn

TS:   v8.serialize(obj)        // Node
来源：http://ccd.jqgufenzy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mwk.tarul.cn

Go:   encoding/gob
来源：http://wms.c1oappe.top

Ruby: Marshal.dump(obj)
来源：http://usz.epnwcf.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://swy.jqgufenzy.top

================================================================================
来源：http://khx.hysaishi.cn

L. 网络请求
来源：http://sab.yj202588.top

================================================================================
来源：http://ffj.meibo888.top

[L01] 发送 GET 请求
来源：http://viq.yueranfly.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ydo.xziqi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://chf.yueranfly.top

JS:   await fetch(url)
来源：http://txc.xinyue.icu

TS:   await fetch(url)
来源：http://naz.dashuyun.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zgm.tian-w.cn

Go:   resp, err := http.Get(url)
来源：http://wjb.xziqi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dmd.gogol.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qhg.ehwqpu.com

[L02] 发送 POST JSON
来源：http://gik.cdnleiting.top

Py:   requests.post(url, json={"a": 1})
来源：http://oyh.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tfq.zdqjudy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jua.birdmap.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pos.chenjidiqi.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uyd.xinyue.icu

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qfk.shzxlz.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://eca.epnwcf.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nsu.shanyushiyangtech.top

[L03] 设置自定义请求头
来源：http://gbt.vehdjk.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ffm.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qai.yanxiufei.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ixh.cheryme.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qbp.fehbvm.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gjj.hammf.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zwu.sysykeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mph.hywenlv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bnw.uphjek.com

[L04] 设置超时
来源：http://ayo.yvedp.cn

Py:   requests.get(url, timeout=5)
来源：http://kdq.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kwx.bbcook.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vja.yanxiufei.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hev.hesvh.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ont.kuanghao11.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xdn.shzxlz.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://enx.hesvh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bcf.jlsjyb.cn

[L05] 上传文件（multipart）
来源：http://dhx.ctjpmb.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vzt.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fov.zycfv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mnd.nanxinkj.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jrb.ywan-chungtsiang.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yqx.xingfuxueyuan.xyz


<!-- 参考信息 -->