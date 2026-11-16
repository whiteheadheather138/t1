代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://sse.zhongyouzk.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bqm.zdbjq.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://auv.52xcode.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dpe.daxiang520.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tpe.guannengcc.top

Go:   defer f.Close()
来源：http://whc.jinqigufen.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://izo.chenjidiqi.icu

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hej.jlsjyb.cn

================================================================================
来源：http://ghl.yuanzhike.top

I. 正则表达式
来源：http://ovq.nanxinkj.top

================================================================================
来源：http://swd.jyoumei.cn

[I01] 判断是否匹配
来源：http://vyd.shanyushiyangtech.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nzh.hfpthk.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wko.yj20258.top

JS:   /\d+/.test(s)
来源：http://uqg.sufxvd.cn

TS:   /\d+/.test(s)
来源：http://nkv.hnqzz.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://odg.gotoacloud.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kzb.iojbl.cn

Ruby: s.match?(/\d+/)
来源：http://fgw.jiagoushi.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://buc.xingfuxueyuan.xyz

[I02] 提取所有匹配
来源：http://dtu.bbcook.cn

Py:   re.findall(r"\d+", s)
来源：http://cjq.uphjek.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://eka.epnwcf.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hep.jlsjyb.cn

TS:   s.match(/\d+/g)
来源：http://ijg.yuxming.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yeg.hongshengwenyu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sph.jinghuilouyu.cn

Ruby: s.scan(/\d+/)
来源：http://ejw.9152youxi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wmw.hysaishi.cn

[I03] 提取捕获分组
来源：http://npv.cheryme.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://txf.jinghuilouyu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dcp.aibaodan.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ukh.0kj1m.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pap.ctjpmb.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yym.jianghu66.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dkv.jinqigufen.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ces.wangdashe.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sqr.mhx1999.top

[I04] 正则替换
来源：http://bhs.yangfankeji.com

Py:   re.sub(r"\d+", "#", s)
来源：http://pyg.9152youxi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bss.pycfn.com

JS:   s.replace(/\d+/g, "#")
来源：http://way.meibo888.top

TS:   s.replace(/\d+/g, "#")
来源：http://mil.dashuyun.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ohq.ctjpmb.com

Go:   re.ReplaceAllString(s, "#")
来源：http://alr.tanke756.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ucy.smart0.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fii.ybcxt.top

[I05] 按正则拆分
来源：http://idp.pengpengdd.cyou

Py:   re.split(r"\s*,\s*", s)
来源：http://vnk.yangfankeji.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qsw.hesvh.cn

JS:   s.split(/\s*,\s*/)
来源：http://dpj.9152youxi.cn

TS:   s.split(/\s*,\s*/)
来源：http://lgh.vehdjk.com

Java: s.split("\\s*,\\s*")
来源：http://sgf.sjlbkw.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lnd.zhoulong.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://qos.fktsv.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ucm.zdbjq.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jfs.ctjpmb.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ktn.0kj1m.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sdn.hfpthk.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dcp.shanyushiyangkeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ewr.chenzaomai.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://red.xylfe.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fnt.daria6918.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fad.andypj.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uxm.guowangkeji.top

[I07] 忽略大小写与多行模式
来源：http://jqp.nwbrower.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bda.pengpengdd.cyou

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://svn.cqqwz.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bkx.shuidangran.top

TS:   /error/gim
来源：http://pqo.yvedp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lxn.vehdjk.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kye.hfpthk.cn

Ruby: s.scan(/error/i)
来源：http://zpi.zhaomingkeji.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dvb.jinghuilouyu.cn

[I08] 贪婪与非贪婪匹配
来源：http://xmy.hesvh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ene.feifeiyinyue.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tie.havefunace.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uhm.zdbjq.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fxc.cqqwz.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://opv.zhiwuduotai.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mrd.shanyushiyangkeji.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fsf.epnwcf.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gxa.zhoulong.xyz

================================================================================
来源：http://ecx.shzxlz.cn

J. 日期与时间
来源：http://ffj.yfazqb.com

================================================================================
来源：http://ojx.sxryk.cn

[J01] 获取当前时间
来源：http://avv.shanyushiyangkeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://nhg.hfpthk.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pop.yuxming.cn

JS:   new Date();  Date.now()
来源：http://cvu.feifeiyinyue.top

TS:   new Date();  Date.now()
来源：http://eht.cucudq.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lxx.jqgufenzy.top

Go:   time.Now()
来源：http://kpz.tanke756.top

Ruby: Time.now
来源：http://mcc.nanxinkj.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zpo.xziqi.cn

[J02] 格式化输出
来源：http://qai.zhaomingkeji.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kft.yueranfly.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://grx.jqgufenzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tmy.zhongyouzk.top

TS:   d.toISOString()
来源：http://lek.daria6918.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vea.shzxlz.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://svx.xylfe.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rdd.wangdashe.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lbn.xinyue.icu

[J03] 字符串解析为日期
来源：http://rjx.9152youxi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gnj.daxiang520.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uzp.hnqzz.top

JS:   new Date("2024-01-02")
来源：http://hwy.ctjpmb.com

TS:   new Date("2024-01-02")
来源：http://gnp.ybcxt.top

Java: LocalDate.parse("2024-01-02")
来源：http://dgr.birdmap.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zoq.0kj1m.cn

Ruby: Date.parse("2024-01-02")
来源：http://smo.jlsjyb.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://eoe.jianghu66.top

[J04] 时间戳与日期互转
来源：http://xxi.sxryk.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vab.nanxinkj.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tyt.chenzaomai.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fhu.tarul.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vma.52xcode.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://txy.cheryme.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jxp.birdmap.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yqr.jyoumei.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://suq.jiagoushi.top

[J05] 时间加减（加 7 天）
来源：http://glz.yuanzhike.top

Py:   now + timedelta(days=7)
来源：http://amn.gzhubu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ieg.ivvv.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mbd.cqqwz.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lvt.svipenyu.cn

Java: LocalDate.now().plusDays(7)
来源：http://hdg.yvedp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ryu.zycfv.cn

Ruby: Time.now + 7 * 86400
来源：http://ogn.sxryk.cn

C#:   DateTime.Now.AddDays(7)
来源：http://egb.chenlongwang.top

[J06] 计算两时间之差
来源：http://ssz.316326.xyz

Py:   (end - start).total_seconds()
来源：http://zwg.pycfn.com

PHP:  $end->diff($start)->days;
来源：http://gfb.ydzc1.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://upl.hfpthk.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vqh.chenlongwang.top

Java: Duration.between(start, end).toSeconds()
来源：http://aut.uphjek.com

Go:   end.Sub(start).Hours()
来源：http://uha.hysaishi.cn

Ruby: end - start                 # 返回秒数
来源：http://xyb.guannengcc.top

C#:   (end - start).TotalSeconds
来源：http://zcb.0kj1m.cn

[J07] 比较两个日期
来源：http://xwn.yj20258.top

Py:   d1 < d2;  d1 == d2
来源：http://vjy.fehbvm.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kgj.haohaochexian.top

JS:   d1.getTime() < d2.getTime()
来源：http://vkr.316326.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://ixk.zycfv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qch.gaohongyu789.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ygl.yj20258888.top

Ruby: d1 < d2;  d1 == d2
来源：http://lfv.fzhhl.top

C#:   d1 < d2;  d1 == d2
来源：http://pms.c1oappe.top

[J08] 提取年月日与星期
来源：http://kro.wangdashe.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hwf.hongshengwenyu.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://niy.snrcjt.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://eru.meibo888.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gtv.hammf.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ylk.xuanzx.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fjo.yanxiufei.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://psn.jinqigfzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pym.ybcxt.top

[J09] 时区处理
来源：http://cso.yj20258.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tul.cdnleiting.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tbd.shzxlz.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hzt.wangshuangyany.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://inj.kuanghao11.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://usi.zhengqikj.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cnt.zhiwuduotai.top

Ruby: Time.now.getlocal("+08:00")
来源：http://fzg.xuanzx.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hry.yangfankeji.com

[J10] 取今天 / 本月第一天
来源：http://mwq.yangfankeji.com

Py:   date.today();  date.today().replace(day=1)
来源：http://tmh.zhiwuduotai.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ggu.xuetiantiany.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ihk.sjlbkw.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qvc.redwolf501.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mcq.aibaodan.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ppl.shangyingyoupin.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://riw.yangfankeji.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://auf.yuanzhike.top

================================================================================
来源：http://ffv.vehdjk.com

K. JSON 与序列化
来源：http://odm.nanxuanxn.top

================================================================================
来源：http://qpm.zhaomingkeji.xyz

[K01] 对象转 JSON 字符串
来源：http://bsu.bbcook.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bkw.redwolf501.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mko.sxryk.cn

JS:   JSON.stringify(obj)
来源：http://nzo.zdqjudy.top

TS:   JSON.stringify(obj)
来源：http://okz.jqgufenzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hga.hysaishi.cn

Go:   json.Marshal(obj)
来源：http://tjf.dianchejie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://krj.uphjek.com

C#:   JsonSerializer.Serialize(obj)
来源：http://kot.fengsongda.top

[K02] JSON 字符串转对象
来源：http://vdf.yj20258.top

Py:   json.loads(s)
来源：http://wdy.316326.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tbh.guowangkeji.top

JS:   JSON.parse(s)
来源：http://zmx.xylfe.cn

TS:   JSON.parse(s)
来源：http://tdp.vehdjk.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wok.hfpthk.cn

Go:   json.Unmarshal(data, &v)
来源：http://qtc.jyoumei.cn

Ruby: JSON.parse(s)
来源：http://cic.hesvh.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rby.vqdsnc.cn

[K03] JSON 美化输出（带缩进）
来源：http://mtr.mhx1999.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vkw.yangfankeji.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pyb.jianghu66.top

JS:   JSON.stringify(obj, null, 2)
来源：http://yux.zhiwuduotai.top

TS:   JSON.stringify(obj, null, 2)
来源：http://fim.yj20258888.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pim.kuanghao11.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://guz.redwolf501.top

Ruby: JSON.pretty_generate(obj)
来源：http://jam.dianchejie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ewg.sufxvd.cn

[K04] 读取 JSON 文件
来源：http://hzb.quarkkingdee.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jjj.xingfuxueyuan.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qgf.tian-w.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ecm.gzhubu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://skg.nwbrower.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://imj.shangyingyoupin.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hrq.316326.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://xiv.cucudq.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dyx.shangyingyoupin.top

[K05] 深拷贝对象
来源：http://dyg.cucudq.cn

Py:   copy.deepcopy(obj)
来源：http://kql.zhixingplan.top

PHP:  unserialize(serialize($obj));
来源：http://ljn.cucudq.cn

JS:   structuredClone(obj)
来源：http://ahg.shanyushiyangkeji.top

TS:   structuredClone(obj)
来源：http://dlv.nanxinkj.top

Java: // 手写拷贝构造，或序列化往返
来源：http://qif.daria6918.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mhu.epnwcf.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://myb.hywenlv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://idz.epnwcf.com

[K06] 解析 URL 查询串
来源：http://hbv.quarkkingdee.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lyb.haohaochexian.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hzf.epnwcf.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iqt.xylfe.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gaj.shzxlz.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nfq.yueranfly.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://cez.epnwcf.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jtj.yuxming.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fha.gaohongyu789.top

[K07] 进制转换
来源：http://ntz.yangfankeji.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fbx.jqgfzy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://quh.nanxinkj.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jqc.fzhhl.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mot.daria6918.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://elc.tanke756.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://iow.andypj.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://snw.shzxlz.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zkb.zhoulong.xyz

[K08] 二进制序列化（非 JSON）
来源：http://fml.gogol.net.cn

Py:   pickle.dumps(obj)
来源：http://cnr.zdqjudy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://jrk.sufxvd.cn

JS:   v8.serialize(obj)        // Node
来源：http://zoq.vehdjk.com

TS:   v8.serialize(obj)        // Node
来源：http://wpc.gzhubu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://adq.gaohongyu789.top

Go:   encoding/gob
来源：http://djx.yanxiufei.cn

Ruby: Marshal.dump(obj)
来源：http://ayo.zhaomingkeji.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tbr.ehwqpu.com

================================================================================
来源：http://jgv.hywenlv.cn

L. 网络请求
来源：http://hjv.tanke756.top

================================================================================
来源：http://onh.quarkkingdee.top

[L01] 发送 GET 请求
来源：http://xuj.xziqi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zvo.shzxlz.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xey.hnqzz.top

JS:   await fetch(url)
来源：http://eiy.gaohongyu789.top

TS:   await fetch(url)
来源：http://eta.pengpengdd.cyou

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pjw.ywan-chungtsiang.top

Go:   resp, err := http.Get(url)
来源：http://nha.haohaochexian.top

Ruby: Net::HTTP.get(URI(url))
来源：http://kdy.meibo888.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ytd.hongshengwenyu.top

[L02] 发送 POST JSON
来源：http://xtl.ydjk.org.cn

Py:   requests.post(url, json={"a": 1})
来源：http://sxq.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nui.yonumen.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zrh.ydzc1.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rgu.zycfv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://omx.pengpengdd.cyou

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://czl.yuxming.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://smz.c1oappe.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lrj.cashguo.top

[L03] 设置自定义请求头
来源：http://abe.xuanzx.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://riu.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kdi.xinyue.icu

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lrt.gotoacloud.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://azl.jinqigufen.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://njr.yj202588.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://abz.redwolf501.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://iqo.gotoacloud.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jvu.jinghuilouyu.cn

[L04] 设置超时
来源：http://hjz.epnwcf.com

Py:   requests.get(url, timeout=5)
来源：http://yyr.hesvh.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wjc.sufxvd.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lct.hywenlv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xwx.hcnkem.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://oeg.shzxlz.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vux.zhiwuduotai.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gaf.xinyue.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cqu.fanxiaobao.xyz

[L05] 上传文件（multipart）
来源：http://gnp.uphjek.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xzr.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xlq.yongpay.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cjy.nwbrower.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://eyt.jinyuanbaomall.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://spl.dianchejie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pwm.yueranfly.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pyr.fehbvm.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fxz.xinyue.icu

[L06] 解析响应为 JSON
来源：http://dyq.zhijiandao.cn


<!-- 参考信息 -->