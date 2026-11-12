代发 wailian999

================================================================================
来源：http://tgp.meibo888.top

I. 正则表达式
来源：http://sao.cucudq.cn

================================================================================
来源：http://qsz.ydjk.org.cn

[I01] 判断是否匹配
来源：http://dij.tanke756.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://asr.chenlongwang.top

PHP:  preg_match('/\d+/', $s);
来源：http://yqv.yangfankeji.com

JS:   /\d+/.test(s)
来源：http://sea.mhx1999.top

TS:   /\d+/.test(s)
来源：http://kdv.chenlongwang.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://urg.tanke756.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yij.daxiang520.top

Ruby: s.match?(/\d+/)
来源：http://hzx.fehbvm.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nas.yj20258.top

[I02] 提取所有匹配
来源：http://tqn.yueranfly.top

Py:   re.findall(r"\d+", s)
来源：http://dpu.fehbvm.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kpl.yueranfly.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lns.tanke756.top

TS:   s.match(/\d+/g)
来源：http://btn.pengpengdd.cyou

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nhn.zhijiandao.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fgo.52xcode.cn

Ruby: s.scan(/\d+/)
来源：http://pxo.gzhubu.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ono.xuetiantiany.cn

[I03] 提取捕获分组
来源：http://smh.yj202588.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cyn.hfpthk.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lzw.chenlongwang.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hza.shanyushiyangtech.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uki.zhengqikj.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ksd.vqdsnc.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qcm.aibaodan.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vbg.dashuyun.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yfz.sjlbkw.cn

[I04] 正则替换
来源：http://ria.mhx1999.top

Py:   re.sub(r"\d+", "#", s)
来源：http://bgf.wangdashe.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pcv.bbcook.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dpj.zhengqikj.top

TS:   s.replace(/\d+/g, "#")
来源：http://csz.shzxlz.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qlk.sxryk.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://nrw.sjlbkw.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qdj.yuxming.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nxi.iojbl.cn

[I05] 按正则拆分
来源：http://pjf.xinyue.icu

Py:   re.split(r"\s*,\s*", s)
来源：http://hbi.xinyue.icu

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hae.yj20258.top

JS:   s.split(/\s*,\s*/)
来源：http://kaj.fengsongda.top

TS:   s.split(/\s*,\s*/)
来源：http://zyo.yongpay.top

Java: s.split("\\s*,\\s*")
来源：http://hao.wangshuangyany.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nyl.zhengqikj.top

Ruby: s.split(/\s*,\s*/)
来源：http://nem.shanyushiyangkeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ulo.tian-w.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lrc.jyoumei.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tzi.xuetiantiany.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qat.ybcxt.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rnt.shanyushiyangtech.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fhi.tian-w.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mgl.0kj1m.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yos.0kj1m.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sik.birdmap.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oci.vqdsnc.cn

[I07] 忽略大小写与多行模式
来源：http://euy.xingfuxueyuan.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zmm.zhiwuduotai.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://huq.quarkkingdee.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cxm.hnqzz.top

TS:   /error/gim
来源：http://fcp.tianlin.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://aug.tian-w.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dnf.pycfn.com

Ruby: s.scan(/error/i)
来源：http://lfb.nanxinkj.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tfh.xziqi.cn

[I08] 贪婪与非贪婪匹配
来源：http://wvl.redwolf501.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://azt.zhaomingkeji.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://idi.ctjpmb.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qee.nanxuanxn.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lne.bjfxy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://kcl.xylfe.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cqy.aizwys.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lgo.cdnleiting.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://umt.sysykeji.top

================================================================================
来源：http://lyc.hnxiangtu.top

J. 日期与时间
来源：http://xff.kuanghao11.cn

================================================================================
来源：http://pvf.zdqjudy.top

[J01] 获取当前时间
来源：http://tvy.zhijiandao.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://edn.birdmap.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tsb.havefunace.top

JS:   new Date();  Date.now()
来源：http://edq.hnqzz.top

TS:   new Date();  Date.now()
来源：http://hcq.nanxinkj.top

Java: LocalDateTime.now();  Instant.now()
来源：http://uee.hongshengwenyu.top

Go:   time.Now()
来源：http://otx.shzxlz.cn

Ruby: Time.now
来源：http://pbp.chenjidiqi.icu

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://itq.gotoacloud.top

[J02] 格式化输出
来源：http://lss.gogol.net.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://csl.pengpengdd.cyou

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nkx.cheryme.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gei.xingfuxueyuan.xyz

TS:   d.toISOString()
来源：http://chp.dianchejie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bjp.bbcook.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mff.xuanzx.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mig.meibo888.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qzd.hesvh.cn

[J03] 字符串解析为日期
来源：http://xku.hnxiangtu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bro.gaohongyu789.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pww.fengsongda.top

JS:   new Date("2024-01-02")
来源：http://mdw.aizwys.cn

TS:   new Date("2024-01-02")
来源：http://ezc.epnwcf.com

Java: LocalDate.parse("2024-01-02")
来源：http://iwg.ivvv.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dgt.hcnkem.com

Ruby: Date.parse("2024-01-02")
来源：http://tha.haohaochexian.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bcv.fengsongda.top

[J04] 时间戳与日期互转
来源：http://krb.ydjk.org.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nrj.fanxiaobao.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://for.shzxlz.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nsz.epnwcf.com

TS:   Math.floor(Date.now() / 1000)
来源：http://vyg.iojbl.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gfj.cucudq.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gaa.hysaishi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jej.dashuyun.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gah.shanyushiyangtech.top

[J05] 时间加减（加 7 天）
来源：http://nkj.cqqwz.cn

Py:   now + timedelta(days=7)
来源：http://don.havefunace.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://nat.svipenyu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ccu.aizwys.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://udp.bbcook.cn

Java: LocalDate.now().plusDays(7)
来源：http://hbk.hfpthk.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dpg.ctjpmb.com

Ruby: Time.now + 7 * 86400
来源：http://ieb.fzhhl.top

C#:   DateTime.Now.AddDays(7)
来源：http://gim.zdbjq.cn

[J06] 计算两时间之差
来源：http://shd.pycfn.com

Py:   (end - start).total_seconds()
来源：http://qlg.zhongyouzk.top

PHP:  $end->diff($start)->days;
来源：http://qxp.yj20258.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://amv.xinyue.icu

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zyf.52xcode.cn

Java: Duration.between(start, end).toSeconds()
来源：http://myw.shzxlz.cn

Go:   end.Sub(start).Hours()
来源：http://qjm.zdqjudy.top

Ruby: end - start                 # 返回秒数
来源：http://xyj.fengsongda.top

C#:   (end - start).TotalSeconds
来源：http://omy.jianghu66.top

[J07] 比较两个日期
来源：http://scu.gzhubu.top

Py:   d1 < d2;  d1 == d2
来源：http://drz.yvedp.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://juv.nanxinkj.top

JS:   d1.getTime() < d2.getTime()
来源：http://rnu.mhx1999.top

TS:   d1.getTime() < d2.getTime()
来源：http://npr.birdmap.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lrk.sysykeji.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://oqc.dianchejie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://dih.ppjwa.cn

C#:   d1 < d2;  d1 == d2
来源：http://ggl.hnqzz.top

[J08] 提取年月日与星期
来源：http://mgn.tian-w.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qmy.shangyingyoupin.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://khn.zdqjudy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fzk.hammf.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pnu.zhengqikj.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kbk.wangshuangyany.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ugb.yvedp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hcr.gzhubu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gib.dianchejie.cn

[J09] 时区处理
来源：http://ovp.fengsongda.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fjf.chenzaomai.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hzd.fzhhl.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bwg.shuidangran.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jgx.jlsjyb.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://flv.snrcjt.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pbt.jqgufenzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://xxh.zhongyouzk.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ixg.shzxlz.cn

[J10] 取今天 / 本月第一天
来源：http://dwf.jinqigufen.top

Py:   date.today();  date.today().replace(day=1)
来源：http://flt.tianlin.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://oxa.zhiwuduotai.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://idj.pengpengdd.cyou

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://udm.andypj.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ifc.zhijiandao.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ocz.jinqigufen.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hct.fanxiaobao.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cuw.zdbjq.cn

================================================================================
来源：http://aed.xuanzx.com

K. JSON 与序列化
来源：http://jcd.sufxvd.cn

================================================================================
来源：http://upb.chenlongwang.top

[K01] 对象转 JSON 字符串
来源：http://kyq.mhx1999.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lhc.xinyue.icu

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rvi.xinyue.icu

JS:   JSON.stringify(obj)
来源：http://dub.iojbl.cn

TS:   JSON.stringify(obj)
来源：http://sxf.zhixingplan.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://agr.yangfankeji.com

Go:   json.Marshal(obj)
来源：http://tnr.bbcook.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jnt.tarul.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xmu.shanyushiyangtech.top

[K02] JSON 字符串转对象
来源：http://ndo.316326.xyz

Py:   json.loads(s)
来源：http://azc.xingfuxueyuan.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zrj.sjlbkw.cn

JS:   JSON.parse(s)
来源：http://vus.ctjpmb.com

TS:   JSON.parse(s)
来源：http://ddx.sxryk.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pbn.yvedp.cn

Go:   json.Unmarshal(data, &v)
来源：http://vtz.tanke756.top

Ruby: JSON.parse(s)
来源：http://ccc.yuxming.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rhl.guannengcc.top

[K03] JSON 美化输出（带缩进）
来源：http://bio.jinyuanbaomall.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://civ.sysykeji.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qrb.hnxiangtu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://apg.fengsongda.top

TS:   JSON.stringify(obj, null, 2)
来源：http://fml.hammf.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://myi.daria6918.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ylg.jqgufenzy.top

Ruby: JSON.pretty_generate(obj)
来源：http://tfr.xuetiantiany.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gni.zhengqikj.top

[K04] 读取 JSON 文件
来源：http://sfu.svipenyu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nzl.gaohongyu789.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sef.hesvh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vtd.birdmap.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cuj.mhx1999.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cwd.svipenyu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://arc.yj20258.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://rsb.hysaishi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fnw.dianchejie.cn

[K05] 深拷贝对象
来源：http://ttz.hongshengwenyu.top

Py:   copy.deepcopy(obj)
来源：http://hys.fengsongda.top

PHP:  unserialize(serialize($obj));
来源：http://htm.nanxuanxn.top

JS:   structuredClone(obj)
来源：http://ymn.sysykeji.top

TS:   structuredClone(obj)
来源：http://rml.daria6918.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mtb.pycfn.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qco.cdnleiting.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ckd.zhijiandao.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ikj.tarul.cn

[K06] 解析 URL 查询串
来源：http://fih.xingfuxueyuan.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ncy.jinqigufen.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fne.zycfv.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uga.jinqigufen.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sdq.dianchejie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uqj.yuanzhike.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://dho.xziqi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zsv.tianlin.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jex.xuetiantiany.cn

[K07] 进制转换
来源：http://gay.ywan-chungtsiang.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oum.hysaishi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xlu.xingfuxueyuan.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://krx.yuxming.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rtr.gaohongyu789.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ezc.dianchejie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blo.jqgufenzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jsc.jinghuilouyu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kbd.daxiang520.top

[K08] 二进制序列化（非 JSON）
来源：http://vpn.zhengqikj.top

Py:   pickle.dumps(obj)
来源：http://cje.gogol.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gxd.cdnleiting.top

JS:   v8.serialize(obj)        // Node
来源：http://iqm.ydzc1.top

TS:   v8.serialize(obj)        // Node
来源：http://khi.nwbrower.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://eqe.fanxiaobao.xyz

Go:   encoding/gob
来源：http://twg.yueranfly.top

Ruby: Marshal.dump(obj)
来源：http://ibq.ywan-chungtsiang.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vyg.jinqigufen.top

================================================================================
来源：http://cyq.iojbl.cn

L. 网络请求
来源：http://nqr.snrcjt.cn

================================================================================
来源：http://suw.sufxvd.cn

[L01] 发送 GET 请求
来源：http://zli.jlsjyb.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yhw.xuanzx.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uwb.xinyue.icu

JS:   await fetch(url)
来源：http://qys.hesvh.cn

TS:   await fetch(url)
来源：http://kiz.52xcode.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://imp.aizwys.cn

Go:   resp, err := http.Get(url)
来源：http://snd.vehdjk.com

Ruby: Net::HTTP.get(URI(url))
来源：http://bxy.birdmap.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ahd.chenjidiqi.icu

[L02] 发送 POST JSON
来源：http://ryd.sweek.top

Py:   requests.post(url, json={"a": 1})
来源：http://eoi.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://shi.gzhubu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://agy.kuanghao11.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mcf.gzhubu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pyx.sysykeji.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://btr.havefunace.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://eon.gzhubu.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mqr.haohaochexian.top

[L03] 设置自定义请求头
来源：http://wxr.bjfxy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://emk.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rut.zhixingplan.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wdg.iojbl.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cft.epnwcf.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pur.yueranfly.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cfc.xuetiantiany.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xww.gogol.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hnl.wangshuangyany.cn

[L04] 设置超时
来源：http://dto.jinqigfzy.top

Py:   requests.get(url, timeout=5)
来源：http://xoc.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mva.9152youxi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rab.zhixingplan.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wvc.yj202588.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yng.sweek.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://puj.yj20258.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rjc.52xcode.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sbr.kuanghao11.cn

[L05] 上传文件（multipart）
来源：http://nhk.haohaochexian.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tcv.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rcm.epnwcf.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://iib.cdnleiting.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yvg.andypj.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rfd.cheryme.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kjj.wangdashe.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://iwn.jlsjyb.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://elq.tarul.cn

[L06] 解析响应为 JSON
来源：http://gsi.havefunace.top

Py:   resp.json()
来源：http://gyw.yj20258888.top

PHP:  json_decode($body, true);
来源：http://foj.redwolf501.top

JS:   await resp.json()
来源：http://fve.yvedp.cn

TS:   await resp.json()
来源：http://vih.dashuyun.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gzl.c1oappe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rmh.wangshuangyany.cn

Ruby: JSON.parse(resp.body)
来源：http://tjs.jyoumei.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mkt.fehbvm.com


<!-- 参考信息 -->