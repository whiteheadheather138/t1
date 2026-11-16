代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zfp.yfazqb.com

Go:   defer f.Close()
来源：http://oqp.daria6918.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uoo.yj20258.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qld.guannengcc.top

================================================================================
来源：http://dtl.hongshengwenyu.top

I. 正则表达式
来源：http://asq.jinghuilouyu.cn

================================================================================
来源：http://gsl.bjfxy.top

[I01] 判断是否匹配
来源：http://byd.hcnkem.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zqe.chenjidiqi.icu

PHP:  preg_match('/\d+/', $s);
来源：http://web.uphjek.com

JS:   /\d+/.test(s)
来源：http://lfv.ehwqpu.com

TS:   /\d+/.test(s)
来源：http://ngi.wangshuangyany.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hqt.jinqigufen.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ewv.nanxuanxn.top

Ruby: s.match?(/\d+/)
来源：http://bla.sysykeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tbc.c1oappe.top

[I02] 提取所有匹配
来源：http://zuk.yonumen.top

Py:   re.findall(r"\d+", s)
来源：http://gft.xziqi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jqj.nanxuanxn.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ndy.sxryk.cn

TS:   s.match(/\d+/g)
来源：http://xjr.ehwqpu.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zap.yongpay.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dck.yueranfly.top

Ruby: s.scan(/\d+/)
来源：http://nyp.zhixingplan.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rnu.tian-w.cn

[I03] 提取捕获分组
来源：http://gok.zhiwuduotai.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yix.yanxiufei.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://avd.jianghu66.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rje.meibo888.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xax.xylfe.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lrs.hfpthk.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xkz.zhiwuduotai.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dsx.gotoacloud.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zam.hysaishi.cn

[I04] 正则替换
来源：http://vmx.yuanzhike.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ziu.fehbvm.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wqv.hfpthk.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zdn.sufxvd.cn

TS:   s.replace(/\d+/g, "#")
来源：http://gyk.feifeiyinyue.top

Java: s.replaceAll("\\d+", "#")
来源：http://nkw.ybcxt.top

Go:   re.ReplaceAllString(s, "#")
来源：http://axc.jinghuilouyu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zjp.hfpthk.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tnm.zhongyouzk.top

[I05] 按正则拆分
来源：http://wmm.daria6918.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://onn.haohaochexian.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dab.ybcxt.top

JS:   s.split(/\s*,\s*/)
来源：http://kfg.yfazqb.com

TS:   s.split(/\s*,\s*/)
来源：http://xbv.yanxiufei.cn

Java: s.split("\\s*,\\s*")
来源：http://nfq.xinyue.icu

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gre.9152youxi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gqq.ehwqpu.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jsn.52xcode.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ncg.yonumen.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hdb.birdmap.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://roc.svipenyu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mhh.xziqi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ywd.zhiwuduotai.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rux.ybcxt.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ayy.hnxiangtu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ybv.tian-w.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ceh.sufxvd.cn

[I07] 忽略大小写与多行模式
来源：http://jwy.andypj.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nen.havefunace.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xkf.xylfe.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cby.shanyushiyangkeji.top

TS:   /error/gim
来源：http://ddi.jinqigfzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wld.zycfv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kuy.yj20258888.top

Ruby: s.scan(/error/i)
来源：http://uic.hesvh.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zkr.zhaomingkeji.xyz

[I08] 贪婪与非贪婪匹配
来源：http://hwj.tanke756.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://foc.jlsjyb.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://eoz.gaohongyu789.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xns.xinyue.icu

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ueu.zdbjq.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lhv.shanyushiyangkeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nwh.hongshengwenyu.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cyy.chenzaomai.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ltl.shanyushiyangkeji.top

================================================================================
来源：http://hkj.cashguo.top

J. 日期与时间
来源：http://dmr.jyoumei.cn

================================================================================
来源：http://cry.yongpay.top

[J01] 获取当前时间
来源：http://xgc.c1oappe.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://zrb.chenlongwang.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cqi.uphjek.com

JS:   new Date();  Date.now()
来源：http://ehn.ydjk.org.cn

TS:   new Date();  Date.now()
来源：http://kbq.yongpay.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ybd.jlsjyb.cn

Go:   time.Now()
来源：http://iym.52xcode.cn

Ruby: Time.now
来源：http://dur.haohaochexian.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uqa.52xcode.cn

[J02] 格式化输出
来源：http://qst.jlsjyb.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jxo.yj202588.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rio.zhengqikj.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zwj.xinyue.icu

TS:   d.toISOString()
来源：http://ahj.pycfn.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vtu.chenlongwang.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ryz.shanyushiyangtech.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vbt.redwolf501.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wto.jinyuanbaomall.cn

[J03] 字符串解析为日期
来源：http://lsf.zdqjudy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zoy.shangyingyoupin.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vrn.gogol.net.cn

JS:   new Date("2024-01-02")
来源：http://yzw.ydzc1.top

TS:   new Date("2024-01-02")
来源：http://hqi.iojbl.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yfb.xuetiantiany.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://udv.smart0.xyz

Ruby: Date.parse("2024-01-02")
来源：http://gss.zdqjudy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dvf.nwbrower.top

[J04] 时间戳与日期互转
来源：http://kwm.jyoumei.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iim.chenzaomai.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dif.snrcjt.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hfe.wangshuangyany.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://byo.ydjk.org.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hyx.ppjwa.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rrg.jqgufenzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mdt.shanyushiyangtech.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://inn.shzxlz.cn

[J05] 时间加减（加 7 天）
来源：http://hnp.yuxming.cn

Py:   now + timedelta(days=7)
来源：http://zsk.meibo888.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ipa.cdnleiting.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dgt.daxiang520.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ytq.uphjek.com

Java: LocalDate.now().plusDays(7)
来源：http://gjt.shzxlz.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://isa.hywenlv.cn

Ruby: Time.now + 7 * 86400
来源：http://oav.zdbjq.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jvk.xuanzx.com

[J06] 计算两时间之差
来源：http://ezd.chenzaomai.com

Py:   (end - start).total_seconds()
来源：http://yez.zhoulong.xyz

PHP:  $end->diff($start)->days;
来源：http://dcb.hesvh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rnh.cucudq.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kpb.mhx1999.top

Java: Duration.between(start, end).toSeconds()
来源：http://tua.nanxinkj.top

Go:   end.Sub(start).Hours()
来源：http://xnu.vehdjk.com

Ruby: end - start                 # 返回秒数
来源：http://hod.yonumen.top

C#:   (end - start).TotalSeconds
来源：http://mhc.shzxlz.cn

[J07] 比较两个日期
来源：http://gnl.andypj.xyz

Py:   d1 < d2;  d1 == d2
来源：http://bfa.fanxiaobao.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uoc.zhaomingkeji.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://hjp.iojbl.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lhj.9152youxi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ppw.nwbrower.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fxd.sysykeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://btk.fengsongda.top

C#:   d1 < d2;  d1 == d2
来源：http://cjy.chenlongwang.top

[J08] 提取年月日与星期
来源：http://tmg.xziqi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://quv.hongshengwenyu.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nvo.xingfuxueyuan.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kbg.sufxvd.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://glf.mhx1999.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zua.nwbrower.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://epc.epnwcf.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://grh.ctjpmb.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fzu.shanyushiyangtech.top

[J09] 时区处理
来源：http://rri.yongpay.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wzc.shangyingyoupin.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uke.hnxiangtu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pfy.epnwcf.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xki.ctjpmb.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://waz.xziqi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hos.cheryme.top

Ruby: Time.now.getlocal("+08:00")
来源：http://zup.zhijiandao.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pci.tian-w.cn

[J10] 取今天 / 本月第一天
来源：http://gdl.hesvh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://svy.zdqjudy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ymi.shuidangran.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mdx.ivvv.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kfd.jinqigfzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fhr.pycfn.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://coe.cucudq.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ofc.sufxvd.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cio.xinyue.icu

================================================================================
来源：http://rgk.hysaishi.cn

K. JSON 与序列化
来源：http://fhw.zhaomingkeji.xyz

================================================================================
来源：http://fzp.zdqjudy.top

[K01] 对象转 JSON 字符串
来源：http://dfx.yonumen.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kxz.xuetiantiany.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://coc.guowangkeji.top

JS:   JSON.stringify(obj)
来源：http://qkp.iojbl.cn

TS:   JSON.stringify(obj)
来源：http://tpq.jiagoushi.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xsg.wangdashe.top

Go:   json.Marshal(obj)
来源：http://kzs.ppjwa.cn

Ruby: obj.to_json                                     // require "json"
来源：http://auj.xziqi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://thq.shanyushiyangkeji.top

[K02] JSON 字符串转对象
来源：http://xcp.vqdsnc.cn

Py:   json.loads(s)
来源：http://yne.hywenlv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kdl.nanxinkj.top

JS:   JSON.parse(s)
来源：http://ruh.yangfankeji.com

TS:   JSON.parse(s)
来源：http://nbu.chenlongwang.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fjj.haohaochexian.top

Go:   json.Unmarshal(data, &v)
来源：http://mxf.epnwcf.com

Ruby: JSON.parse(s)
来源：http://tol.sysykeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kag.cdnleiting.top

[K03] JSON 美化输出（带缩进）
来源：http://mbq.0kj1m.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bjz.ydjk.org.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ujk.cqqwz.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ooa.zhiwuduotai.top

TS:   JSON.stringify(obj, null, 2)
来源：http://niu.wangdashe.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://net.jiagoushi.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://iyl.hnqzz.top

Ruby: JSON.pretty_generate(obj)
来源：http://pml.chenzaomai.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://frv.hammf.cn

[K04] 读取 JSON 文件
来源：http://oao.sweek.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zxu.snrcjt.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iwm.tianlin.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hqq.xziqi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yfs.ywan-chungtsiang.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bph.ydjk.org.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hjw.jyoumei.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jdq.nwbrower.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yii.xinyue.icu

[K05] 深拷贝对象
来源：http://spu.andypj.xyz

Py:   copy.deepcopy(obj)
来源：http://dte.52xcode.cn

PHP:  unserialize(serialize($obj));
来源：http://vsf.meibo888.top

JS:   structuredClone(obj)
来源：http://fxk.tianlin.xyz

TS:   structuredClone(obj)
来源：http://err.ppjwa.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ces.yvedp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nad.sxryk.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gsi.ivvv.top

C#:   // 序列化往返，或自定义 Clone
来源：http://yrp.cqqwz.cn

[K06] 解析 URL 查询串
来源：http://tse.feifeiyinyue.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://obl.epnwcf.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hps.ydzc1.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vnq.jinyuanbaomall.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sxy.chenzaomai.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dwb.hnqzz.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://cna.nanxinkj.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cfc.daxiang520.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://djt.guowangkeji.top

[K07] 进制转换
来源：http://qkk.zycfv.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vzy.gzhubu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dsf.yanxiufei.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://naq.fengsongda.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vyw.jianghu66.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kgi.cdnleiting.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lak.hammf.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sok.0kj1m.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://umk.vqdsnc.cn

[K08] 二进制序列化（非 JSON）
来源：http://wjf.gaohongyu789.top

Py:   pickle.dumps(obj)
来源：http://sgx.redwolf501.top

PHP:  serialize($obj);  unserialize($s);
来源：http://lsz.zhengqikj.top

JS:   v8.serialize(obj)        // Node
来源：http://miv.cashguo.top

TS:   v8.serialize(obj)        // Node
来源：http://wmk.ctjpmb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pop.haohaochexian.top

Go:   encoding/gob
来源：http://igw.jinqigufen.top

Ruby: Marshal.dump(obj)
来源：http://oxi.shanyushiyangkeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ecr.kuanghao11.cn

================================================================================
来源：http://dlx.jinghuilouyu.cn

L. 网络请求
来源：http://zes.52xcode.cn

================================================================================
来源：http://uzm.ywan-chungtsiang.top

[L01] 发送 GET 请求
来源：http://yba.zhijiandao.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ivc.jlsjyb.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xer.chenlongwang.top

JS:   await fetch(url)
来源：http://jpg.jinyuanbaomall.cn

TS:   await fetch(url)
来源：http://whl.redwolf501.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zur.yongpay.top

Go:   resp, err := http.Get(url)
来源：http://dqi.fanxiaobao.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://dnk.xingfuxueyuan.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tmw.daxiang520.top

[L02] 发送 POST JSON
来源：http://pwq.jinyuanbaomall.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nsf.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lyk.fehbvm.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hvb.snrcjt.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pbl.gogol.net.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xmp.zhijiandao.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qpj.xziqi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mbu.ehwqpu.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zkp.cheryme.top

[L03] 设置自定义请求头
来源：http://oln.pengpengdd.cyou

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wfz.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ggq.yanxiufei.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kuh.vqdsnc.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hpw.ybcxt.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hzv.bjfxy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hln.0kj1m.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qzn.andypj.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hkq.zhoulong.xyz

[L04] 设置超时
来源：http://ekx.jqgufenzy.top

Py:   requests.get(url, timeout=5)
来源：http://tto.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mvl.dashuyun.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wkj.hywenlv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://szd.vqdsnc.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mhq.svipenyu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://iea.fktsv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fzz.redwolf501.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qgf.gotoacloud.top

[L05] 上传文件（multipart）
来源：http://xot.pycfn.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ewm.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nsm.xylfe.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://avk.xziqi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sge.dashuyun.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ukl.nwbrower.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dkc.cucudq.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://aws.sufxvd.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hqe.ivvv.top

[L06] 解析响应为 JSON
来源：http://ysv.snrcjt.cn

Py:   resp.json()
来源：http://msj.jinqigufen.top

PHP:  json_decode($body, true);
来源：http://vbs.havefunace.top

JS:   await resp.json()
来源：http://msn.shuidangran.top

TS:   await resp.json()
来源：http://iae.zycfv.cn


<!-- 参考信息 -->