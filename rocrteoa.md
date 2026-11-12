代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://njt.c1oappe.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vih.shuidangran.top

Ruby: s.match?(/\d+/)
来源：http://ehh.gaohongyu789.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lnv.sufxvd.cn

[I02] 提取所有匹配
来源：http://ilh.ivvv.top

Py:   re.findall(r"\d+", s)
来源：http://cxf.zhaomingkeji.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fal.gzhubu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tuv.sxryk.cn

TS:   s.match(/\d+/g)
来源：http://rvz.feifeiyinyue.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hhb.cashguo.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uuh.hfpthk.cn

Ruby: s.scan(/\d+/)
来源：http://dxd.shuidangran.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pbw.shangyingyoupin.top

[I03] 提取捕获分组
来源：http://oye.sxryk.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rir.nanxinkj.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fli.cheryme.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vqa.birdmap.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qwd.shangyingyoupin.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xtd.yueranfly.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://edt.sxryk.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://akv.hesvh.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://eqi.hcnkem.com

[I04] 正则替换
来源：http://xrh.hongshengwenyu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://snt.yfazqb.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pzo.uphjek.com

JS:   s.replace(/\d+/g, "#")
来源：http://yfp.ywan-chungtsiang.top

TS:   s.replace(/\d+/g, "#")
来源：http://pfk.uphjek.com

Java: s.replaceAll("\\d+", "#")
来源：http://ibj.zhijiandao.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://yag.bjfxy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://pwc.zhaomingkeji.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://haj.gzhubu.top

[I05] 按正则拆分
来源：http://kqw.aizwys.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://whw.yfazqb.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://iaa.shanyushiyangtech.top

JS:   s.split(/\s*,\s*/)
来源：http://cux.hfpthk.cn

TS:   s.split(/\s*,\s*/)
来源：http://fre.yangfankeji.com

Java: s.split("\\s*,\\s*")
来源：http://nvb.yj202588.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://myb.ywan-chungtsiang.top

Ruby: s.split(/\s*,\s*/)
来源：http://lwt.chenlongwang.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fhh.sxryk.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pca.cheryme.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bhy.kuanghao11.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zcn.chenlongwang.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zhn.zhaomingkeji.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kvj.gotoacloud.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gzw.yonumen.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://led.zhixingplan.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yko.epnwcf.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yot.yongpay.top

[I07] 忽略大小写与多行模式
来源：http://yzo.jlsjyb.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cms.52xcode.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hcz.zhijiandao.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://usy.zhijiandao.cn

TS:   /error/gim
来源：http://lpy.shanyushiyangkeji.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://roi.yj20258888.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uoj.chenlongwang.top

Ruby: s.scan(/error/i)
来源：http://zfu.wangshuangyany.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pau.xuetiantiany.cn

[I08] 贪婪与非贪婪匹配
来源：http://bvj.xinyue.icu

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ngk.cdnleiting.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pyc.52xcode.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://slb.0kj1m.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vra.ydzc1.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://wnn.xziqi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rzb.cdnleiting.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uxe.fanxiaobao.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yni.havefunace.top

================================================================================
来源：http://joq.yuxming.cn

J. 日期与时间
来源：http://hde.yangfankeji.com

================================================================================
来源：http://xqi.yuxming.cn

[J01] 获取当前时间
来源：http://qic.ydzc1.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://moy.redwolf501.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lpc.havefunace.top

JS:   new Date();  Date.now()
来源：http://gav.hammf.cn

TS:   new Date();  Date.now()
来源：http://cck.cashguo.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ums.ydjk.org.cn

Go:   time.Now()
来源：http://nlg.shuidangran.top

Ruby: Time.now
来源：http://xbn.hysaishi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://brb.fzhhl.top

[J02] 格式化输出
来源：http://mii.pengpengdd.cyou

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xcq.zhiwuduotai.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://krl.jlsjyb.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uqp.snrcjt.cn

TS:   d.toISOString()
来源：http://cma.yongpay.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://flg.yangfankeji.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bwd.smart0.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gqf.hcnkem.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://awd.aibaodan.cn

[J03] 字符串解析为日期
来源：http://thh.yongpay.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jtw.feifeiyinyue.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rrl.shanyushiyangkeji.top

JS:   new Date("2024-01-02")
来源：http://kpc.hnxiangtu.top

TS:   new Date("2024-01-02")
来源：http://bth.yuxming.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bva.zhixingplan.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qmq.jianghu66.top

Ruby: Date.parse("2024-01-02")
来源：http://adv.zdbjq.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jxz.zdbjq.cn

[J04] 时间戳与日期互转
来源：http://zmo.zdbjq.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vne.sweek.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://okc.mhx1999.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dtw.cdnleiting.top

TS:   Math.floor(Date.now() / 1000)
来源：http://wnh.yj202588.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vjx.iojbl.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lhq.jinghuilouyu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://myz.yangfankeji.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://eue.haohaochexian.top

[J05] 时间加减（加 7 天）
来源：http://ojq.yj20258.top

Py:   now + timedelta(days=7)
来源：http://jgz.redwolf501.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://pij.shangyingyoupin.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://idp.ppjwa.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xjx.jqgufenzy.top

Java: LocalDate.now().plusDays(7)
来源：http://igc.zhengqikj.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://arp.xuanzx.com

Ruby: Time.now + 7 * 86400
来源：http://xlt.shanyushiyangkeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://rtt.0kj1m.cn

[J06] 计算两时间之差
来源：http://hyz.zdqjudy.top

Py:   (end - start).total_seconds()
来源：http://igi.sysykeji.top

PHP:  $end->diff($start)->days;
来源：http://asg.cheryme.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xre.yuxming.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sqg.shangyingyoupin.top

Java: Duration.between(start, end).toSeconds()
来源：http://icx.wangdashe.top

Go:   end.Sub(start).Hours()
来源：http://cnu.svipenyu.cn

Ruby: end - start                 # 返回秒数
来源：http://fsj.cheryme.top

C#:   (end - start).TotalSeconds
来源：http://tgk.ppjwa.cn

[J07] 比较两个日期
来源：http://ozj.quarkkingdee.top

Py:   d1 < d2;  d1 == d2
来源：http://aeb.xuanzx.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kqr.zhaomingkeji.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://ump.cheryme.top

TS:   d1.getTime() < d2.getTime()
来源：http://vqp.haohaochexian.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://omv.xinyue.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lop.9152youxi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://tpt.xuetiantiany.cn

C#:   d1 < d2;  d1 == d2
来源：http://rjy.zhoulong.xyz

[J08] 提取年月日与星期
来源：http://ktl.shzxlz.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dyo.guannengcc.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ssa.xuanzx.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ybf.meibo888.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nyu.shzxlz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ivp.52xcode.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://txr.quarkkingdee.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dwk.zdqjudy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pdc.zdbjq.cn

[J09] 时区处理
来源：http://yai.zhixingplan.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wty.tarul.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qwq.pengpengdd.cyou

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dpn.fanxiaobao.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xak.guowangkeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dna.meibo888.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://koh.zhengqikj.top

Ruby: Time.now.getlocal("+08:00")
来源：http://plt.yj20258.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ekp.wangshuangyany.cn

[J10] 取今天 / 本月第一天
来源：http://hqc.shanyushiyangtech.top

Py:   date.today();  date.today().replace(day=1)
来源：http://fyl.zhiwuduotai.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zdp.zhijiandao.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://akp.yuxming.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://edw.yuxming.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hvo.havefunace.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://aus.cashguo.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tsm.svipenyu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nmo.cqqwz.cn

================================================================================
来源：http://egi.shanyushiyangtech.top

K. JSON 与序列化
来源：http://gnq.zhixingplan.top

================================================================================
来源：http://vvm.yongpay.top

[K01] 对象转 JSON 字符串
来源：http://nxt.ppjwa.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://woo.dianchejie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ncc.fktsv.cn

JS:   JSON.stringify(obj)
来源：http://rnb.vehdjk.com

TS:   JSON.stringify(obj)
来源：http://nvx.feifeiyinyue.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lek.daria6918.cn

Go:   json.Marshal(obj)
来源：http://ind.jqgufenzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://xdj.fktsv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hmg.ybcxt.top

[K02] JSON 字符串转对象
来源：http://fbv.tian-w.cn

Py:   json.loads(s)
来源：http://tpv.zhiwuduotai.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://utt.jqgufenzy.top

JS:   JSON.parse(s)
来源：http://xve.guowangkeji.top

TS:   JSON.parse(s)
来源：http://sqi.zhoulong.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oft.sufxvd.cn

Go:   json.Unmarshal(data, &v)
来源：http://bko.fzhhl.top

Ruby: JSON.parse(s)
来源：http://ggs.hammf.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qvs.kuanghao11.cn

[K03] JSON 美化输出（带缩进）
来源：http://zpr.xylfe.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qjw.nanxuanxn.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fpq.jiagoushi.top

JS:   JSON.stringify(obj, null, 2)
来源：http://zzs.ehwqpu.com

TS:   JSON.stringify(obj, null, 2)
来源：http://zoe.316326.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hxi.fanxiaobao.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uva.hammf.cn

Ruby: JSON.pretty_generate(obj)
来源：http://uyh.jiagoushi.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://inw.sysykeji.top

[K04] 读取 JSON 文件
来源：http://jwx.snrcjt.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fue.cucudq.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vig.tianlin.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://icp.yangfankeji.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jpy.shanyushiyangkeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uoh.nwbrower.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ebe.nanxuanxn.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ksj.nanxuanxn.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tba.zhoulong.xyz

[K05] 深拷贝对象
来源：http://wjx.hnxiangtu.top

Py:   copy.deepcopy(obj)
来源：http://utw.shuidangran.top

PHP:  unserialize(serialize($obj));
来源：http://hpc.gotoacloud.top

JS:   structuredClone(obj)
来源：http://eeg.vqdsnc.cn

TS:   structuredClone(obj)
来源：http://dph.yj20258.top

Java: // 手写拷贝构造，或序列化往返
来源：http://kaf.jinqigufen.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tuf.yonumen.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rcy.sysykeji.top

C#:   // 序列化往返，或自定义 Clone
来源：http://qrc.tanke756.top

[K06] 解析 URL 查询串
来源：http://ljf.wangdashe.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://crv.xziqi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yqw.fzhhl.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sdb.yj202588.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://coe.zhongyouzk.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bnw.epnwcf.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://xcc.yanxiufei.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rsg.cdnleiting.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nom.c1oappe.top

[K07] 进制转换
来源：http://lzk.yonumen.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ctt.cucudq.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vdd.sjlbkw.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pkt.9152youxi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gjh.yvedp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hgh.yj202588.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://suw.aizwys.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cno.chenjidiqi.icu

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hum.pengpengdd.cyou

[K08] 二进制序列化（非 JSON）
来源：http://mkl.nanxuanxn.top

Py:   pickle.dumps(obj)
来源：http://mky.xziqi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bpk.wangdashe.top

JS:   v8.serialize(obj)        // Node
来源：http://pxu.shanyushiyangtech.top

TS:   v8.serialize(obj)        // Node
来源：http://cfv.316326.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jlj.vqdsnc.cn

Go:   encoding/gob
来源：http://znu.ydzc1.top

Ruby: Marshal.dump(obj)
来源：http://bfr.nanxinkj.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rqh.c1oappe.top

================================================================================
来源：http://ejz.shanyushiyangkeji.top

L. 网络请求
来源：http://fwr.yj20258.top

================================================================================
来源：http://kdc.9152youxi.cn

[L01] 发送 GET 请求
来源：http://zom.gotoacloud.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bdh.uphjek.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lvv.dianchejie.cn

JS:   await fetch(url)
来源：http://kia.hnxiangtu.top

TS:   await fetch(url)
来源：http://rwc.vqdsnc.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hrw.fanxiaobao.xyz

Go:   resp, err := http.Get(url)
来源：http://eih.9152youxi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://uyq.ybcxt.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pph.zdbjq.cn

[L02] 发送 POST JSON
来源：http://ykb.snrcjt.cn

Py:   requests.post(url, json={"a": 1})
来源：http://luz.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vqx.dianchejie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bzx.nwbrower.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wqj.316326.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ctz.zhijiandao.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xoo.pengpengdd.cyou

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://alq.fanxiaobao.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fvy.yuanzhike.top

[L03] 设置自定义请求头
来源：http://sjm.mhx1999.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bkg.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nbm.yonumen.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zbc.yuxming.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wwp.sxryk.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bbq.sysykeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ycu.guowangkeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mxp.gotoacloud.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jqc.fehbvm.com

[L04] 设置超时
来源：http://wpt.jqgufenzy.top

Py:   requests.get(url, timeout=5)
来源：http://wzm.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ruq.guannengcc.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ziz.yuanzhike.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jia.0kj1m.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rif.hcnkem.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qdv.fzhhl.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://oum.meibo888.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dkc.iojbl.cn

[L05] 上传文件（multipart）
来源：http://vxb.hongshengwenyu.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ncl.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kcf.sysykeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sjj.jinqigufen.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sdt.nwbrower.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ywa.smart0.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yqc.daxiang520.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pze.fzhhl.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ftz.gotoacloud.top

[L06] 解析响应为 JSON
来源：http://urv.guowangkeji.top

Py:   resp.json()
来源：http://egr.daria6918.cn

PHP:  json_decode($body, true);
来源：http://tob.zhaomingkeji.xyz

JS:   await resp.json()
来源：http://ere.hywenlv.cn

TS:   await resp.json()
来源：http://pqx.quarkkingdee.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cki.gotoacloud.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dlr.hywenlv.cn

Ruby: JSON.parse(resp.body)
来源：http://qsd.daria6918.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://atr.ehwqpu.com

[L07] 处理 HTTP 状态码
来源：http://wpv.nanxuanxn.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rpu.aizwys.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zrf.hongshengwenyu.top

JS:   resp.ok;  resp.status
来源：http://zgv.cashguo.top

TS:   resp.ok;  resp.status
来源：http://sph.yfazqb.com

Java: resp.statusCode()
来源：http://tgq.meibo888.top

Go:   resp.StatusCode
来源：http://vzn.fanxiaobao.xyz

Ruby: resp.code.to_i
来源：http://ibh.fzhhl.top


<!-- 参考信息 -->