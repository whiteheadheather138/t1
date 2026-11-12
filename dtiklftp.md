代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dlk.c1oappe.top

Go:   defer f.Close()
来源：http://tvk.gotoacloud.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mnn.guannengcc.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ylv.jqgfzy.top

================================================================================
来源：http://aig.yj202588.top

I. 正则表达式
来源：http://uir.svipenyu.cn

================================================================================
来源：http://dkc.shanyushiyangkeji.top

[I01] 判断是否匹配
来源：http://dzz.wangdashe.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ebu.gaohongyu789.top

PHP:  preg_match('/\d+/', $s);
来源：http://dig.hongshengwenyu.top

JS:   /\d+/.test(s)
来源：http://wmp.jqgufenzy.top

TS:   /\d+/.test(s)
来源：http://zkx.hcnkem.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tvi.havefunace.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jse.zdqjudy.top

Ruby: s.match?(/\d+/)
来源：http://zts.guannengcc.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dau.birdmap.top

[I02] 提取所有匹配
来源：http://wcb.xuanzx.com

Py:   re.findall(r"\d+", s)
来源：http://grv.smart0.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vff.sysykeji.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xgo.hnxiangtu.top

TS:   s.match(/\d+/g)
来源：http://jwz.jianghu66.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ijt.sjlbkw.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yzn.aibaodan.cn

Ruby: s.scan(/\d+/)
来源：http://goo.pengpengdd.cyou

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://klj.fzhhl.top

[I03] 提取捕获分组
来源：http://dgz.quarkkingdee.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gas.uphjek.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pvx.ppjwa.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dmi.jianghu66.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qop.0kj1m.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gxn.feifeiyinyue.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rob.zhongyouzk.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kja.fengsongda.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wyo.cashguo.top

[I04] 正则替换
来源：http://xtz.shanyushiyangtech.top

Py:   re.sub(r"\d+", "#", s)
来源：http://kaj.9152youxi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://evs.ydzc1.top

JS:   s.replace(/\d+/g, "#")
来源：http://mgu.quarkkingdee.top

TS:   s.replace(/\d+/g, "#")
来源：http://hgt.hnqzz.top

Java: s.replaceAll("\\d+", "#")
来源：http://shs.meibo888.top

Go:   re.ReplaceAllString(s, "#")
来源：http://kwc.xziqi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cpi.yanxiufei.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vod.sweek.top

[I05] 按正则拆分
来源：http://dzt.aibaodan.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://pao.jianghu66.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tzr.sysykeji.top

JS:   s.split(/\s*,\s*/)
来源：http://lev.jqgufenzy.top

TS:   s.split(/\s*,\s*/)
来源：http://guw.daxiang520.top

Java: s.split("\\s*,\\s*")
来源：http://ptu.svipenyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://naq.xingfuxueyuan.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://eie.ehwqpu.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kmq.yangfankeji.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xfj.chenjidiqi.icu

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tlr.fengsongda.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://prr.c1oappe.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ewl.yj20258.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rlx.hywenlv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dyo.0kj1m.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lmt.jinqigfzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://czh.cucudq.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rql.jlsjyb.cn

[I07] 忽略大小写与多行模式
来源：http://bhi.feifeiyinyue.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kcz.sxryk.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jct.ybcxt.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mbg.fktsv.cn

TS:   /error/gim
来源：http://ipz.xuetiantiany.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cjl.dianchejie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lln.nanxuanxn.top

Ruby: s.scan(/error/i)
来源：http://dpa.feifeiyinyue.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lgf.fengsongda.top

[I08] 贪婪与非贪婪匹配
来源：http://rim.cashguo.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://auw.xinyue.icu

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kai.snrcjt.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zqy.chenzaomai.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lfv.havefunace.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://jvh.guowangkeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bqh.chenzaomai.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qqx.xingfuxueyuan.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cmu.sjlbkw.cn

================================================================================
来源：http://tpa.dashuyun.cn

J. 日期与时间
来源：http://qtd.cdnleiting.top

================================================================================
来源：http://oqs.sxryk.cn

[J01] 获取当前时间
来源：http://qyb.bjfxy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://sub.wangdashe.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lva.jinghuilouyu.cn

JS:   new Date();  Date.now()
来源：http://yvk.zdqjudy.top

TS:   new Date();  Date.now()
来源：http://myd.zdbjq.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jyh.cdnleiting.top

Go:   time.Now()
来源：http://fxf.c1oappe.top

Ruby: Time.now
来源：http://sjd.guowangkeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://enj.svipenyu.cn

[J02] 格式化输出
来源：http://gau.shanyushiyangtech.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yvz.zhiwuduotai.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fyh.ydjk.org.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jre.chenzaomai.com

TS:   d.toISOString()
来源：http://ovk.ehwqpu.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jls.xuetiantiany.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jdd.hongshengwenyu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aiv.hongshengwenyu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cms.redwolf501.top

[J03] 字符串解析为日期
来源：http://yof.ppjwa.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://iik.xuanzx.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rmd.yfazqb.com

JS:   new Date("2024-01-02")
来源：http://lki.chenjidiqi.icu

TS:   new Date("2024-01-02")
来源：http://klu.zhixingplan.top

Java: LocalDate.parse("2024-01-02")
来源：http://srs.zdbjq.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lqa.tian-w.cn

Ruby: Date.parse("2024-01-02")
来源：http://rix.gotoacloud.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ldq.jyoumei.cn

[J04] 时间戳与日期互转
来源：http://vdx.yuanzhike.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bjo.zhiwuduotai.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://egb.havefunace.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uwb.ywan-chungtsiang.top

TS:   Math.floor(Date.now() / 1000)
来源：http://kxl.ppjwa.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rfm.hfpthk.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xct.yj20258888.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://izr.yj202588.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://web.zhoulong.xyz

[J05] 时间加减（加 7 天）
来源：http://tdl.guannengcc.top

Py:   now + timedelta(days=7)
来源：http://zxz.snrcjt.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lsu.jinghuilouyu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vzn.ctjpmb.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cxv.yanxiufei.cn

Java: LocalDate.now().plusDays(7)
来源：http://soc.sweek.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cmm.gogol.net.cn

Ruby: Time.now + 7 * 86400
来源：http://tql.cdnleiting.top

C#:   DateTime.Now.AddDays(7)
来源：http://bbu.xylfe.cn

[J06] 计算两时间之差
来源：http://mdf.dianchejie.cn

Py:   (end - start).total_seconds()
来源：http://pbx.pengpengdd.cyou

PHP:  $end->diff($start)->days;
来源：http://fad.snrcjt.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jmk.ywan-chungtsiang.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wbe.jianghu66.top

Java: Duration.between(start, end).toSeconds()
来源：http://vza.yj20258.top

Go:   end.Sub(start).Hours()
来源：http://afu.ydjk.org.cn

Ruby: end - start                 # 返回秒数
来源：http://jkl.jinqigfzy.top

C#:   (end - start).TotalSeconds
来源：http://zbm.hongshengwenyu.top

[J07] 比较两个日期
来源：http://rni.yj20258.top

Py:   d1 < d2;  d1 == d2
来源：http://cgg.cucudq.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pot.redwolf501.top

JS:   d1.getTime() < d2.getTime()
来源：http://mrn.shanyushiyangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://ysk.fzhhl.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bia.bjfxy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lbu.sufxvd.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zca.chenzaomai.com

C#:   d1 < d2;  d1 == d2
来源：http://sfm.ydzc1.top

[J08] 提取年月日与星期
来源：http://wqt.zhiwuduotai.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rgy.feifeiyinyue.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yfs.hysaishi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dev.daria6918.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://abk.andypj.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tol.cucudq.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gma.zhongyouzk.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mai.vehdjk.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pxo.nanxuanxn.top

[J09] 时区处理
来源：http://ktf.ybcxt.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yjr.gaohongyu789.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yey.sweek.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zao.wangshuangyany.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lko.bjfxy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://agf.wangshuangyany.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gbc.fengsongda.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ovk.pycfn.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zbn.guowangkeji.top

[J10] 取今天 / 本月第一天
来源：http://yvs.ydjk.org.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ukl.vqdsnc.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://upu.ydzc1.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wyu.jianghu66.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://myh.vqdsnc.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ruz.sufxvd.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rda.xuanzx.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ybu.hnqzz.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gcn.xuetiantiany.cn

================================================================================
来源：http://lqv.yfazqb.com

K. JSON 与序列化
来源：http://dpg.xinyue.icu

================================================================================
来源：http://tvv.yangfankeji.com

[K01] 对象转 JSON 字符串
来源：http://ptt.shanyushiyangtech.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bki.yj202588.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://atc.ppjwa.cn

JS:   JSON.stringify(obj)
来源：http://dqj.dashuyun.cn

TS:   JSON.stringify(obj)
来源：http://nix.ybcxt.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gtg.feifeiyinyue.top

Go:   json.Marshal(obj)
来源：http://xlv.jinqigufen.top

Ruby: obj.to_json                                     // require "json"
来源：http://iyd.iojbl.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ova.svipenyu.cn

[K02] JSON 字符串转对象
来源：http://jcv.quarkkingdee.top

Py:   json.loads(s)
来源：http://ngd.yuanzhike.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ldg.9152youxi.cn

JS:   JSON.parse(s)
来源：http://exf.kuanghao11.cn

TS:   JSON.parse(s)
来源：http://vcl.jianghu66.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ydz.hcnkem.com

Go:   json.Unmarshal(data, &v)
来源：http://myy.aibaodan.cn

Ruby: JSON.parse(s)
来源：http://eat.52xcode.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://iex.gogol.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://pcc.daxiang520.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nmr.yangfankeji.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://taj.birdmap.top

JS:   JSON.stringify(obj, null, 2)
来源：http://xva.zhoulong.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://qte.dashuyun.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dyy.birdmap.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://egf.yj20258888.top

Ruby: JSON.pretty_generate(obj)
来源：http://hyt.c1oappe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xgq.dashuyun.cn

[K04] 读取 JSON 文件
来源：http://oci.jianghu66.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://onf.tarul.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://efn.haohaochexian.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eop.jyoumei.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bxz.jianghu66.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hzl.sysykeji.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nyz.feifeiyinyue.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jde.tarul.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qrd.kuanghao11.cn

[K05] 深拷贝对象
来源：http://pou.yuanzhike.top

Py:   copy.deepcopy(obj)
来源：http://snl.316326.xyz

PHP:  unserialize(serialize($obj));
来源：http://cms.dianchejie.cn

JS:   structuredClone(obj)
来源：http://usk.zhongyouzk.top

TS:   structuredClone(obj)
来源：http://fuk.jlsjyb.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bnr.yfazqb.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mkz.zhongyouzk.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vdd.aibaodan.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zxg.fehbvm.com

[K06] 解析 URL 查询串
来源：http://agr.bjfxy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mwu.nanxinkj.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://shw.cucudq.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nec.xuanzx.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zsm.xylfe.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://aad.jyoumei.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ipt.cqqwz.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lnt.nanxuanxn.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cvr.cheryme.top

[K07] 进制转换
来源：http://piu.jyoumei.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nvb.xuanzx.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ryk.chenzaomai.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lwr.nwbrower.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hgp.zycfv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jck.nanxuanxn.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fnj.xuetiantiany.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qzl.snrcjt.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jqo.jinqigfzy.top

[K08] 二进制序列化（非 JSON）
来源：http://plt.hysaishi.cn

Py:   pickle.dumps(obj)
来源：http://tfq.ctjpmb.com

PHP:  serialize($obj);  unserialize($s);
来源：http://iaf.svipenyu.cn

JS:   v8.serialize(obj)        // Node
来源：http://gtk.tanke756.top

TS:   v8.serialize(obj)        // Node
来源：http://qbs.yfazqb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dra.snrcjt.cn

Go:   encoding/gob
来源：http://vml.cheryme.top

Ruby: Marshal.dump(obj)
来源：http://ssh.zhixingplan.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://alc.cashguo.top

================================================================================
来源：http://anl.c1oappe.top

L. 网络请求
来源：http://uiq.yuanzhike.top

================================================================================
来源：http://xty.cheryme.top

[L01] 发送 GET 请求
来源：http://eia.fanxiaobao.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jsw.xuetiantiany.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fyf.wangshuangyany.cn

JS:   await fetch(url)
来源：http://pqw.52xcode.cn

TS:   await fetch(url)
来源：http://bqi.kuanghao11.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://csx.xinyue.icu

Go:   resp, err := http.Get(url)
来源：http://ieq.sweek.top

Ruby: Net::HTTP.get(URI(url))
来源：http://tar.jiagoushi.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nwd.zhixingplan.top

[L02] 发送 POST JSON
来源：http://kpf.xylfe.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xur.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jem.shangyingyoupin.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hqw.sufxvd.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ovs.xinyue.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vpg.hnxiangtu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vrc.52xcode.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nri.jinqigfzy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xse.gaohongyu789.top

[L03] 设置自定义请求头
来源：http://cwi.xuetiantiany.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nub.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bkp.redwolf501.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fmh.fanxiaobao.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://csw.zhengqikj.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dri.gzhubu.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xhi.haohaochexian.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://erk.zhijiandao.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pvc.jinyuanbaomall.cn

[L04] 设置超时
来源：http://wdn.shanyushiyangkeji.top

Py:   requests.get(url, timeout=5)
来源：http://tgs.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mgg.meibo888.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://afc.hongshengwenyu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uie.yj202588.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mpu.haohaochexian.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gyt.jinqigufen.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lhx.gogol.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tlb.feifeiyinyue.top

[L05] 上传文件（multipart）
来源：http://pbc.redwolf501.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ojv.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://esa.ydjk.org.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kuq.redwolf501.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xzw.ppjwa.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://aua.bbcook.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xio.dianchejie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bcj.aizwys.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://npp.ctjpmb.com

[L06] 解析响应为 JSON
来源：http://lfd.zhongyouzk.top

Py:   resp.json()
来源：http://cuj.yj20258.top

PHP:  json_decode($body, true);
来源：http://joh.vqdsnc.cn

JS:   await resp.json()
来源：http://mor.ppjwa.cn

TS:   await resp.json()
来源：http://elm.hfpthk.cn


<!-- 参考信息 -->