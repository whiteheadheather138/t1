代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qod.birdmap.top

Go:   defer f.Close()
来源：http://vja.daxiang520.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bbl.aizwys.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dhp.zhengqikj.top

================================================================================
来源：http://rre.9152youxi.cn

I. 正则表达式
来源：http://ttn.ywan-chungtsiang.top

================================================================================
来源：http://pwu.xinyue.icu

[I01] 判断是否匹配
来源：http://lwb.hcnkem.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cyv.bjfxy.top

PHP:  preg_match('/\d+/', $s);
来源：http://pxm.fktsv.cn

JS:   /\d+/.test(s)
来源：http://nzz.ppjwa.cn

TS:   /\d+/.test(s)
来源：http://ftd.xingfuxueyuan.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://htr.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mxx.ydzc1.top

Ruby: s.match?(/\d+/)
来源：http://wkq.birdmap.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yvj.cheryme.top

[I02] 提取所有匹配
来源：http://bst.daria6918.cn

Py:   re.findall(r"\d+", s)
来源：http://dwj.hnxiangtu.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wht.jinqigfzy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://typ.zhoulong.xyz

TS:   s.match(/\d+/g)
来源：http://xjb.bbcook.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fpf.snrcjt.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gxt.haohaochexian.top

Ruby: s.scan(/\d+/)
来源：http://tvq.ctjpmb.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://flg.epnwcf.com

[I03] 提取捕获分组
来源：http://gjs.sjlbkw.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://eoz.sufxvd.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dvq.xingfuxueyuan.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pmn.nanxinkj.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ljt.cucudq.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://muo.wangshuangyany.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ifq.haohaochexian.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yzt.yueranfly.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ztx.jqgfzy.top

[I04] 正则替换
来源：http://acj.shanyushiyangtech.top

Py:   re.sub(r"\d+", "#", s)
来源：http://twz.ivvv.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ppc.quarkkingdee.top

JS:   s.replace(/\d+/g, "#")
来源：http://ffp.ybcxt.top

TS:   s.replace(/\d+/g, "#")
来源：http://dhb.daria6918.cn

Java: s.replaceAll("\\d+", "#")
来源：http://eix.ppjwa.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lqm.zhoulong.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://yrg.0kj1m.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qyl.pengpengdd.cyou

[I05] 按正则拆分
来源：http://wrh.fanxiaobao.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://avy.yvedp.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zpx.xylfe.cn

JS:   s.split(/\s*,\s*/)
来源：http://obz.ivvv.top

TS:   s.split(/\s*,\s*/)
来源：http://obk.xziqi.cn

Java: s.split("\\s*,\\s*")
来源：http://obk.jinghuilouyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://itm.vehdjk.com

Ruby: s.split(/\s*,\s*/)
来源：http://dmf.yj20258888.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ctf.yongpay.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xym.haohaochexian.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tzz.gaohongyu789.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zqs.guowangkeji.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oru.zhengqikj.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nnn.yuanzhike.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://meg.shzxlz.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xef.52xcode.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://unx.shanyushiyangtech.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vmv.pengpengdd.cyou

[I07] 忽略大小写与多行模式
来源：http://raf.zdqjudy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hiq.jianghu66.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://iqk.jqgufenzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cfd.yanxiufei.cn

TS:   /error/gim
来源：http://jqs.yj202588.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://izc.xylfe.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kfg.ydzc1.top

Ruby: s.scan(/error/i)
来源：http://vak.ydzc1.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lux.yueranfly.top

[I08] 贪婪与非贪婪匹配
来源：http://dkh.gotoacloud.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tdm.hysaishi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ewj.fanxiaobao.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://trh.guannengcc.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bwd.uphjek.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://nei.ydzc1.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sxv.dianchejie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pnz.kuanghao11.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://olv.pengpengdd.cyou

================================================================================
来源：http://cdj.bjfxy.top

J. 日期与时间
来源：http://htj.redwolf501.top

================================================================================
来源：http://ixx.ppjwa.cn

[J01] 获取当前时间
来源：http://nan.c1oappe.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://rbm.snrcjt.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mev.yuanzhike.top

JS:   new Date();  Date.now()
来源：http://ltu.pycfn.com

TS:   new Date();  Date.now()
来源：http://fbx.daxiang520.top

Java: LocalDateTime.now();  Instant.now()
来源：http://uor.hfpthk.cn

Go:   time.Now()
来源：http://okl.xuetiantiany.cn

Ruby: Time.now
来源：http://gyi.jinqigfzy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zgk.shangyingyoupin.top

[J02] 格式化输出
来源：http://jdp.zhongyouzk.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rbr.hnqzz.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zaw.yangfankeji.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vli.tanke756.top

TS:   d.toISOString()
来源：http://ncu.hnqzz.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fjm.svipenyu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kxv.jqgfzy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://asa.shzxlz.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uqi.zdqjudy.top

[J03] 字符串解析为日期
来源：http://iwi.guowangkeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://doa.quarkkingdee.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gof.jqgufenzy.top

JS:   new Date("2024-01-02")
来源：http://okv.hysaishi.cn

TS:   new Date("2024-01-02")
来源：http://lab.ppjwa.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xly.zhoulong.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hms.yueranfly.top

Ruby: Date.parse("2024-01-02")
来源：http://mna.sufxvd.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uuf.9152youxi.cn

[J04] 时间戳与日期互转
来源：http://lsz.cqqwz.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hfm.aibaodan.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rqb.hesvh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nyh.jlsjyb.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ewi.fanxiaobao.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tjh.jianghu66.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qxh.daxiang520.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uye.hcnkem.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ber.wangshuangyany.cn

[J05] 时间加减（加 7 天）
来源：http://vlh.ywan-chungtsiang.top

Py:   now + timedelta(days=7)
来源：http://nzr.jianghu66.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://kox.hammf.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://spx.chenzaomai.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cpz.hnqzz.top

Java: LocalDate.now().plusDays(7)
来源：http://jwz.smart0.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yze.hfpthk.cn

Ruby: Time.now + 7 * 86400
来源：http://cua.haohaochexian.top

C#:   DateTime.Now.AddDays(7)
来源：http://agw.fanxiaobao.xyz

[J06] 计算两时间之差
来源：http://gva.c1oappe.top

Py:   (end - start).total_seconds()
来源：http://ofw.ivvv.top

PHP:  $end->diff($start)->days;
来源：http://utn.zhengqikj.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jyd.tianlin.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pcr.fktsv.cn

Java: Duration.between(start, end).toSeconds()
来源：http://njq.dashuyun.cn

Go:   end.Sub(start).Hours()
来源：http://slv.xingfuxueyuan.xyz

Ruby: end - start                 # 返回秒数
来源：http://pec.52xcode.cn

C#:   (end - start).TotalSeconds
来源：http://qjs.birdmap.top

[J07] 比较两个日期
来源：http://iyk.hesvh.cn

Py:   d1 < d2;  d1 == d2
来源：http://hlv.aibaodan.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gkf.xuetiantiany.cn

JS:   d1.getTime() < d2.getTime()
来源：http://aqj.yueranfly.top

TS:   d1.getTime() < d2.getTime()
来源：http://rfx.shanyushiyangkeji.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ond.jqgfzy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ntl.shuidangran.top

Ruby: d1 < d2;  d1 == d2
来源：http://wtn.quarkkingdee.top

C#:   d1 < d2;  d1 == d2
来源：http://imm.guowangkeji.top

[J08] 提取年月日与星期
来源：http://zua.cheryme.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lqg.yangfankeji.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://aby.hnxiangtu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bbw.jinghuilouyu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bfk.shzxlz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://eec.jiagoushi.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://iiu.epnwcf.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hvu.pycfn.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ygc.jiagoushi.top

[J09] 时区处理
来源：http://kbi.shangyingyoupin.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://twr.tianlin.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://moz.fengsongda.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tqm.quarkkingdee.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mis.vehdjk.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qip.fzhhl.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cbo.nanxinkj.top

Ruby: Time.now.getlocal("+08:00")
来源：http://fzn.xziqi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gml.cdnleiting.top

[J10] 取今天 / 本月第一天
来源：http://spl.vqdsnc.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tby.jinghuilouyu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://epb.vqdsnc.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yaj.nwbrower.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ndt.yueranfly.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mxw.jyoumei.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://iua.sufxvd.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uxc.hongshengwenyu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vdg.hammf.cn

================================================================================
来源：http://qde.shzxlz.cn

K. JSON 与序列化
来源：http://vcn.sweek.top

================================================================================
来源：http://xgf.gaohongyu789.top

[K01] 对象转 JSON 字符串
来源：http://pqy.ydzc1.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xsz.316326.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mid.dashuyun.cn

JS:   JSON.stringify(obj)
来源：http://wyb.dianchejie.cn

TS:   JSON.stringify(obj)
来源：http://kwi.svipenyu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ejw.jlsjyb.cn

Go:   json.Marshal(obj)
来源：http://fwv.uphjek.com

Ruby: obj.to_json                                     // require "json"
来源：http://kjc.smart0.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://yrq.9152youxi.cn

[K02] JSON 字符串转对象
来源：http://amc.hnqzz.top

Py:   json.loads(s)
来源：http://jzw.meibo888.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ayc.jinghuilouyu.cn

JS:   JSON.parse(s)
来源：http://zka.cheryme.top

TS:   JSON.parse(s)
来源：http://khf.fehbvm.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fwa.shanyushiyangkeji.top

Go:   json.Unmarshal(data, &v)
来源：http://yat.xinyue.icu

Ruby: JSON.parse(s)
来源：http://odq.yongpay.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uss.sweek.top

[K03] JSON 美化输出（带缩进）
来源：http://fcl.haohaochexian.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://beb.cdnleiting.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vgv.yuxming.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://oqk.sufxvd.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tig.xuetiantiany.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lhp.cqqwz.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uko.ehwqpu.com

Ruby: JSON.pretty_generate(obj)
来源：http://qwo.sxryk.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zou.cqqwz.cn

[K04] 读取 JSON 文件
来源：http://fta.meibo888.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tvg.kuanghao11.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://puy.gotoacloud.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gjp.aizwys.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oka.smart0.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ics.yj20258.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dul.cqqwz.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hsc.nanxuanxn.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jxf.jinqigfzy.top

[K05] 深拷贝对象
来源：http://dvp.kuanghao11.cn

Py:   copy.deepcopy(obj)
来源：http://xon.52xcode.cn

PHP:  unserialize(serialize($obj));
来源：http://hep.ehwqpu.com

JS:   structuredClone(obj)
来源：http://mrg.tianlin.xyz

TS:   structuredClone(obj)
来源：http://jzp.zdbjq.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ykn.aibaodan.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tmg.zdbjq.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://viq.ivvv.top

C#:   // 序列化往返，或自定义 Clone
来源：http://gbv.kuanghao11.cn

[K06] 解析 URL 查询串
来源：http://pot.vqdsnc.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rnk.zhoulong.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tbs.tian-w.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ejs.jqgufenzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://foj.aizwys.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mme.aibaodan.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://lxc.jinyuanbaomall.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wvu.yvedp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nwt.tianlin.xyz

[K07] 进制转换
来源：http://rtb.vqdsnc.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://swx.wangshuangyany.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lsa.vehdjk.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kii.fzhhl.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vey.jinqigfzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ely.xuetiantiany.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zcb.hywenlv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fxv.gogol.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yoq.yj202588.top

[K08] 二进制序列化（非 JSON）
来源：http://lni.yvedp.cn

Py:   pickle.dumps(obj)
来源：http://zfg.jinyuanbaomall.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bgi.sufxvd.cn

JS:   v8.serialize(obj)        // Node
来源：http://jvr.fehbvm.com

TS:   v8.serialize(obj)        // Node
来源：http://bce.smart0.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qdb.yvedp.cn

Go:   encoding/gob
来源：http://jmp.fanxiaobao.xyz

Ruby: Marshal.dump(obj)
来源：http://sqf.ehwqpu.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qxk.ctjpmb.com

================================================================================
来源：http://rar.c1oappe.top

L. 网络请求
来源：http://hgw.ivvv.top

================================================================================
来源：http://why.hnqzz.top

[L01] 发送 GET 请求
来源：http://mwz.guowangkeji.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cdz.shangyingyoupin.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://muh.shuidangran.top

JS:   await fetch(url)
来源：http://chd.ivvv.top

TS:   await fetch(url)
来源：http://bcx.zhijiandao.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hmm.shanyushiyangtech.top

Go:   resp, err := http.Get(url)
来源：http://yim.wangshuangyany.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hzu.ivvv.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ytz.ctjpmb.com

[L02] 发送 POST JSON
来源：http://itw.xinyue.icu

Py:   requests.post(url, json={"a": 1})
来源：http://rlx.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://leo.feifeiyinyue.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wgg.yongpay.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vui.xziqi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fug.shangyingyoupin.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kpc.nanxuanxn.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://loj.dashuyun.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://scf.jqgfzy.top

[L03] 设置自定义请求头
来源：http://ard.yvedp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hhr.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rew.uphjek.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jvy.shangyingyoupin.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ult.jinghuilouyu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vol.fehbvm.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://urm.chenlongwang.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xjb.zycfv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ebd.sjlbkw.cn

[L04] 设置超时
来源：http://yfp.cheryme.top

Py:   requests.get(url, timeout=5)
来源：http://ipg.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tht.jinghuilouyu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cgv.pengpengdd.cyou

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://egm.jqgufenzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bzh.ppjwa.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zno.aizwys.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ldr.hammf.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://eeu.jinghuilouyu.cn

[L05] 上传文件（multipart）
来源：http://jdt.andypj.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://czy.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mhk.aizwys.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vse.snrcjt.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dqp.yvedp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hkw.hongshengwenyu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qcw.pengpengdd.cyou

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dgg.nanxuanxn.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ewd.52xcode.cn

[L06] 解析响应为 JSON
来源：http://arh.jianghu66.top

Py:   resp.json()
来源：http://acn.hysaishi.cn

PHP:  json_decode($body, true);
来源：http://jlc.birdmap.top

JS:   await resp.json()
来源：http://kcd.zhoulong.xyz

TS:   await resp.json()
来源：http://ciq.xylfe.cn


<!-- 参考信息 -->