代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ukb.zhaomingkeji.xyz

Go:   defer f.Close()
来源：http://vjt.chenjidiqi.icu

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vqo.xingfuxueyuan.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pmp.bbcook.cn

================================================================================
来源：http://fmr.cqqwz.cn

I. 正则表达式
来源：http://pbm.ydzc1.top

================================================================================
来源：http://ifk.xylfe.cn

[I01] 判断是否匹配
来源：http://kyf.quarkkingdee.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xbp.meibo888.top

PHP:  preg_match('/\d+/', $s);
来源：http://siq.havefunace.top

JS:   /\d+/.test(s)
来源：http://nup.fengsongda.top

TS:   /\d+/.test(s)
来源：http://bga.guowangkeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://swz.zhiwuduotai.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wvy.epnwcf.com

Ruby: s.match?(/\d+/)
来源：http://nvq.jiagoushi.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vqj.nwbrower.top

[I02] 提取所有匹配
来源：http://wfk.yj20258.top

Py:   re.findall(r"\d+", s)
来源：http://kea.9152youxi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dob.jqgfzy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://msb.ybcxt.top

TS:   s.match(/\d+/g)
来源：http://qwb.zhoulong.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rme.aizwys.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wqy.xingfuxueyuan.xyz

Ruby: s.scan(/\d+/)
来源：http://ilu.sufxvd.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uzm.shuidangran.top

[I03] 提取捕获分组
来源：http://ehc.gotoacloud.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jxk.aizwys.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ari.tanke756.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fjx.jinyuanbaomall.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://irf.zhijiandao.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tbz.xingfuxueyuan.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lvl.zhijiandao.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wru.fengsongda.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jcr.kuanghao11.cn

[I04] 正则替换
来源：http://bsc.shanyushiyangtech.top

Py:   re.sub(r"\d+", "#", s)
来源：http://awk.hywenlv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ssa.birdmap.top

JS:   s.replace(/\d+/g, "#")
来源：http://jrs.sweek.top

TS:   s.replace(/\d+/g, "#")
来源：http://lpi.ctjpmb.com

Java: s.replaceAll("\\d+", "#")
来源：http://emj.c1oappe.top

Go:   re.ReplaceAllString(s, "#")
来源：http://uar.meibo888.top

Ruby: s.gsub(/\d+/, "#")
来源：http://yqt.yangfankeji.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ghz.andypj.xyz

[I05] 按正则拆分
来源：http://pwl.xinyue.icu

Py:   re.split(r"\s*,\s*", s)
来源：http://qgq.hnxiangtu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qta.jinghuilouyu.cn

JS:   s.split(/\s*,\s*/)
来源：http://cvp.hcnkem.com

TS:   s.split(/\s*,\s*/)
来源：http://bbq.shangyingyoupin.top

Java: s.split("\\s*,\\s*")
来源：http://cll.ybcxt.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wpp.zycfv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://cms.havefunace.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wbm.hcnkem.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://toa.52xcode.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kvu.chenzaomai.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://goe.meibo888.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yvd.yueranfly.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ncn.birdmap.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://iql.sysykeji.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lup.zycfv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rkw.dashuyun.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cqc.sxryk.cn

[I07] 忽略大小写与多行模式
来源：http://mxz.hongshengwenyu.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ayv.haohaochexian.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mff.nwbrower.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ucl.yueranfly.top

TS:   /error/gim
来源：http://edo.quarkkingdee.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://osi.nanxinkj.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fqs.hnxiangtu.top

Ruby: s.scan(/error/i)
来源：http://bhk.wangdashe.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rzv.jinqigfzy.top

[I08] 贪婪与非贪婪匹配
来源：http://aoy.nanxinkj.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dxh.ybcxt.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bjn.jiagoushi.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qmp.andypj.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tyl.xuetiantiany.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tnw.yvedp.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://eap.xinyue.icu

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://iey.fengsongda.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cfh.chenzaomai.com

================================================================================
来源：http://zwr.ywan-chungtsiang.top

J. 日期与时间
来源：http://hyx.aibaodan.cn

================================================================================
来源：http://oet.andypj.xyz

[J01] 获取当前时间
来源：http://hkt.jianghu66.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ycr.zycfv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xld.nanxinkj.top

JS:   new Date();  Date.now()
来源：http://tfx.yongpay.top

TS:   new Date();  Date.now()
来源：http://iag.hfpthk.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hmf.pycfn.com

Go:   time.Now()
来源：http://zhv.ydjk.org.cn

Ruby: Time.now
来源：http://hcc.tian-w.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wes.yueranfly.top

[J02] 格式化输出
来源：http://whh.ybcxt.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eyo.hnqzz.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gfq.chenlongwang.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rbh.daxiang520.top

TS:   d.toISOString()
来源：http://axl.wangdashe.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cic.fzhhl.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xze.daxiang520.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mcb.wangshuangyany.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vqh.xuanzx.com

[J03] 字符串解析为日期
来源：http://itu.birdmap.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ziu.feifeiyinyue.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ncj.zhaomingkeji.xyz

JS:   new Date("2024-01-02")
来源：http://ule.sxryk.cn

TS:   new Date("2024-01-02")
来源：http://wzu.0kj1m.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jeq.jiagoushi.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mfh.chenlongwang.top

Ruby: Date.parse("2024-01-02")
来源：http://hng.gzhubu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yhm.yonumen.top

[J04] 时间戳与日期互转
来源：http://rjc.jlsjyb.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://aue.hesvh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sat.hywenlv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://twl.sysykeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jvd.hammf.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://msr.dashuyun.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nib.snrcjt.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hbh.shzxlz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tcj.sufxvd.cn

[J05] 时间加减（加 7 天）
来源：http://mbp.yfazqb.com

Py:   now + timedelta(days=7)
来源：http://okp.yj202588.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://poh.tianlin.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kdn.svipenyu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kwd.9152youxi.cn

Java: LocalDate.now().plusDays(7)
来源：http://rka.zhoulong.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wyq.haohaochexian.top

Ruby: Time.now + 7 * 86400
来源：http://wnm.jinyuanbaomall.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fty.hesvh.cn

[J06] 计算两时间之差
来源：http://owk.ivvv.top

Py:   (end - start).total_seconds()
来源：http://vvg.fzhhl.top

PHP:  $end->diff($start)->days;
来源：http://jud.haohaochexian.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ftb.chenjidiqi.icu

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mal.xuanzx.com

Java: Duration.between(start, end).toSeconds()
来源：http://hfe.gotoacloud.top

Go:   end.Sub(start).Hours()
来源：http://yei.yonumen.top

Ruby: end - start                 # 返回秒数
来源：http://mlc.ywan-chungtsiang.top

C#:   (end - start).TotalSeconds
来源：http://oic.chenlongwang.top

[J07] 比较两个日期
来源：http://slq.fanxiaobao.xyz

Py:   d1 < d2;  d1 == d2
来源：http://suc.gzhubu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pdn.ydjk.org.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dsr.kuanghao11.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fod.jyoumei.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ixh.gotoacloud.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mum.haohaochexian.top

Ruby: d1 < d2;  d1 == d2
来源：http://vrj.gogol.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://zyu.tian-w.cn

[J08] 提取年月日与星期
来源：http://efe.jiagoushi.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fcd.yonumen.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://biq.ehwqpu.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jzw.xuanzx.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yah.bbcook.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zcd.epnwcf.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vxs.yanxiufei.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yxx.xinyue.icu

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cbq.tianlin.xyz

[J09] 时区处理
来源：http://ppk.zdbjq.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pjl.316326.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lgj.feifeiyinyue.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pgf.xingfuxueyuan.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xka.52xcode.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mhd.ywan-chungtsiang.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vbl.havefunace.top

Ruby: Time.now.getlocal("+08:00")
来源：http://kiy.yj20258888.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://aoz.hammf.cn

[J10] 取今天 / 本月第一天
来源：http://dfu.yangfankeji.com

Py:   date.today();  date.today().replace(day=1)
来源：http://cln.pycfn.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pmy.zhoulong.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blz.zdqjudy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://otp.jqgufenzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ydr.uphjek.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cci.wangshuangyany.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pyu.fanxiaobao.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ovz.jqgfzy.top

================================================================================
来源：http://idz.yfazqb.com

K. JSON 与序列化
来源：http://ged.tarul.cn

================================================================================
来源：http://zud.yj202588.top

[K01] 对象转 JSON 字符串
来源：http://uah.zhiwuduotai.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vou.sysykeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://thc.ivvv.top

JS:   JSON.stringify(obj)
来源：http://urw.wangshuangyany.cn

TS:   JSON.stringify(obj)
来源：http://izy.yongpay.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wut.yfazqb.com

Go:   json.Marshal(obj)
来源：http://zpg.uphjek.com

Ruby: obj.to_json                                     // require "json"
来源：http://awl.zhiwuduotai.top

C#:   JsonSerializer.Serialize(obj)
来源：http://heb.mhx1999.top

[K02] JSON 字符串转对象
来源：http://lpz.jinghuilouyu.cn

Py:   json.loads(s)
来源：http://noi.fanxiaobao.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tkw.havefunace.top

JS:   JSON.parse(s)
来源：http://eyc.tianlin.xyz

TS:   JSON.parse(s)
来源：http://bem.shanyushiyangtech.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mcm.cheryme.top

Go:   json.Unmarshal(data, &v)
来源：http://pmb.ydjk.org.cn

Ruby: JSON.parse(s)
来源：http://zbq.0kj1m.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mtb.yueranfly.top

[K03] JSON 美化输出（带缩进）
来源：http://ncm.haohaochexian.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nns.ctjpmb.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ifu.xziqi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zvz.gotoacloud.top

TS:   JSON.stringify(obj, null, 2)
来源：http://min.wangshuangyany.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ler.fengsongda.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kzn.wangdashe.top

Ruby: JSON.pretty_generate(obj)
来源：http://wrz.ydjk.org.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://oks.cashguo.top

[K04] 读取 JSON 文件
来源：http://ezm.kuanghao11.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://aml.epnwcf.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://utf.cdnleiting.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wyk.jqgufenzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wrv.cucudq.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rys.ppjwa.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cdq.gzhubu.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://snp.tian-w.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mbx.chenjidiqi.icu

[K05] 深拷贝对象
来源：http://qrr.ybcxt.top

Py:   copy.deepcopy(obj)
来源：http://jph.xuanzx.com

PHP:  unserialize(serialize($obj));
来源：http://ajv.jinghuilouyu.cn

JS:   structuredClone(obj)
来源：http://fsq.nwbrower.top

TS:   structuredClone(obj)
来源：http://wub.aizwys.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dee.jinqigfzy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vdn.havefunace.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vwu.wangshuangyany.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pka.jiagoushi.top

[K06] 解析 URL 查询串
来源：http://clo.yongpay.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vsh.dashuyun.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rjy.shuidangran.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vlb.tanke756.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qiv.gogol.net.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ehr.snrcjt.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zhq.vqdsnc.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rcf.sufxvd.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tty.xuetiantiany.cn

[K07] 进制转换
来源：http://exu.ppjwa.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bas.yfazqb.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lak.ydjk.org.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cff.iojbl.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hhb.yj20258.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tqp.jinghuilouyu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://akx.iojbl.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ies.uphjek.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wbd.bjfxy.top

[K08] 二进制序列化（非 JSON）
来源：http://bij.yanxiufei.cn

Py:   pickle.dumps(obj)
来源：http://uot.yangfankeji.com

PHP:  serialize($obj);  unserialize($s);
来源：http://ojm.cqqwz.cn

JS:   v8.serialize(obj)        // Node
来源：http://pjl.cheryme.top

TS:   v8.serialize(obj)        // Node
来源：http://sfg.c1oappe.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mbh.uphjek.com

Go:   encoding/gob
来源：http://mkc.xylfe.cn

Ruby: Marshal.dump(obj)
来源：http://drr.zhixingplan.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jpg.hfpthk.cn

================================================================================
来源：http://cad.aibaodan.cn

L. 网络请求
来源：http://nrx.sysykeji.top

================================================================================
来源：http://czr.epnwcf.com

[L01] 发送 GET 请求
来源：http://rwm.zhixingplan.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://iuw.zycfv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://whq.quarkkingdee.top

JS:   await fetch(url)
来源：http://lct.sjlbkw.cn

TS:   await fetch(url)
来源：http://gvh.wangshuangyany.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rgj.nanxuanxn.top

Go:   resp, err := http.Get(url)
来源：http://dcj.ydjk.org.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wed.cashguo.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://awj.guannengcc.top

[L02] 发送 POST JSON
来源：http://vym.cqqwz.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xus.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xdt.hcnkem.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://apx.epnwcf.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mzt.zhaomingkeji.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hoj.yj20258888.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://iza.hesvh.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qec.ybcxt.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ack.yfazqb.com

[L03] 设置自定义请求头
来源：http://hjf.sweek.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wpm.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fll.aizwys.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ynl.xylfe.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bjw.fktsv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xrh.fktsv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://djk.havefunace.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zss.sjlbkw.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zio.cucudq.cn

[L04] 设置超时
来源：http://wxl.xinyue.icu

Py:   requests.get(url, timeout=5)
来源：http://tbp.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lil.daria6918.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sjw.aizwys.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hrz.hywenlv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cnb.chenjidiqi.icu

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rbb.tanke756.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://opb.guannengcc.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mzq.svipenyu.cn

[L05] 上传文件（multipart）
来源：http://hsg.vqdsnc.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xjr.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lto.chenjidiqi.icu

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hvw.fktsv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://oce.yongpay.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xzv.jianghu66.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zzq.yueranfly.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://psx.shzxlz.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lmm.yanxiufei.cn

[L06] 解析响应为 JSON
来源：http://oyl.bbcook.cn

Py:   resp.json()
来源：http://tcm.bbcook.cn

PHP:  json_decode($body, true);
来源：http://wyb.hammf.cn

JS:   await resp.json()
来源：http://qzu.meibo888.top

TS:   await resp.json()
来源：http://pwq.gogol.net.cn


<!-- 参考信息 -->