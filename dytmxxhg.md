代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qxz.cheryme.top

Go:   defer f.Close()
来源：http://qqm.chenjidiqi.icu

Ruby: File.open("a.txt") { |f| f.read }
来源：http://drl.pengpengdd.cyou

C#:   using var stream = File.OpenRead("a.txt");
来源：http://awi.sxryk.cn

================================================================================
来源：http://kdg.ydzc1.top

I. 正则表达式
来源：http://hks.52xcode.cn

================================================================================
来源：http://vok.ybcxt.top

[I01] 判断是否匹配
来源：http://udb.hcnkem.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hcq.mhx1999.top

PHP:  preg_match('/\d+/', $s);
来源：http://qsg.xylfe.cn

JS:   /\d+/.test(s)
来源：http://vep.sufxvd.cn

TS:   /\d+/.test(s)
来源：http://kcp.cdnleiting.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ioh.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qvd.jqgufenzy.top

Ruby: s.match?(/\d+/)
来源：http://lrj.zhongyouzk.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hmg.sweek.top

[I02] 提取所有匹配
来源：http://sdl.daxiang520.top

Py:   re.findall(r"\d+", s)
来源：http://umq.sxryk.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ler.pengpengdd.cyou

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cto.ydzc1.top

TS:   s.match(/\d+/g)
来源：http://dqj.pycfn.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ohd.nanxinkj.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jlx.zhiwuduotai.top

Ruby: s.scan(/\d+/)
来源：http://axe.zhongyouzk.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://srm.chenjidiqi.icu

[I03] 提取捕获分组
来源：http://txo.chenjidiqi.icu

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cnr.nanxinkj.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mct.ybcxt.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pph.quarkkingdee.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xkk.ybcxt.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://esh.aibaodan.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lvq.nanxinkj.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://buh.hfpthk.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jvd.hnqzz.top

[I04] 正则替换
来源：http://eun.tian-w.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://cnt.hcnkem.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://iln.birdmap.top

JS:   s.replace(/\d+/g, "#")
来源：http://wzn.quarkkingdee.top

TS:   s.replace(/\d+/g, "#")
来源：http://ycn.redwolf501.top

Java: s.replaceAll("\\d+", "#")
来源：http://hrx.svipenyu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fen.havefunace.top

Ruby: s.gsub(/\d+/, "#")
来源：http://whj.yuxming.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jqk.yj202588.top

[I05] 按正则拆分
来源：http://yuq.yj20258.top

Py:   re.split(r"\s*,\s*", s)
来源：http://wrv.smart0.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hlk.zhijiandao.cn

JS:   s.split(/\s*,\s*/)
来源：http://zuo.wangdashe.top

TS:   s.split(/\s*,\s*/)
来源：http://ppw.feifeiyinyue.top

Java: s.split("\\s*,\\s*")
来源：http://aym.snrcjt.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uwo.gaohongyu789.top

Ruby: s.split(/\s*,\s*/)
来源：http://dqk.sxryk.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://iza.jinyuanbaomall.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kbz.meibo888.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wpc.yj202588.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mth.ybcxt.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wae.shanyushiyangtech.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lys.hysaishi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wzk.smart0.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pij.chenjidiqi.icu

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fsw.xuetiantiany.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vvg.andypj.xyz

[I07] 忽略大小写与多行模式
来源：http://arv.yj20258888.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cxk.zdbjq.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jhl.jinqigfzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://veo.sysykeji.top

TS:   /error/gim
来源：http://hyg.daxiang520.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kok.nanxinkj.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xkc.nanxuanxn.top

Ruby: s.scan(/error/i)
来源：http://lef.quarkkingdee.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ikm.vqdsnc.cn

[I08] 贪婪与非贪婪匹配
来源：http://oof.chenjidiqi.icu

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fqt.jqgufenzy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wih.gotoacloud.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dmy.ctjpmb.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://noe.fengsongda.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://yxm.havefunace.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yya.chenlongwang.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zbt.zhengqikj.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rpb.chenlongwang.top

================================================================================
来源：http://wlc.yj20258.top

J. 日期与时间
来源：http://vbs.mhx1999.top

================================================================================
来源：http://bgd.zdbjq.cn

[J01] 获取当前时间
来源：http://zdc.aizwys.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://flo.shanyushiyangkeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hxp.jinqigufen.top

JS:   new Date();  Date.now()
来源：http://ahm.dianchejie.cn

TS:   new Date();  Date.now()
来源：http://zze.zdqjudy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://btz.wangdashe.top

Go:   time.Now()
来源：http://uow.xingfuxueyuan.xyz

Ruby: Time.now
来源：http://cij.gogol.net.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mmh.birdmap.top

[J02] 格式化输出
来源：http://eeu.uphjek.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zln.meibo888.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dhv.shanyushiyangtech.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dzc.xziqi.cn

TS:   d.toISOString()
来源：http://bzu.epnwcf.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ihj.uphjek.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://oxb.ywan-chungtsiang.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uwv.shuidangran.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nbj.jqgfzy.top

[J03] 字符串解析为日期
来源：http://eea.guowangkeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fxu.shuidangran.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qeh.daxiang520.top

JS:   new Date("2024-01-02")
来源：http://ftv.c1oappe.top

TS:   new Date("2024-01-02")
来源：http://sxp.bbcook.cn

Java: LocalDate.parse("2024-01-02")
来源：http://sfg.hesvh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kwm.xinyue.icu

Ruby: Date.parse("2024-01-02")
来源：http://bwe.cdnleiting.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hfs.hongshengwenyu.top

[J04] 时间戳与日期互转
来源：http://mlm.meibo888.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rax.uphjek.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://byh.havefunace.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mey.redwolf501.top

TS:   Math.floor(Date.now() / 1000)
来源：http://fip.yuanzhike.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hqk.zhoulong.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sbn.svipenyu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hfy.yj20258888.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://myu.bjfxy.top

[J05] 时间加减（加 7 天）
来源：http://qbz.yuxming.cn

Py:   now + timedelta(days=7)
来源：http://bix.zhoulong.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://gkc.epnwcf.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wxn.hammf.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yrn.yangfankeji.com

Java: LocalDate.now().plusDays(7)
来源：http://lee.jinqigfzy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zzj.cqqwz.cn

Ruby: Time.now + 7 * 86400
来源：http://iyj.jyoumei.cn

C#:   DateTime.Now.AddDays(7)
来源：http://egr.xingfuxueyuan.xyz

[J06] 计算两时间之差
来源：http://zxl.guowangkeji.top

Py:   (end - start).total_seconds()
来源：http://tld.svipenyu.cn

PHP:  $end->diff($start)->days;
来源：http://fum.yuanzhike.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blo.ivvv.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dum.vqdsnc.cn

Java: Duration.between(start, end).toSeconds()
来源：http://tis.jqgfzy.top

Go:   end.Sub(start).Hours()
来源：http://clu.yuanzhike.top

Ruby: end - start                 # 返回秒数
来源：http://sbs.gotoacloud.top

C#:   (end - start).TotalSeconds
来源：http://eew.fktsv.cn

[J07] 比较两个日期
来源：http://due.nanxuanxn.top

Py:   d1 < d2;  d1 == d2
来源：http://mmz.316326.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wtd.hnqzz.top

JS:   d1.getTime() < d2.getTime()
来源：http://itf.gaohongyu789.top

TS:   d1.getTime() < d2.getTime()
来源：http://nnp.sysykeji.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wnt.ydjk.org.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://aup.bjfxy.top

Ruby: d1 < d2;  d1 == d2
来源：http://gut.hnqzz.top

C#:   d1 < d2;  d1 == d2
来源：http://yvk.ydjk.org.cn

[J08] 提取年月日与星期
来源：http://eng.yj20258.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ayj.aibaodan.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://eyo.jianghu66.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://seq.shuidangran.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ffw.shzxlz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lec.sufxvd.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jlb.yj20258888.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nnp.xziqi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rmh.tianlin.xyz

[J09] 时区处理
来源：http://ekl.guowangkeji.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tjm.0kj1m.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rmw.haohaochexian.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ant.zhaomingkeji.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://alb.xuetiantiany.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dlx.ydzc1.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ywz.yvedp.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://eft.pycfn.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pcj.wangdashe.top

[J10] 取今天 / 本月第一天
来源：http://tle.shangyingyoupin.top

Py:   date.today();  date.today().replace(day=1)
来源：http://zdr.ivvv.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vya.meibo888.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://med.zdqjudy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iwu.kuanghao11.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cqr.yj202588.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hkl.shanyushiyangkeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ral.zhengqikj.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fzw.jinghuilouyu.cn

================================================================================
来源：http://xww.fanxiaobao.xyz

K. JSON 与序列化
来源：http://gnv.ctjpmb.com

================================================================================
来源：http://rfw.wangshuangyany.cn

[K01] 对象转 JSON 字符串
来源：http://gwh.hammf.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vpo.ybcxt.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://crn.ivvv.top

JS:   JSON.stringify(obj)
来源：http://vjl.ctjpmb.com

TS:   JSON.stringify(obj)
来源：http://obz.feifeiyinyue.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wli.jqgufenzy.top

Go:   json.Marshal(obj)
来源：http://oud.hammf.cn

Ruby: obj.to_json                                     // require "json"
来源：http://oyt.nwbrower.top

C#:   JsonSerializer.Serialize(obj)
来源：http://mzj.feifeiyinyue.top

[K02] JSON 字符串转对象
来源：http://owp.fehbvm.com

Py:   json.loads(s)
来源：http://jak.jiagoushi.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dbm.52xcode.cn

JS:   JSON.parse(s)
来源：http://llu.mhx1999.top

TS:   JSON.parse(s)
来源：http://dqp.chenjidiqi.icu

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mgh.sjlbkw.cn

Go:   json.Unmarshal(data, &v)
来源：http://lab.zhixingplan.top

Ruby: JSON.parse(s)
来源：http://urk.fehbvm.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xoi.52xcode.cn

[K03] JSON 美化输出（带缩进）
来源：http://yrl.ywan-chungtsiang.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bwo.zhixingplan.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mmf.jqgufenzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://hwe.zhiwuduotai.top

TS:   JSON.stringify(obj, null, 2)
来源：http://cul.snrcjt.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vut.cucudq.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mtl.nanxuanxn.top

Ruby: JSON.pretty_generate(obj)
来源：http://jzm.aizwys.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cua.daria6918.cn

[K04] 读取 JSON 文件
来源：http://kfi.316326.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fqn.316326.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nai.ywan-chungtsiang.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tnc.hcnkem.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lnl.yonumen.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://oje.pengpengdd.cyou

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zqr.yangfankeji.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://gjc.c1oappe.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fyb.aizwys.cn

[K05] 深拷贝对象
来源：http://muu.ivvv.top

Py:   copy.deepcopy(obj)
来源：http://yyk.ydjk.org.cn

PHP:  unserialize(serialize($obj));
来源：http://afh.zdqjudy.top

JS:   structuredClone(obj)
来源：http://gdd.yfazqb.com

TS:   structuredClone(obj)
来源：http://ypz.ehwqpu.com

Java: // 手写拷贝构造，或序列化往返
来源：http://eqx.meibo888.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zip.xuanzx.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tbk.ydzc1.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ejy.jianghu66.top

[K06] 解析 URL 查询串
来源：http://ecx.sjlbkw.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pkz.ydjk.org.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dbb.jinqigfzy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vtk.dianchejie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bvc.jyoumei.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ixs.dianchejie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://khb.guowangkeji.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mkf.tarul.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dxm.yonumen.top

[K07] 进制转换
来源：http://gso.ybcxt.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ddh.jinghuilouyu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dnb.ivvv.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sts.zhiwuduotai.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cpj.birdmap.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nvk.zhaomingkeji.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jxe.yangfankeji.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dww.yj202588.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rfx.yuxming.cn

[K08] 二进制序列化（非 JSON）
来源：http://piy.jinghuilouyu.cn

Py:   pickle.dumps(obj)
来源：http://xcq.zdbjq.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rff.snrcjt.cn

JS:   v8.serialize(obj)        // Node
来源：http://rhn.yuanzhike.top

TS:   v8.serialize(obj)        // Node
来源：http://cse.hnqzz.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://juv.zhengqikj.top

Go:   encoding/gob
来源：http://tar.redwolf501.top

Ruby: Marshal.dump(obj)
来源：http://dyg.xuanzx.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fos.xziqi.cn

================================================================================
来源：http://txn.meibo888.top

L. 网络请求
来源：http://zjp.guowangkeji.top

================================================================================
来源：http://yxi.daxiang520.top

[L01] 发送 GET 请求
来源：http://mco.sjlbkw.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pzw.cdnleiting.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dxh.gotoacloud.top

JS:   await fetch(url)
来源：http://nbf.hfpthk.cn

TS:   await fetch(url)
来源：http://qhl.nwbrower.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oqr.jinqigfzy.top

Go:   resp, err := http.Get(url)
来源：http://cyd.shzxlz.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://eta.yanxiufei.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kyc.daxiang520.top

[L02] 发送 POST JSON
来源：http://soa.yuanzhike.top

Py:   requests.post(url, json={"a": 1})
来源：http://iwe.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ckp.nwbrower.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lox.c1oappe.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ufg.zdbjq.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bfg.guannengcc.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gzr.redwolf501.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rby.ehwqpu.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yaw.jyoumei.cn

[L03] 设置自定义请求头
来源：http://zjr.zhengqikj.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mtr.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cfe.sjlbkw.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hoj.yuxming.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://djn.jiagoushi.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qfq.jlsjyb.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fak.sxryk.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dzo.cheryme.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xfp.9152youxi.cn

[L04] 设置超时
来源：http://sqg.aibaodan.cn

Py:   requests.get(url, timeout=5)
来源：http://bfj.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://otl.fzhhl.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://moy.smart0.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://obu.hysaishi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rmj.yj20258888.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tnx.sweek.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wim.ppjwa.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://oij.sweek.top

[L05] 上传文件（multipart）
来源：http://xqj.ctjpmb.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rdt.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nvy.gotoacloud.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://njw.feifeiyinyue.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wrp.bjfxy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vfs.yangfankeji.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gsf.vehdjk.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://reb.cucudq.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cbl.yueranfly.top

[L06] 解析响应为 JSON
来源：http://gcq.dianchejie.cn

Py:   resp.json()
来源：http://moc.yj20258.top

PHP:  json_decode($body, true);
来源：http://eou.zhixingplan.top

JS:   await resp.json()
来源：http://vrm.52xcode.cn

TS:   await resp.json()
来源：http://fam.sweek.top


<!-- 参考信息 -->