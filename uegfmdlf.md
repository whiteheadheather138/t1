代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fcc.zhongyouzk.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yap.redwolf501.top

Ruby: s.match?(/\d+/)
来源：http://diq.cdnleiting.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jwv.svipenyu.cn

[I02] 提取所有匹配
来源：http://oxo.yangfankeji.com

Py:   re.findall(r"\d+", s)
来源：http://etp.sjlbkw.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fxk.jqgfzy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ohr.yongpay.top

TS:   s.match(/\d+/g)
来源：http://xdc.tanke756.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lhp.chenzaomai.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uaw.daria6918.cn

Ruby: s.scan(/\d+/)
来源：http://qws.gaohongyu789.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bkk.yanxiufei.cn

[I03] 提取捕获分组
来源：http://hqm.tanke756.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jcv.zhoulong.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://roi.wangshuangyany.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mbs.sjlbkw.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dzz.epnwcf.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xix.dashuyun.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ugj.zycfv.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://myb.jianghu66.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hgo.tanke756.top

[I04] 正则替换
来源：http://ofx.xuanzx.com

Py:   re.sub(r"\d+", "#", s)
来源：http://sbh.52xcode.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://aww.sxryk.cn

JS:   s.replace(/\d+/g, "#")
来源：http://csk.dianchejie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nei.jinqigfzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://lqr.epnwcf.com

Go:   re.ReplaceAllString(s, "#")
来源：http://ida.vehdjk.com

Ruby: s.gsub(/\d+/, "#")
来源：http://hsp.aibaodan.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://olf.sxryk.cn

[I05] 按正则拆分
来源：http://iqr.sufxvd.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kts.vehdjk.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://why.dashuyun.cn

JS:   s.split(/\s*,\s*/)
来源：http://opd.fehbvm.com

TS:   s.split(/\s*,\s*/)
来源：http://khp.smart0.xyz

Java: s.split("\\s*,\\s*")
来源：http://jfr.ybcxt.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://feo.hnqzz.top

Ruby: s.split(/\s*,\s*/)
来源：http://vva.zhoulong.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rju.shanyushiyangkeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hfa.ybcxt.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lop.cqqwz.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tmm.yonumen.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oed.hesvh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zth.cheryme.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gof.hysaishi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://oma.cashguo.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://imy.meibo888.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://akb.chenjidiqi.icu

[I07] 忽略大小写与多行模式
来源：http://ely.guowangkeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hjb.sweek.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wsc.hcnkem.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gfl.ehwqpu.com

TS:   /error/gim
来源：http://dst.yanxiufei.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ine.snrcjt.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gqi.yangfankeji.com

Ruby: s.scan(/error/i)
来源：http://znd.nanxuanxn.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://geg.redwolf501.top

[I08] 贪婪与非贪婪匹配
来源：http://nsd.cqqwz.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sjo.wangdashe.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lxc.yvedp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qvu.zhaomingkeji.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fuf.gotoacloud.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://kcd.hywenlv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://end.nanxuanxn.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xfl.zycfv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://klj.zdbjq.cn

================================================================================
来源：http://pat.yvedp.cn

J. 日期与时间
来源：http://mku.hesvh.cn

================================================================================
来源：http://xfr.wangdashe.top

[J01] 获取当前时间
来源：http://str.sxryk.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://nsl.52xcode.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xqh.jinqigfzy.top

JS:   new Date();  Date.now()
来源：http://qev.gogol.net.cn

TS:   new Date();  Date.now()
来源：http://rkm.hywenlv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pvb.wangdashe.top

Go:   time.Now()
来源：http://kjt.birdmap.top

Ruby: Time.now
来源：http://ivu.fzhhl.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://noi.zhiwuduotai.top

[J02] 格式化输出
来源：http://ehl.vqdsnc.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sgq.cdnleiting.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fja.gaohongyu789.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tbb.nanxinkj.top

TS:   d.toISOString()
来源：http://nky.cheryme.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ubf.meibo888.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wni.nwbrower.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ncr.zhoulong.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tuj.sufxvd.cn

[J03] 字符串解析为日期
来源：http://mzf.jyoumei.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://far.yangfankeji.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yng.hysaishi.cn

JS:   new Date("2024-01-02")
来源：http://ilc.zhijiandao.cn

TS:   new Date("2024-01-02")
来源：http://vtm.mhx1999.top

Java: LocalDate.parse("2024-01-02")
来源：http://yhg.fehbvm.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jpd.guannengcc.top

Ruby: Date.parse("2024-01-02")
来源：http://xot.zhijiandao.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://anm.xylfe.cn

[J04] 时间戳与日期互转
来源：http://alp.wangshuangyany.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ocw.snrcjt.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ukw.316326.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cmc.zdbjq.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zwe.havefunace.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uvf.svipenyu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rzx.feifeiyinyue.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hxf.gogol.net.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rqq.guannengcc.top

[J05] 时间加减（加 7 天）
来源：http://iia.daxiang520.top

Py:   now + timedelta(days=7)
来源：http://bvs.sysykeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://wmv.gzhubu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nhi.zdqjudy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://eqo.snrcjt.cn

Java: LocalDate.now().plusDays(7)
来源：http://scy.tarul.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://iwm.jqgfzy.top

Ruby: Time.now + 7 * 86400
来源：http://gha.316326.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://fxo.ivvv.top

[J06] 计算两时间之差
来源：http://wtu.gotoacloud.top

Py:   (end - start).total_seconds()
来源：http://fmf.yvedp.cn

PHP:  $end->diff($start)->days;
来源：http://cvp.yuanzhike.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fhu.ybcxt.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ktl.pycfn.com

Java: Duration.between(start, end).toSeconds()
来源：http://ing.zhaomingkeji.xyz

Go:   end.Sub(start).Hours()
来源：http://kgo.hfpthk.cn

Ruby: end - start                 # 返回秒数
来源：http://pvx.fengsongda.top

C#:   (end - start).TotalSeconds
来源：http://tfa.zhaomingkeji.xyz

[J07] 比较两个日期
来源：http://san.jqgfzy.top

Py:   d1 < d2;  d1 == d2
来源：http://orx.ybcxt.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ldz.pengpengdd.cyou

JS:   d1.getTime() < d2.getTime()
来源：http://xjg.fehbvm.com

TS:   d1.getTime() < d2.getTime()
来源：http://sum.feifeiyinyue.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gpn.hcnkem.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bwe.hammf.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mdp.feifeiyinyue.top

C#:   d1 < d2;  d1 == d2
来源：http://kqx.cheryme.top

[J08] 提取年月日与星期
来源：http://azh.shanyushiyangkeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pzk.cashguo.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ego.zhongyouzk.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ntk.shanyushiyangkeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ctw.nanxinkj.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yti.mhx1999.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://syn.haohaochexian.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tdq.jqgfzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://abc.sweek.top

[J09] 时区处理
来源：http://dob.nwbrower.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sji.316326.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ddk.yonumen.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ifa.havefunace.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mrp.jqgfzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://chz.chenzaomai.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kbr.sweek.top

Ruby: Time.now.getlocal("+08:00")
来源：http://hjt.hongshengwenyu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ifz.svipenyu.cn

[J10] 取今天 / 本月第一天
来源：http://znf.epnwcf.com

Py:   date.today();  date.today().replace(day=1)
来源：http://kou.hysaishi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xyd.jinqigufen.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qan.kuanghao11.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mri.shuidangran.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zyc.yuxming.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dot.gogol.net.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://oax.pycfn.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://aii.zhixingplan.top

================================================================================
来源：http://nyi.hesvh.cn

K. JSON 与序列化
来源：http://cqr.birdmap.top

================================================================================
来源：http://nns.dianchejie.cn

[K01] 对象转 JSON 字符串
来源：http://eug.epnwcf.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tbz.shuidangran.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gjb.tian-w.cn

JS:   JSON.stringify(obj)
来源：http://uya.hcnkem.com

TS:   JSON.stringify(obj)
来源：http://krl.yanxiufei.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jpv.jqgfzy.top

Go:   json.Marshal(obj)
来源：http://jkl.jlsjyb.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zpz.svipenyu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qyr.sjlbkw.cn

[K02] JSON 字符串转对象
来源：http://hts.tianlin.xyz

Py:   json.loads(s)
来源：http://qei.svipenyu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qao.yj20258888.top

JS:   JSON.parse(s)
来源：http://fea.316326.xyz

TS:   JSON.parse(s)
来源：http://wmm.shzxlz.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bav.shzxlz.cn

Go:   json.Unmarshal(data, &v)
来源：http://utr.zhiwuduotai.top

Ruby: JSON.parse(s)
来源：http://qmt.zycfv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ole.yuanzhike.top

[K03] JSON 美化输出（带缩进）
来源：http://otg.nanxuanxn.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yeo.ywan-chungtsiang.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xdz.aizwys.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zwp.chenlongwang.top

TS:   JSON.stringify(obj, null, 2)
来源：http://nib.vqdsnc.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hlp.yj20258888.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cxk.fzhhl.top

Ruby: JSON.pretty_generate(obj)
来源：http://uxi.zdqjudy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vbj.aibaodan.cn

[K04] 读取 JSON 文件
来源：http://tlt.316326.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xfg.52xcode.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://noy.xinyue.icu

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bbb.hammf.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tmu.chenlongwang.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xke.sufxvd.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ldt.jinqigfzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ujm.cheryme.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xqv.xinyue.icu

[K05] 深拷贝对象
来源：http://rao.yj20258888.top

Py:   copy.deepcopy(obj)
来源：http://bca.jqgufenzy.top

PHP:  unserialize(serialize($obj));
来源：http://nlm.havefunace.top

JS:   structuredClone(obj)
来源：http://scm.zhiwuduotai.top

TS:   structuredClone(obj)
来源：http://brr.sysykeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://bfc.hongshengwenyu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hly.shzxlz.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rog.jinyuanbaomall.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pir.zdbjq.cn

[K06] 解析 URL 查询串
来源：http://wfv.tianlin.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ufc.gogol.net.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://civ.ppjwa.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jis.52xcode.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://epi.fanxiaobao.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jkf.jqgufenzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://pqd.shangyingyoupin.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gow.hfpthk.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dbg.0kj1m.cn

[K07] 进制转换
来源：http://exo.yfazqb.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jkh.xuetiantiany.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mck.cqqwz.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ged.shangyingyoupin.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://puc.yj202588.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rdp.zhiwuduotai.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oqb.fktsv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://top.tianlin.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://okc.ppjwa.cn

[K08] 二进制序列化（非 JSON）
来源：http://mqi.sxryk.cn

Py:   pickle.dumps(obj)
来源：http://xxu.jianghu66.top

PHP:  serialize($obj);  unserialize($s);
来源：http://vxx.yj20258.top

JS:   v8.serialize(obj)        // Node
来源：http://ghc.zycfv.cn

TS:   v8.serialize(obj)        // Node
来源：http://yvq.c1oappe.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gyg.yfazqb.com

Go:   encoding/gob
来源：http://irg.sufxvd.cn

Ruby: Marshal.dump(obj)
来源：http://ugh.bbcook.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://adm.hesvh.cn

================================================================================
来源：http://aqy.9152youxi.cn

L. 网络请求
来源：http://obh.hammf.cn

================================================================================
来源：http://eie.ydzc1.top

[L01] 发送 GET 请求
来源：http://awj.tanke756.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ysz.daxiang520.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fze.vehdjk.com

JS:   await fetch(url)
来源：http://qjb.wangdashe.top

TS:   await fetch(url)
来源：http://gsa.daria6918.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fqc.haohaochexian.top

Go:   resp, err := http.Get(url)
来源：http://tsy.jinqigufen.top

Ruby: Net::HTTP.get(URI(url))
来源：http://wgn.316326.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ppz.shuidangran.top

[L02] 发送 POST JSON
来源：http://riv.fengsongda.top

Py:   requests.post(url, json={"a": 1})
来源：http://dfe.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cme.fehbvm.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bnk.c1oappe.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zea.zhiwuduotai.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tui.iojbl.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bqg.cucudq.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ksp.sweek.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://shi.gogol.net.cn

[L03] 设置自定义请求头
来源：http://ukl.sxryk.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ckl.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vwv.hysaishi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ynk.tanke756.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dww.nwbrower.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lmt.ivvv.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://oml.zhixingplan.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jau.jqgfzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://coa.hysaishi.cn

[L04] 设置超时
来源：http://wew.cdnleiting.top

Py:   requests.get(url, timeout=5)
来源：http://phq.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hur.yuanzhike.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ogf.hongshengwenyu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uqc.52xcode.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://aew.shuidangran.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xwa.nwbrower.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://akq.yvedp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vvt.yvedp.cn

[L05] 上传文件（multipart）
来源：http://jhv.nanxuanxn.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://crx.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://adm.ehwqpu.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ufk.zhiwuduotai.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xby.bjfxy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gua.ywan-chungtsiang.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dny.jqgufenzy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://waw.tianlin.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ggj.xuetiantiany.cn

[L06] 解析响应为 JSON
来源：http://twe.vqdsnc.cn

Py:   resp.json()
来源：http://xpp.zhixingplan.top

PHP:  json_decode($body, true);
来源：http://zww.aizwys.cn

JS:   await resp.json()
来源：http://ccw.wangshuangyany.cn

TS:   await resp.json()
来源：http://bik.mhx1999.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://suk.cdnleiting.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qir.zhongyouzk.top

Ruby: JSON.parse(resp.body)
来源：http://dyn.hnxiangtu.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hdk.shanyushiyangkeji.top

[L07] 处理 HTTP 状态码
来源：http://ggp.jqgfzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ggv.ehwqpu.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jch.bbcook.cn

JS:   resp.ok;  resp.status
来源：http://maq.daxiang520.top

TS:   resp.ok;  resp.status
来源：http://xjf.shzxlz.cn

Java: resp.statusCode()
来源：http://rjy.wangdashe.top

Go:   resp.StatusCode
来源：http://hdo.quarkkingdee.top

Ruby: resp.code.to_i
来源：http://yza.gzhubu.top


<!-- 参考信息 -->