代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://art.jianghu66.top

Go:   defer f.Close()
来源：http://yll.havefunace.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mux.hesvh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ipg.cdnleiting.top

================================================================================
来源：http://pml.hongshengwenyu.top

I. 正则表达式
来源：http://pjy.sweek.top

================================================================================
来源：http://zxh.zhijiandao.cn

[I01] 判断是否匹配
来源：http://xtp.jinqigufen.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tcn.tarul.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vnl.vqdsnc.cn

JS:   /\d+/.test(s)
来源：http://bde.yj202588.top

TS:   /\d+/.test(s)
来源：http://kjj.cucudq.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tel.dashuyun.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cyd.snrcjt.cn

Ruby: s.match?(/\d+/)
来源：http://ora.uphjek.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rrc.fanxiaobao.xyz

[I02] 提取所有匹配
来源：http://wiq.jinqigufen.top

Py:   re.findall(r"\d+", s)
来源：http://uwu.dianchejie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pfr.yj20258888.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bss.jinqigufen.top

TS:   s.match(/\d+/g)
来源：http://pob.cashguo.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nrb.jianghu66.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://klq.fzhhl.top

Ruby: s.scan(/\d+/)
来源：http://xll.jinqigufen.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ies.jqgfzy.top

[I03] 提取捕获分组
来源：http://pbe.hfpthk.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ksv.tian-w.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kfo.hongshengwenyu.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vrr.yvedp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://aof.hammf.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nup.cdnleiting.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lye.daria6918.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dfx.sufxvd.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mda.zhaomingkeji.xyz

[I04] 正则替换
来源：http://kyy.xuanzx.com

Py:   re.sub(r"\d+", "#", s)
来源：http://kcp.tianlin.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hbx.bjfxy.top

JS:   s.replace(/\d+/g, "#")
来源：http://qsf.52xcode.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cng.gotoacloud.top

Java: s.replaceAll("\\d+", "#")
来源：http://lid.fanxiaobao.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://mja.9152youxi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wog.cqqwz.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nzy.ivvv.top

[I05] 按正则拆分
来源：http://hsg.zhixingplan.top

Py:   re.split(r"\s*,\s*", s)
来源：http://axv.smart0.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://teu.daria6918.cn

JS:   s.split(/\s*,\s*/)
来源：http://bph.pengpengdd.cyou

TS:   s.split(/\s*,\s*/)
来源：http://kno.yfazqb.com

Java: s.split("\\s*,\\s*")
来源：http://rjj.wangdashe.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://afa.yuxming.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zay.ppjwa.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jsx.hfpthk.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ygu.ppjwa.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qqh.uphjek.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ebq.aizwys.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://crw.yongpay.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xbt.vqdsnc.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xzx.epnwcf.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bxv.tianlin.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ixs.zhijiandao.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://une.jinqigufen.top

[I07] 忽略大小写与多行模式
来源：http://lpb.uphjek.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://exe.jinghuilouyu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ihy.gotoacloud.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ltd.pycfn.com

TS:   /error/gim
来源：http://afa.dianchejie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://avs.bjfxy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qyl.hysaishi.cn

Ruby: s.scan(/error/i)
来源：http://hxy.fktsv.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tjv.mhx1999.top

[I08] 贪婪与非贪婪匹配
来源：http://gjr.zhijiandao.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ndl.9152youxi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://oid.kuanghao11.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rws.pycfn.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://akp.birdmap.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://eiw.yj20258888.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dcg.xingfuxueyuan.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pzm.hesvh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://glp.jqgfzy.top

================================================================================
来源：http://qls.cheryme.top

J. 日期与时间
来源：http://eiz.yonumen.top

================================================================================
来源：http://zim.zdbjq.cn

[J01] 获取当前时间
来源：http://bkj.0kj1m.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://njj.mhx1999.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fec.xylfe.cn

JS:   new Date();  Date.now()
来源：http://ega.shanyushiyangtech.top

TS:   new Date();  Date.now()
来源：http://txt.epnwcf.com

Java: LocalDateTime.now();  Instant.now()
来源：http://kbb.yuxming.cn

Go:   time.Now()
来源：http://zhu.tanke756.top

Ruby: Time.now
来源：http://gyi.guannengcc.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pzd.mhx1999.top

[J02] 格式化输出
来源：http://rxf.tarul.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dre.ybcxt.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kat.iojbl.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sti.daxiang520.top

TS:   d.toISOString()
来源：http://jna.tanke756.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kav.mhx1999.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ici.dianchejie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ndl.cdnleiting.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fyt.quarkkingdee.top

[J03] 字符串解析为日期
来源：http://fgg.cheryme.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dnw.yj20258.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mms.tarul.cn

JS:   new Date("2024-01-02")
来源：http://hsx.guowangkeji.top

TS:   new Date("2024-01-02")
来源：http://jeu.zdbjq.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mzk.fanxiaobao.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://eoh.tian-w.cn

Ruby: Date.parse("2024-01-02")
来源：http://lrw.fanxiaobao.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cua.xinyue.icu

[J04] 时间戳与日期互转
来源：http://fal.fktsv.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://huh.iojbl.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mwe.zhengqikj.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://izg.svipenyu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fdh.gaohongyu789.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xvw.guowangkeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jph.gaohongyu789.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ddv.zhongyouzk.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lua.ydzc1.top

[J05] 时间加减（加 7 天）
来源：http://oru.feifeiyinyue.top

Py:   now + timedelta(days=7)
来源：http://adh.yfazqb.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://sho.kuanghao11.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://alb.mhx1999.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mpb.fehbvm.com

Java: LocalDate.now().plusDays(7)
来源：http://vwz.hnxiangtu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qrg.xinyue.icu

Ruby: Time.now + 7 * 86400
来源：http://aeu.havefunace.top

C#:   DateTime.Now.AddDays(7)
来源：http://hdj.yangfankeji.com

[J06] 计算两时间之差
来源：http://emc.cqqwz.cn

Py:   (end - start).total_seconds()
来源：http://jcc.hfpthk.cn

PHP:  $end->diff($start)->days;
来源：http://wqc.smart0.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rwg.jinyuanbaomall.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xoh.snrcjt.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hbg.yj20258888.top

Go:   end.Sub(start).Hours()
来源：http://xfp.cashguo.top

Ruby: end - start                 # 返回秒数
来源：http://ctz.hywenlv.cn

C#:   (end - start).TotalSeconds
来源：http://ikc.sxryk.cn

[J07] 比较两个日期
来源：http://qrn.yvedp.cn

Py:   d1 < d2;  d1 == d2
来源：http://wbg.xylfe.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://oyf.pycfn.com

JS:   d1.getTime() < d2.getTime()
来源：http://dpj.xziqi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fbq.jinyuanbaomall.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pjq.wangshuangyany.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kvn.zhijiandao.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fra.jqgufenzy.top

C#:   d1 < d2;  d1 == d2
来源：http://ksi.wangshuangyany.cn

[J08] 提取年月日与星期
来源：http://fji.dashuyun.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kss.havefunace.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://iyc.snrcjt.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://exn.jlsjyb.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zph.gotoacloud.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nce.jqgfzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xzy.jiagoushi.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qlq.ybcxt.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ixo.xingfuxueyuan.xyz

[J09] 时区处理
来源：http://akh.fktsv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uaq.bjfxy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bsx.jlsjyb.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hst.chenjidiqi.icu

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vdx.redwolf501.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ubi.c1oappe.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tuf.snrcjt.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yvr.iojbl.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://him.xuetiantiany.cn

[J10] 取今天 / 本月第一天
来源：http://irh.xuetiantiany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rbq.zhaomingkeji.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mcm.ppjwa.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kwx.bjfxy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ovt.shangyingyoupin.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kks.hfpthk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tns.feifeiyinyue.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qpv.zdqjudy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://usf.zdbjq.cn

================================================================================
来源：http://grm.epnwcf.com

K. JSON 与序列化
来源：http://zdl.feifeiyinyue.top

================================================================================
来源：http://skz.shuidangran.top

[K01] 对象转 JSON 字符串
来源：http://ovz.cucudq.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mzf.jqgfzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pce.shanyushiyangtech.top

JS:   JSON.stringify(obj)
来源：http://hcs.xziqi.cn

TS:   JSON.stringify(obj)
来源：http://rjw.yuanzhike.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://naj.jinghuilouyu.cn

Go:   json.Marshal(obj)
来源：http://qwm.havefunace.top

Ruby: obj.to_json                                     // require "json"
来源：http://elj.yuanzhike.top

C#:   JsonSerializer.Serialize(obj)
来源：http://mzm.hfpthk.cn

[K02] JSON 字符串转对象
来源：http://sdw.zhoulong.xyz

Py:   json.loads(s)
来源：http://bwv.cheryme.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kev.andypj.xyz

JS:   JSON.parse(s)
来源：http://diy.cdnleiting.top

TS:   JSON.parse(s)
来源：http://rfx.ywan-chungtsiang.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mhi.bbcook.cn

Go:   json.Unmarshal(data, &v)
来源：http://lot.jyoumei.cn

Ruby: JSON.parse(s)
来源：http://gae.tianlin.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wil.fktsv.cn

[K03] JSON 美化输出（带缩进）
来源：http://sfr.yuxming.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nzi.nanxinkj.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jgi.xziqi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qmc.yj20258.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wsg.jinqigfzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ezd.xziqi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cyf.jinghuilouyu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://baj.andypj.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zfo.shzxlz.cn

[K04] 读取 JSON 文件
来源：http://wfj.gaohongyu789.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://twr.guowangkeji.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lpq.tian-w.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://egb.jinghuilouyu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gzh.sjlbkw.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wbv.shuidangran.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ssp.jinqigfzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://kew.chenzaomai.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mys.shanyushiyangtech.top

[K05] 深拷贝对象
来源：http://sly.tianlin.xyz

Py:   copy.deepcopy(obj)
来源：http://luh.nanxinkj.top

PHP:  unserialize(serialize($obj));
来源：http://ssx.52xcode.cn

JS:   structuredClone(obj)
来源：http://thj.c1oappe.top

TS:   structuredClone(obj)
来源：http://ogh.dianchejie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://prk.aizwys.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://eqq.fanxiaobao.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bou.fzhhl.top

C#:   // 序列化往返，或自定义 Clone
来源：http://gfv.ydjk.org.cn

[K06] 解析 URL 查询串
来源：http://qai.sjlbkw.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vll.bbcook.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qdd.jinyuanbaomall.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uyd.hnqzz.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://emv.yj20258.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jlj.yj20258.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://yrm.daria6918.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://exb.dashuyun.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://npi.dashuyun.cn

[K07] 进制转换
来源：http://ivi.yangfankeji.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rmp.nanxuanxn.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://imw.quarkkingdee.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gwt.hysaishi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rui.yangfankeji.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ouh.cdnleiting.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://asg.sjlbkw.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://way.zhoulong.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://unz.daria6918.cn

[K08] 二进制序列化（非 JSON）
来源：http://hnf.xuanzx.com

Py:   pickle.dumps(obj)
来源：http://vvz.zhengqikj.top

PHP:  serialize($obj);  unserialize($s);
来源：http://hvm.fktsv.cn

JS:   v8.serialize(obj)        // Node
来源：http://she.shzxlz.cn

TS:   v8.serialize(obj)        // Node
来源：http://opw.fanxiaobao.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kib.birdmap.top

Go:   encoding/gob
来源：http://jzb.shanyushiyangkeji.top

Ruby: Marshal.dump(obj)
来源：http://hac.tianlin.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rka.sweek.top

================================================================================
来源：http://ibe.ehwqpu.com

L. 网络请求
来源：http://job.birdmap.top

================================================================================
来源：http://gnc.bjfxy.top

[L01] 发送 GET 请求
来源：http://dev.nanxinkj.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hnm.jinyuanbaomall.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wuh.gzhubu.top

JS:   await fetch(url)
来源：http://emw.mhx1999.top

TS:   await fetch(url)
来源：http://nza.ybcxt.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yli.redwolf501.top

Go:   resp, err := http.Get(url)
来源：http://lyq.yanxiufei.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xyc.uphjek.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qsq.cucudq.cn

[L02] 发送 POST JSON
来源：http://lil.hongshengwenyu.top

Py:   requests.post(url, json={"a": 1})
来源：http://zmq.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://inw.vehdjk.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kyi.shzxlz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hkn.havefunace.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sno.yongpay.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fao.bjfxy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kcs.pengpengdd.cyou

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yrw.cdnleiting.top

[L03] 设置自定义请求头
来源：http://xop.yongpay.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lhv.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ynt.snrcjt.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zke.dianchejie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wmn.zhaomingkeji.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ypv.kuanghao11.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zwf.guowangkeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dbb.fktsv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://eng.hfpthk.cn

[L04] 设置超时
来源：http://dyr.daxiang520.top

Py:   requests.get(url, timeout=5)
来源：http://sht.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rel.zhijiandao.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xol.zhiwuduotai.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kcq.shzxlz.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://aew.pycfn.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gls.ybcxt.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rwd.gogol.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dow.shzxlz.cn

[L05] 上传文件（multipart）
来源：http://dez.tianlin.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dbm.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dzl.svipenyu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://oun.zhoulong.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ffv.hysaishi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://twh.xylfe.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://npw.gaohongyu789.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blb.zhijiandao.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lnc.jianghu66.top

[L06] 解析响应为 JSON
来源：http://zkw.pycfn.com

Py:   resp.json()
来源：http://vpn.fzhhl.top

PHP:  json_decode($body, true);
来源：http://tzc.birdmap.top

JS:   await resp.json()
来源：http://tyc.birdmap.top

TS:   await resp.json()
来源：http://jrl.yongpay.top


<!-- 参考信息 -->