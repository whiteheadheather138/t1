代发 wailian999

================================================================================
来源：http://vqr.epnwcf.com

I. 正则表达式
来源：http://qqb.shanyushiyangkeji.top

================================================================================
来源：http://jtw.redwolf501.top

[I01] 判断是否匹配
来源：http://xxe.jyoumei.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://guj.hammf.cn

PHP:  preg_match('/\d+/', $s);
来源：http://uxf.nanxuanxn.top

JS:   /\d+/.test(s)
来源：http://lku.daria6918.cn

TS:   /\d+/.test(s)
来源：http://btd.daxiang520.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ibp.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ryp.52xcode.cn

Ruby: s.match?(/\d+/)
来源：http://rkt.gogol.net.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://eol.ehwqpu.com

[I02] 提取所有匹配
来源：http://kcc.zhijiandao.cn

Py:   re.findall(r"\d+", s)
来源：http://vxu.yvedp.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rzc.tianlin.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ulr.hesvh.cn

TS:   s.match(/\d+/g)
来源：http://ber.xingfuxueyuan.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fmq.zhongyouzk.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pvr.tanke756.top

Ruby: s.scan(/\d+/)
来源：http://ksf.ehwqpu.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cby.ivvv.top

[I03] 提取捕获分组
来源：http://spe.fanxiaobao.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://asu.jinqigufen.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ljm.fzhhl.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tvr.yongpay.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://eut.pycfn.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ngz.uphjek.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://etm.yonumen.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://krk.sjlbkw.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vzp.zhoulong.xyz

[I04] 正则替换
来源：http://owx.chenlongwang.top

Py:   re.sub(r"\d+", "#", s)
来源：http://etw.kuanghao11.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nll.9152youxi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ant.yuxming.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qib.jqgufenzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://xvv.zdbjq.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://obn.ctjpmb.com

Ruby: s.gsub(/\d+/, "#")
来源：http://eta.daria6918.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uje.ywan-chungtsiang.top

[I05] 按正则拆分
来源：http://dza.vehdjk.com

Py:   re.split(r"\s*,\s*", s)
来源：http://qul.cucudq.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://scl.tarul.cn

JS:   s.split(/\s*,\s*/)
来源：http://job.yj202588.top

TS:   s.split(/\s*,\s*/)
来源：http://uri.iojbl.cn

Java: s.split("\\s*,\\s*")
来源：http://wtc.yuanzhike.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dwm.9152youxi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mxg.cheryme.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://doo.wangdashe.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ppu.snrcjt.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nno.yanxiufei.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rux.iojbl.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://czw.guannengcc.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://odb.quarkkingdee.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yta.xingfuxueyuan.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://owi.gogol.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kjh.guannengcc.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lim.yanxiufei.cn

[I07] 忽略大小写与多行模式
来源：http://hnd.cdnleiting.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://czo.jqgfzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wug.zhixingplan.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qwv.tian-w.cn

TS:   /error/gim
来源：http://fak.zhengqikj.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://sxo.fanxiaobao.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ijy.ctjpmb.com

Ruby: s.scan(/error/i)
来源：http://wqu.feifeiyinyue.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wdu.hnqzz.top

[I08] 贪婪与非贪婪匹配
来源：http://rbz.hammf.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://skr.pengpengdd.cyou

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nlc.zdbjq.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qeu.zhijiandao.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uxv.jiagoushi.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://cih.jiagoushi.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xud.tianlin.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vpw.hnxiangtu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ptm.316326.xyz

================================================================================
来源：http://ayg.jyoumei.cn

J. 日期与时间
来源：http://rnm.daxiang520.top

================================================================================
来源：http://dzm.hnxiangtu.top

[J01] 获取当前时间
来源：http://etj.ybcxt.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://gci.zhijiandao.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://oyx.ybcxt.top

JS:   new Date();  Date.now()
来源：http://ozm.jyoumei.cn

TS:   new Date();  Date.now()
来源：http://fmn.mhx1999.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ckf.shzxlz.cn

Go:   time.Now()
来源：http://lip.cheryme.top

Ruby: Time.now
来源：http://yss.yj20258.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jhn.cheryme.top

[J02] 格式化输出
来源：http://far.smart0.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ppv.yj202588.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yka.haohaochexian.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cnc.hesvh.cn

TS:   d.toISOString()
来源：http://ciz.yuxming.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ekl.hnxiangtu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qni.jqgfzy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qjc.yfazqb.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://evk.pengpengdd.cyou

[J03] 字符串解析为日期
来源：http://alp.sweek.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gxc.ppjwa.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ljr.chenlongwang.top

JS:   new Date("2024-01-02")
来源：http://wub.jinqigfzy.top

TS:   new Date("2024-01-02")
来源：http://rdd.xinyue.icu

Java: LocalDate.parse("2024-01-02")
来源：http://zww.sysykeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tbt.ybcxt.top

Ruby: Date.parse("2024-01-02")
来源：http://qxw.xziqi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ggj.jyoumei.cn

[J04] 时间戳与日期互转
来源：http://llv.smart0.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zvn.tanke756.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cvn.shuidangran.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cnu.chenlongwang.top

TS:   Math.floor(Date.now() / 1000)
来源：http://vfu.hammf.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://eoz.sjlbkw.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lup.wangshuangyany.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lba.yj202588.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kbs.xinyue.icu

[J05] 时间加减（加 7 天）
来源：http://qgy.chenzaomai.com

Py:   now + timedelta(days=7)
来源：http://nxn.vqdsnc.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wpk.cashguo.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://psc.yj20258.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://asx.c1oappe.top

Java: LocalDate.now().plusDays(7)
来源：http://sux.fzhhl.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ehk.mhx1999.top

Ruby: Time.now + 7 * 86400
来源：http://ulq.daxiang520.top

C#:   DateTime.Now.AddDays(7)
来源：http://ymd.jyoumei.cn

[J06] 计算两时间之差
来源：http://uvy.hysaishi.cn

Py:   (end - start).total_seconds()
来源：http://fiy.gogol.net.cn

PHP:  $end->diff($start)->days;
来源：http://nur.birdmap.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xqz.vqdsnc.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ybw.havefunace.top

Java: Duration.between(start, end).toSeconds()
来源：http://ukt.vehdjk.com

Go:   end.Sub(start).Hours()
来源：http://gvu.zhixingplan.top

Ruby: end - start                 # 返回秒数
来源：http://ett.nanxuanxn.top

C#:   (end - start).TotalSeconds
来源：http://jeo.xuanzx.com

[J07] 比较两个日期
来源：http://rtb.jinghuilouyu.cn

Py:   d1 < d2;  d1 == d2
来源：http://vgt.cucudq.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xby.jinqigufen.top

JS:   d1.getTime() < d2.getTime()
来源：http://stn.hnxiangtu.top

TS:   d1.getTime() < d2.getTime()
来源：http://ywq.dianchejie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ghf.ybcxt.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pjz.ybcxt.top

Ruby: d1 < d2;  d1 == d2
来源：http://joz.ivvv.top

C#:   d1 < d2;  d1 == d2
来源：http://zli.iojbl.cn

[J08] 提取年月日与星期
来源：http://jzk.kuanghao11.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kgn.yfazqb.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ydy.c1oappe.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gpk.zhongyouzk.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tgv.haohaochexian.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yfm.tanke756.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://euw.yonumen.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://iqn.sufxvd.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nho.yanxiufei.cn

[J09] 时区处理
来源：http://poq.yueranfly.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gpf.xinyue.icu

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bxy.yj202588.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sho.yanxiufei.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://msi.tianlin.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ucl.quarkkingdee.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jyg.vehdjk.com

Ruby: Time.now.getlocal("+08:00")
来源：http://wij.sweek.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dcx.daxiang520.top

[J10] 取今天 / 本月第一天
来源：http://tyh.wangdashe.top

Py:   date.today();  date.today().replace(day=1)
来源：http://iyc.yangfankeji.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jho.smart0.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tnq.xingfuxueyuan.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ecy.vehdjk.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nyv.mhx1999.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mgs.daria6918.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ivv.aizwys.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rdh.nanxuanxn.top

================================================================================
来源：http://npd.shzxlz.cn

K. JSON 与序列化
来源：http://enb.zhixingplan.top

================================================================================
来源：http://twx.pengpengdd.cyou

[K01] 对象转 JSON 字符串
来源：http://yhj.daxiang520.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mbl.feifeiyinyue.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lmy.ydzc1.top

JS:   JSON.stringify(obj)
来源：http://xmb.quarkkingdee.top

TS:   JSON.stringify(obj)
来源：http://qyh.xuetiantiany.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vmx.xuanzx.com

Go:   json.Marshal(obj)
来源：http://rrq.nwbrower.top

Ruby: obj.to_json                                     // require "json"
来源：http://vig.jiagoushi.top

C#:   JsonSerializer.Serialize(obj)
来源：http://mlv.gaohongyu789.top

[K02] JSON 字符串转对象
来源：http://puh.ehwqpu.com

Py:   json.loads(s)
来源：http://ktf.vehdjk.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dyk.vehdjk.com

JS:   JSON.parse(s)
来源：http://wex.fzhhl.top

TS:   JSON.parse(s)
来源：http://rlh.yj20258888.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blr.0kj1m.cn

Go:   json.Unmarshal(data, &v)
来源：http://bsl.zdbjq.cn

Ruby: JSON.parse(s)
来源：http://cio.cashguo.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ncm.zhiwuduotai.top

[K03] JSON 美化输出（带缩进）
来源：http://cll.zdqjudy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dcl.ehwqpu.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lll.zhixingplan.top

JS:   JSON.stringify(obj, null, 2)
来源：http://vhi.yuxming.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wuz.nanxinkj.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jns.aizwys.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hle.ywan-chungtsiang.top

Ruby: JSON.pretty_generate(obj)
来源：http://hxe.hcnkem.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ffz.chenlongwang.top

[K04] 读取 JSON 文件
来源：http://uum.shuidangran.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fmc.wangshuangyany.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://olw.iojbl.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hhx.yuanzhike.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oqt.redwolf501.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lfq.tian-w.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tuq.gogol.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pdz.snrcjt.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fjy.tianlin.xyz

[K05] 深拷贝对象
来源：http://efo.daxiang520.top

Py:   copy.deepcopy(obj)
来源：http://hyn.zdqjudy.top

PHP:  unserialize(serialize($obj));
来源：http://jib.chenlongwang.top

JS:   structuredClone(obj)
来源：http://ore.iojbl.cn

TS:   structuredClone(obj)
来源：http://cro.xuetiantiany.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vna.zycfv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rtm.yj20258888.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lek.tian-w.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://nby.jqgufenzy.top

[K06] 解析 URL 查询串
来源：http://mpw.fzhhl.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oor.xuetiantiany.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ukf.haohaochexian.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qdk.jqgufenzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://heu.ehwqpu.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qza.wangshuangyany.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://inz.xuetiantiany.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cux.ppjwa.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://snn.fanxiaobao.xyz

[K07] 进制转换
来源：http://qtv.nanxuanxn.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tmj.jianghu66.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fbd.aibaodan.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kdl.tanke756.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://otb.chenzaomai.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ymv.iojbl.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sbg.nwbrower.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pot.yanxiufei.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qkm.zdqjudy.top

[K08] 二进制序列化（非 JSON）
来源：http://adg.aibaodan.cn

Py:   pickle.dumps(obj)
来源：http://udg.jyoumei.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fbj.0kj1m.cn

JS:   v8.serialize(obj)        // Node
来源：http://ffv.shzxlz.cn

TS:   v8.serialize(obj)        // Node
来源：http://xvh.c1oappe.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sec.chenlongwang.top

Go:   encoding/gob
来源：http://ics.ywan-chungtsiang.top

Ruby: Marshal.dump(obj)
来源：http://jcj.yonumen.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pts.sjlbkw.cn

================================================================================
来源：http://upd.xuanzx.com

L. 网络请求
来源：http://sqk.yuxming.cn

================================================================================
来源：http://ehr.guowangkeji.top

[L01] 发送 GET 请求
来源：http://mxq.feifeiyinyue.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ctt.yonumen.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xgo.yj20258.top

JS:   await fetch(url)
来源：http://lbu.kuanghao11.cn

TS:   await fetch(url)
来源：http://ive.hammf.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zqc.dianchejie.cn

Go:   resp, err := http.Get(url)
来源：http://jly.zhaomingkeji.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://ljy.cdnleiting.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uwp.fktsv.cn

[L02] 发送 POST JSON
来源：http://hmy.nwbrower.top

Py:   requests.post(url, json={"a": 1})
来源：http://rkg.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ffh.ppjwa.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vkv.jqgufenzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zej.yuxming.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yuj.jqgufenzy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://koj.jinqigfzy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ajw.chenzaomai.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ixw.zhaomingkeji.xyz

[L03] 设置自定义请求头
来源：http://bfu.chenzaomai.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rmr.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qtb.cdnleiting.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sie.ywan-chungtsiang.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uik.xziqi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xqa.jyoumei.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://isj.yuanzhike.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xus.xuanzx.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vka.xuanzx.com

[L04] 设置超时
来源：http://qur.haohaochexian.top

Py:   requests.get(url, timeout=5)
来源：http://anv.9152youxi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ygf.shangyingyoupin.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bpv.hammf.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qzo.fehbvm.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cpw.ydjk.org.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jbs.hnxiangtu.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jve.zhijiandao.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tlm.yuanzhike.top

[L05] 上传文件（multipart）
来源：http://wkf.nwbrower.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bcy.shzxlz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pvy.tian-w.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lxs.shzxlz.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yap.cucudq.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yed.guannengcc.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://omc.xziqi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nbn.vehdjk.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vtt.zhiwuduotai.top

[L06] 解析响应为 JSON
来源：http://ooi.hammf.cn

Py:   resp.json()
来源：http://qjy.jiagoushi.top

PHP:  json_decode($body, true);
来源：http://pyn.vehdjk.com

JS:   await resp.json()
来源：http://hur.shanyushiyangkeji.top

TS:   await resp.json()
来源：http://tnu.nanxuanxn.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zth.quarkkingdee.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://aiu.jianghu66.top

Ruby: JSON.parse(resp.body)
来源：http://iwv.redwolf501.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pjj.hywenlv.cn


<!-- 参考信息 -->