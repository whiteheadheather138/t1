代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ldz.cucudq.cn

Go:   defer f.Close()
来源：http://ndq.jinyuanbaomall.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fov.guannengcc.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mtm.hesvh.cn

================================================================================
来源：http://roq.jinqigufen.top

I. 正则表达式
来源：http://dvy.aizwys.cn

================================================================================
来源：http://gjs.zdbjq.cn

[I01] 判断是否匹配
来源：http://jhr.mhx1999.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bta.haohaochexian.top

PHP:  preg_match('/\d+/', $s);
来源：http://qwv.redwolf501.top

JS:   /\d+/.test(s)
来源：http://fej.cucudq.cn

TS:   /\d+/.test(s)
来源：http://cdl.cashguo.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hwb.havefunace.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dwi.hfpthk.cn

Ruby: s.match?(/\d+/)
来源：http://gad.jinghuilouyu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ual.zhoulong.xyz

[I02] 提取所有匹配
来源：http://ppf.epnwcf.com

Py:   re.findall(r"\d+", s)
来源：http://yif.shangyingyoupin.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mut.quarkkingdee.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sdx.pengpengdd.cyou

TS:   s.match(/\d+/g)
来源：http://qdi.yuxming.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kyv.gogol.net.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://oec.gzhubu.top

Ruby: s.scan(/\d+/)
来源：http://qhe.feifeiyinyue.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://llm.tian-w.cn

[I03] 提取捕获分组
来源：http://noo.gzhubu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://orj.haohaochexian.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nia.hnxiangtu.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bzy.yongpay.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qie.daxiang520.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mju.cucudq.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ovf.haohaochexian.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pkk.ivvv.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nci.pengpengdd.cyou

[I04] 正则替换
来源：http://ddo.dianchejie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://cjx.xylfe.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rxi.gzhubu.top

JS:   s.replace(/\d+/g, "#")
来源：http://npd.andypj.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://ejm.ydzc1.top

Java: s.replaceAll("\\d+", "#")
来源：http://kcn.fehbvm.com

Go:   re.ReplaceAllString(s, "#")
来源：http://ymw.yuanzhike.top

Ruby: s.gsub(/\d+/, "#")
来源：http://miw.jlsjyb.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gug.fktsv.cn

[I05] 按正则拆分
来源：http://tct.hysaishi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mns.wangdashe.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xrf.quarkkingdee.top

JS:   s.split(/\s*,\s*/)
来源：http://ptw.hywenlv.cn

TS:   s.split(/\s*,\s*/)
来源：http://yjk.bbcook.cn

Java: s.split("\\s*,\\s*")
来源：http://nar.ybcxt.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://grn.yj202588.top

Ruby: s.split(/\s*,\s*/)
来源：http://tbi.sjlbkw.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://efn.xuanzx.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bmn.yangfankeji.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lyx.cdnleiting.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://szz.tanke756.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rzw.cucudq.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bux.cheryme.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://msf.fzhhl.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ijt.haohaochexian.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://eoe.aizwys.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uoq.jlsjyb.cn

[I07] 忽略大小写与多行模式
来源：http://snt.yj202588.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://emi.gogol.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wso.svipenyu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nwl.epnwcf.com

TS:   /error/gim
来源：http://uii.0kj1m.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kbi.chenlongwang.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ilo.fzhhl.top

Ruby: s.scan(/error/i)
来源：http://bpa.hongshengwenyu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gjf.redwolf501.top

[I08] 贪婪与非贪婪匹配
来源：http://aew.xziqi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fwe.fanxiaobao.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rad.jlsjyb.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://byw.fengsongda.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qpd.gotoacloud.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://oqk.yfazqb.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://opn.zhiwuduotai.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gwy.fktsv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bor.yueranfly.top

================================================================================
来源：http://gva.yuxming.cn

J. 日期与时间
来源：http://vop.hnxiangtu.top

================================================================================
来源：http://vgn.316326.xyz

[J01] 获取当前时间
来源：http://hcq.cdnleiting.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://grn.havefunace.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://oon.zycfv.cn

JS:   new Date();  Date.now()
来源：http://nah.shanyushiyangtech.top

TS:   new Date();  Date.now()
来源：http://qfh.yangfankeji.com

Java: LocalDateTime.now();  Instant.now()
来源：http://lnh.jianghu66.top

Go:   time.Now()
来源：http://zhx.zdqjudy.top

Ruby: Time.now
来源：http://fgg.wangshuangyany.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pgr.quarkkingdee.top

[J02] 格式化输出
来源：http://rqw.gotoacloud.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ubt.yvedp.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xqo.xuanzx.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fhf.hesvh.cn

TS:   d.toISOString()
来源：http://fry.ydjk.org.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ktk.gogol.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fbc.andypj.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ksz.hysaishi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oyn.jlsjyb.cn

[J03] 字符串解析为日期
来源：http://liw.guowangkeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://scg.hfpthk.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nfs.316326.xyz

JS:   new Date("2024-01-02")
来源：http://pqa.0kj1m.cn

TS:   new Date("2024-01-02")
来源：http://jbx.hysaishi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://lwj.hammf.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mhc.jqgufenzy.top

Ruby: Date.parse("2024-01-02")
来源：http://twq.zhoulong.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://osq.zhongyouzk.top

[J04] 时间戳与日期互转
来源：http://qnm.zhengqikj.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://oal.guowangkeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iky.wangdashe.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nte.snrcjt.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zjn.nwbrower.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://umh.yonumen.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://not.xylfe.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ewj.xingfuxueyuan.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://eco.jlsjyb.cn

[J05] 时间加减（加 7 天）
来源：http://ngu.vqdsnc.cn

Py:   now + timedelta(days=7)
来源：http://bhc.jlsjyb.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vcm.tanke756.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ecr.meibo888.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jgw.hywenlv.cn

Java: LocalDate.now().plusDays(7)
来源：http://zaz.xinyue.icu

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fuz.shuidangran.top

Ruby: Time.now + 7 * 86400
来源：http://uts.shanyushiyangtech.top

C#:   DateTime.Now.AddDays(7)
来源：http://uqc.yj202588.top

[J06] 计算两时间之差
来源：http://gvm.jinqigufen.top

Py:   (end - start).total_seconds()
来源：http://dvy.pycfn.com

PHP:  $end->diff($start)->days;
来源：http://wfl.nwbrower.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mxg.ehwqpu.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lub.vehdjk.com

Java: Duration.between(start, end).toSeconds()
来源：http://qvu.guannengcc.top

Go:   end.Sub(start).Hours()
来源：http://orf.zhoulong.xyz

Ruby: end - start                 # 返回秒数
来源：http://nka.316326.xyz

C#:   (end - start).TotalSeconds
来源：http://cti.jinghuilouyu.cn

[J07] 比较两个日期
来源：http://utl.pengpengdd.cyou

Py:   d1 < d2;  d1 == d2
来源：http://nzw.zhiwuduotai.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dsy.ywan-chungtsiang.top

JS:   d1.getTime() < d2.getTime()
来源：http://emh.cdnleiting.top

TS:   d1.getTime() < d2.getTime()
来源：http://szj.chenzaomai.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ows.zhongyouzk.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hni.mhx1999.top

Ruby: d1 < d2;  d1 == d2
来源：http://hkg.cheryme.top

C#:   d1 < d2;  d1 == d2
来源：http://igb.ctjpmb.com

[J08] 提取年月日与星期
来源：http://zts.guowangkeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fkl.gaohongyu789.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jmt.yj20258.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ubn.zhongyouzk.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wwl.52xcode.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://eyo.shuidangran.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fmv.tanke756.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://iok.shanyushiyangtech.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vux.jinqigufen.top

[J09] 时区处理
来源：http://hwt.shzxlz.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pcn.hywenlv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nbh.wangshuangyany.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uku.chenlongwang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ray.zhijiandao.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qmp.chenlongwang.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fae.uphjek.com

Ruby: Time.now.getlocal("+08:00")
来源：http://jhh.jinyuanbaomall.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yvd.zdbjq.cn

[J10] 取今天 / 本月第一天
来源：http://myt.jinqigfzy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://spt.ehwqpu.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pfo.sufxvd.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hoq.tarul.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://axm.fktsv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uoq.sufxvd.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bqd.hongshengwenyu.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jzy.chenzaomai.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gqc.hysaishi.cn

================================================================================
来源：http://qqz.xziqi.cn

K. JSON 与序列化
来源：http://uyw.c1oappe.top

================================================================================
来源：http://dmn.0kj1m.cn

[K01] 对象转 JSON 字符串
来源：http://smu.feifeiyinyue.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nuo.gaohongyu789.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://keb.guannengcc.top

JS:   JSON.stringify(obj)
来源：http://ahh.pengpengdd.cyou

TS:   JSON.stringify(obj)
来源：http://rtn.zhoulong.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nmy.daria6918.cn

Go:   json.Marshal(obj)
来源：http://ndi.nwbrower.top

Ruby: obj.to_json                                     // require "json"
来源：http://efg.shzxlz.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bfh.mhx1999.top

[K02] JSON 字符串转对象
来源：http://ggn.fengsongda.top

Py:   json.loads(s)
来源：http://xrb.yfazqb.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://geu.yueranfly.top

JS:   JSON.parse(s)
来源：http://xmm.ppjwa.cn

TS:   JSON.parse(s)
来源：http://iff.nanxuanxn.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://utg.52xcode.cn

Go:   json.Unmarshal(data, &v)
来源：http://mye.jinqigfzy.top

Ruby: JSON.parse(s)
来源：http://zgq.tianlin.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gnt.bjfxy.top

[K03] JSON 美化输出（带缩进）
来源：http://jnr.bjfxy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yiy.smart0.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cjw.yueranfly.top

JS:   JSON.stringify(obj, null, 2)
来源：http://xiu.aibaodan.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://udd.ehwqpu.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://unn.bbcook.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zfq.jinqigufen.top

Ruby: JSON.pretty_generate(obj)
来源：http://ses.yj20258.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yan.hnxiangtu.top

[K04] 读取 JSON 文件
来源：http://opc.havefunace.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qyp.jinghuilouyu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://deq.zhongyouzk.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kdc.shuidangran.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blb.zhixingplan.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sly.cashguo.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rks.feifeiyinyue.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://arc.ywan-chungtsiang.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hix.gotoacloud.top

[K05] 深拷贝对象
来源：http://iiu.316326.xyz

Py:   copy.deepcopy(obj)
来源：http://vmk.hfpthk.cn

PHP:  unserialize(serialize($obj));
来源：http://wln.yfazqb.com

JS:   structuredClone(obj)
来源：http://jlo.kuanghao11.cn

TS:   structuredClone(obj)
来源：http://fhe.chenzaomai.com

Java: // 手写拷贝构造，或序列化往返
来源：http://wzu.chenjidiqi.icu

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rvj.yongpay.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tzu.ybcxt.top

C#:   // 序列化往返，或自定义 Clone
来源：http://whe.tanke756.top

[K06] 解析 URL 查询串
来源：http://euw.tanke756.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wri.daxiang520.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sfx.fehbvm.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jbz.xinyue.icu

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rkx.tianlin.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ywb.tarul.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vku.dashuyun.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ldd.yonumen.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gvb.tarul.cn

[K07] 进制转换
来源：http://usi.sxryk.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zqa.birdmap.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hjj.jyoumei.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zdc.epnwcf.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wsh.tarul.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://inp.zdbjq.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uiu.epnwcf.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uor.jinqigufen.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gwb.hnxiangtu.top

[K08] 二进制序列化（非 JSON）
来源：http://iek.zhoulong.xyz

Py:   pickle.dumps(obj)
来源：http://iop.iojbl.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nlf.jqgufenzy.top

JS:   v8.serialize(obj)        // Node
来源：http://zuf.cqqwz.cn

TS:   v8.serialize(obj)        // Node
来源：http://mms.yj20258888.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kmf.zhoulong.xyz

Go:   encoding/gob
来源：http://ewt.xylfe.cn

Ruby: Marshal.dump(obj)
来源：http://gir.hnqzz.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mau.mhx1999.top

================================================================================
来源：http://qtd.hnxiangtu.top

L. 网络请求
来源：http://ypu.nanxinkj.top

================================================================================
来源：http://ftz.nanxinkj.top

[L01] 发送 GET 请求
来源：http://pmy.wangshuangyany.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bed.guannengcc.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mei.hywenlv.cn

JS:   await fetch(url)
来源：http://xzm.wangdashe.top

TS:   await fetch(url)
来源：http://vgr.zycfv.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qja.ehwqpu.com

Go:   resp, err := http.Get(url)
来源：http://pye.fktsv.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fjr.yvedp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vrj.gaohongyu789.top

[L02] 发送 POST JSON
来源：http://pel.yangfankeji.com

Py:   requests.post(url, json={"a": 1})
来源：http://aly.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wmv.zhiwuduotai.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://guu.guannengcc.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rsa.svipenyu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pdy.xuanzx.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rao.guannengcc.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ffq.hcnkem.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://glp.jinyuanbaomall.cn

[L03] 设置自定义请求头
来源：http://opt.yj20258888.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dyj.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qts.yj20258888.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rpz.shuidangran.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dai.0kj1m.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kvt.hcnkem.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mra.xuetiantiany.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rnj.jinqigfzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rxw.zdqjudy.top

[L04] 设置超时
来源：http://atc.yangfankeji.com

Py:   requests.get(url, timeout=5)
来源：http://nfv.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ijc.cdnleiting.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hjg.jiagoushi.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jqa.guannengcc.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ucw.ehwqpu.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jzf.nanxuanxn.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jfh.pengpengdd.cyou

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wcp.yvedp.cn

[L05] 上传文件（multipart）
来源：http://gvn.snrcjt.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rzb.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mwa.c1oappe.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pyy.guowangkeji.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zmu.yuxming.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pix.svipenyu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://szd.zhongyouzk.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://did.shzxlz.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fbq.cucudq.cn

[L06] 解析响应为 JSON
来源：http://wkh.hywenlv.cn

Py:   resp.json()
来源：http://qnc.jinyuanbaomall.cn

PHP:  json_decode($body, true);
来源：http://hue.sufxvd.cn

JS:   await resp.json()
来源：http://aks.haohaochexian.top

TS:   await resp.json()
来源：http://ngo.jqgufenzy.top


<!-- 参考信息 -->