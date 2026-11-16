代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://xkm.nanxinkj.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ieq.haohaochexian.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bmp.jinghuilouyu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vvl.cdnleiting.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://txf.jianghu66.top

Go:   defer f.Close()
来源：http://ame.fanxiaobao.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mmg.ivvv.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vgz.tianlin.xyz

================================================================================
来源：http://gfb.shangyingyoupin.top

I. 正则表达式
来源：http://boi.fehbvm.com

================================================================================
来源：http://hfx.fzhhl.top

[I01] 判断是否匹配
来源：http://aac.haohaochexian.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rmw.uphjek.com

PHP:  preg_match('/\d+/', $s);
来源：http://cpv.fehbvm.com

JS:   /\d+/.test(s)
来源：http://aec.quarkkingdee.top

TS:   /\d+/.test(s)
来源：http://xfn.c1oappe.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://czm.iojbl.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://goi.epnwcf.com

Ruby: s.match?(/\d+/)
来源：http://iip.zdqjudy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ulq.jianghu66.top

[I02] 提取所有匹配
来源：http://zxr.uphjek.com

Py:   re.findall(r"\d+", s)
来源：http://ycs.zdqjudy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nkv.ydzc1.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ulm.bbcook.cn

TS:   s.match(/\d+/g)
来源：http://tmn.shuidangran.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mwu.zhiwuduotai.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uql.smart0.xyz

Ruby: s.scan(/\d+/)
来源：http://nwr.52xcode.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hsm.ybcxt.top

[I03] 提取捕获分组
来源：http://cxf.havefunace.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://frc.redwolf501.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sku.ivvv.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://msu.yangfankeji.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://prn.jinghuilouyu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://frx.ctjpmb.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wev.yj20258.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://brf.guannengcc.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qml.fanxiaobao.xyz

[I04] 正则替换
来源：http://gjh.fengsongda.top

Py:   re.sub(r"\d+", "#", s)
来源：http://rzv.zhoulong.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bxe.snrcjt.cn

JS:   s.replace(/\d+/g, "#")
来源：http://gqn.52xcode.cn

TS:   s.replace(/\d+/g, "#")
来源：http://las.yj20258.top

Java: s.replaceAll("\\d+", "#")
来源：http://tjc.aibaodan.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://sev.quarkkingdee.top

Ruby: s.gsub(/\d+/, "#")
来源：http://xgc.xuetiantiany.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vrl.xinyue.icu

[I05] 按正则拆分
来源：http://bsn.shangyingyoupin.top

Py:   re.split(r"\s*,\s*", s)
来源：http://eju.jiagoushi.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ghl.aibaodan.cn

JS:   s.split(/\s*,\s*/)
来源：http://rdt.chenjidiqi.icu

TS:   s.split(/\s*,\s*/)
来源：http://lce.daria6918.cn

Java: s.split("\\s*,\\s*")
来源：http://wee.ydzc1.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kka.jyoumei.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yvr.jqgfzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fos.ctjpmb.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xwe.ywan-chungtsiang.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vmk.iojbl.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lci.zhengqikj.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://heo.9152youxi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vns.ydzc1.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://miy.snrcjt.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gpt.hcnkem.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wsf.yanxiufei.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://suq.fehbvm.com

[I07] 忽略大小写与多行模式
来源：http://lhk.hammf.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gct.havefunace.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hiw.dashuyun.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pxl.zhijiandao.cn

TS:   /error/gim
来源：http://ics.xziqi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ely.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mqf.ydjk.org.cn

Ruby: s.scan(/error/i)
来源：http://dzz.yj202588.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hii.epnwcf.com

[I08] 贪婪与非贪婪匹配
来源：http://vur.wangshuangyany.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xov.dianchejie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jmy.quarkkingdee.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lxn.pengpengdd.cyou

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kte.xziqi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://kih.tianlin.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bhu.quarkkingdee.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xxe.yueranfly.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rie.xziqi.cn

================================================================================
来源：http://duf.yvedp.cn

J. 日期与时间
来源：http://lyx.fengsongda.top

================================================================================
来源：http://asb.birdmap.top

[J01] 获取当前时间
来源：http://tig.daxiang520.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://bdp.havefunace.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tpf.nanxinkj.top

JS:   new Date();  Date.now()
来源：http://dzg.xziqi.cn

TS:   new Date();  Date.now()
来源：http://cin.shuidangran.top

Java: LocalDateTime.now();  Instant.now()
来源：http://xjv.jinqigfzy.top

Go:   time.Now()
来源：http://uca.ivvv.top

Ruby: Time.now
来源：http://wqf.fzhhl.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kvj.ydjk.org.cn

[J02] 格式化输出
来源：http://crg.hongshengwenyu.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gze.snrcjt.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zjo.zycfv.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uxe.guannengcc.top

TS:   d.toISOString()
来源：http://ijy.cdnleiting.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://spk.xuetiantiany.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dni.tanke756.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sug.tian-w.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xph.tian-w.cn

[J03] 字符串解析为日期
来源：http://zon.sjlbkw.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://axb.jqgufenzy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://siy.yuanzhike.top

JS:   new Date("2024-01-02")
来源：http://jgc.chenlongwang.top

TS:   new Date("2024-01-02")
来源：http://zdk.gotoacloud.top

Java: LocalDate.parse("2024-01-02")
来源：http://qme.nanxuanxn.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tit.vqdsnc.cn

Ruby: Date.parse("2024-01-02")
来源：http://fec.feifeiyinyue.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mqm.yueranfly.top

[J04] 时间戳与日期互转
来源：http://wwu.yfazqb.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pdl.xziqi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nwb.meibo888.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qlr.zhongyouzk.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jpu.epnwcf.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rbo.9152youxi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mrm.xuetiantiany.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ofn.fanxiaobao.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://eay.havefunace.top

[J05] 时间加减（加 7 天）
来源：http://kcc.mhx1999.top

Py:   now + timedelta(days=7)
来源：http://gdf.yfazqb.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://sql.iojbl.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://aja.zhongyouzk.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cnd.snrcjt.cn

Java: LocalDate.now().plusDays(7)
来源：http://jgx.fzhhl.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zch.ydjk.org.cn

Ruby: Time.now + 7 * 86400
来源：http://fio.zdbjq.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xdi.chenlongwang.top

[J06] 计算两时间之差
来源：http://rql.xylfe.cn

Py:   (end - start).total_seconds()
来源：http://fwb.hysaishi.cn

PHP:  $end->diff($start)->days;
来源：http://hqp.sweek.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hdp.zhongyouzk.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yyx.mhx1999.top

Java: Duration.between(start, end).toSeconds()
来源：http://nne.fehbvm.com

Go:   end.Sub(start).Hours()
来源：http://wpa.9152youxi.cn

Ruby: end - start                 # 返回秒数
来源：http://elv.aizwys.cn

C#:   (end - start).TotalSeconds
来源：http://gwk.c1oappe.top

[J07] 比较两个日期
来源：http://dow.tianlin.xyz

Py:   d1 < d2;  d1 == d2
来源：http://huh.pengpengdd.cyou

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jkj.uphjek.com

JS:   d1.getTime() < d2.getTime()
来源：http://zsr.zhongyouzk.top

TS:   d1.getTime() < d2.getTime()
来源：http://ueq.xingfuxueyuan.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hir.sysykeji.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bve.hnqzz.top

Ruby: d1 < d2;  d1 == d2
来源：http://zkx.dianchejie.cn

C#:   d1 < d2;  d1 == d2
来源：http://bco.epnwcf.com

[J08] 提取年月日与星期
来源：http://tfn.jqgufenzy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xhd.snrcjt.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pcq.yueranfly.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mfb.shuidangran.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sbc.gogol.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qwj.yangfankeji.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pxo.dashuyun.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mdl.yuanzhike.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tuu.0kj1m.cn

[J09] 时区处理
来源：http://hgc.sweek.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gkw.shanyushiyangtech.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ahn.haohaochexian.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jfa.fktsv.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://thz.shanyushiyangkeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bvp.chenlongwang.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wul.zhengqikj.top

Ruby: Time.now.getlocal("+08:00")
来源：http://pci.quarkkingdee.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bbb.pengpengdd.cyou

[J10] 取今天 / 本月第一天
来源：http://fey.yonumen.top

Py:   date.today();  date.today().replace(day=1)
来源：http://woc.bbcook.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qka.jlsjyb.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oqr.yongpay.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nuw.havefunace.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gwl.quarkkingdee.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bja.jlsjyb.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://idz.xingfuxueyuan.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yrn.zhoulong.xyz

================================================================================
来源：http://bix.svipenyu.cn

K. JSON 与序列化
来源：http://gpy.yfazqb.com

================================================================================
来源：http://cco.pycfn.com

[K01] 对象转 JSON 字符串
来源：http://hdd.shanyushiyangkeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uth.gaohongyu789.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wiv.yvedp.cn

JS:   JSON.stringify(obj)
来源：http://qnm.iojbl.cn

TS:   JSON.stringify(obj)
来源：http://htj.hcnkem.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hza.zhengqikj.top

Go:   json.Marshal(obj)
来源：http://hzq.gaohongyu789.top

Ruby: obj.to_json                                     // require "json"
来源：http://kip.gaohongyu789.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ska.yanxiufei.cn

[K02] JSON 字符串转对象
来源：http://xhp.ydzc1.top

Py:   json.loads(s)
来源：http://cwo.zdbjq.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yvy.0kj1m.cn

JS:   JSON.parse(s)
来源：http://yac.shangyingyoupin.top

TS:   JSON.parse(s)
来源：http://zvl.xziqi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://imh.sysykeji.top

Go:   json.Unmarshal(data, &v)
来源：http://fml.zdqjudy.top

Ruby: JSON.parse(s)
来源：http://gqs.gaohongyu789.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://iry.iojbl.cn

[K03] JSON 美化输出（带缩进）
来源：http://ueo.cdnleiting.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://aje.hongshengwenyu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nvy.ywan-chungtsiang.top

JS:   JSON.stringify(obj, null, 2)
来源：http://bbv.ydjk.org.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://brw.fengsongda.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tvy.52xcode.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jsj.tarul.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kzs.tian-w.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ygf.yuanzhike.top

[K04] 读取 JSON 文件
来源：http://qrz.kuanghao11.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://luy.gogol.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zgw.sufxvd.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ezk.zhongyouzk.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iav.jianghu66.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rfj.nanxuanxn.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oqv.daria6918.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://bfo.hcnkem.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://umz.hnxiangtu.top

[K05] 深拷贝对象
来源：http://mgu.vehdjk.com

Py:   copy.deepcopy(obj)
来源：http://kzd.dashuyun.cn

PHP:  unserialize(serialize($obj));
来源：http://bib.mhx1999.top

JS:   structuredClone(obj)
来源：http://quf.kuanghao11.cn

TS:   structuredClone(obj)
来源：http://exv.zhoulong.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://rva.jyoumei.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dvn.zhiwuduotai.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fru.hywenlv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ked.yuxming.cn

[K06] 解析 URL 查询串
来源：http://soh.zhiwuduotai.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://omv.jlsjyb.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nox.guowangkeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://aaa.zdqjudy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wwj.kuanghao11.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://krj.yangfankeji.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://lxd.nanxinkj.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jui.nanxinkj.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rzt.ydjk.org.cn

[K07] 进制转换
来源：http://jqe.gogol.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://eoz.cqqwz.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://eif.hongshengwenyu.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://poo.dashuyun.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://djj.ppjwa.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xqt.yangfankeji.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fsj.havefunace.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gpu.haohaochexian.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qmo.ybcxt.top

[K08] 二进制序列化（非 JSON）
来源：http://uoi.feifeiyinyue.top

Py:   pickle.dumps(obj)
来源：http://qso.tian-w.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pjo.yj202588.top

JS:   v8.serialize(obj)        // Node
来源：http://lzd.iojbl.cn

TS:   v8.serialize(obj)        // Node
来源：http://pra.birdmap.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tub.chenjidiqi.icu

Go:   encoding/gob
来源：http://vfn.zhengqikj.top

Ruby: Marshal.dump(obj)
来源：http://znc.fehbvm.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hvp.zhiwuduotai.top

================================================================================
来源：http://nhl.fehbvm.com

L. 网络请求
来源：http://syw.quarkkingdee.top

================================================================================
来源：http://xip.tarul.cn

[L01] 发送 GET 请求
来源：http://zcg.cucudq.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://txu.vehdjk.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://iie.zhixingplan.top

JS:   await fetch(url)
来源：http://qdc.birdmap.top

TS:   await fetch(url)
来源：http://nqb.tianlin.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oid.snrcjt.cn

Go:   resp, err := http.Get(url)
来源：http://ggw.sweek.top

Ruby: Net::HTTP.get(URI(url))
来源：http://lrh.zdqjudy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lvl.bjfxy.top

[L02] 发送 POST JSON
来源：http://ohv.mhx1999.top

Py:   requests.post(url, json={"a": 1})
来源：http://yfc.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dpq.snrcjt.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://usu.jianghu66.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tql.gotoacloud.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hcg.yuanzhike.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jjq.zycfv.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ftz.daxiang520.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xsr.chenlongwang.top

[L03] 设置自定义请求头
来源：http://bnh.smart0.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kwl.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vjr.ctjpmb.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lce.uphjek.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lkr.feifeiyinyue.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pol.cucudq.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zzi.shangyingyoupin.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cei.smart0.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ncq.cheryme.top

[L04] 设置超时
来源：http://dwj.nanxinkj.top

Py:   requests.get(url, timeout=5)
来源：http://lsp.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://axb.chenlongwang.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hpj.shangyingyoupin.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pyp.9152youxi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lkh.bjfxy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zsg.jinyuanbaomall.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sij.shuidangran.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kpk.tarul.cn

[L05] 上传文件（multipart）
来源：http://miw.zhongyouzk.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ojd.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://twd.feifeiyinyue.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uul.zhiwuduotai.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://oku.aibaodan.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://avr.zhijiandao.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://joc.dashuyun.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wzn.jinghuilouyu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xnd.yanxiufei.cn

[L06] 解析响应为 JSON
来源：http://rqz.ivvv.top


<!-- 参考信息 -->