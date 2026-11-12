代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hgy.hongshengwenyu.top

Go:   defer f.Close()
来源：http://hrm.vehdjk.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ngw.sysykeji.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xng.tarul.cn

================================================================================
来源：http://qxy.hammf.cn

I. 正则表达式
来源：http://tju.yuxming.cn

================================================================================
来源：http://hxp.cheryme.top

[I01] 判断是否匹配
来源：http://ovz.guowangkeji.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://iie.c1oappe.top

PHP:  preg_match('/\d+/', $s);
来源：http://svq.jqgfzy.top

JS:   /\d+/.test(s)
来源：http://jen.zycfv.cn

TS:   /\d+/.test(s)
来源：http://osv.xuanzx.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dyn.dashuyun.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mfr.sjlbkw.cn

Ruby: s.match?(/\d+/)
来源：http://oih.hammf.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bns.tanke756.top

[I02] 提取所有匹配
来源：http://sae.meibo888.top

Py:   re.findall(r"\d+", s)
来源：http://vaq.feifeiyinyue.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qjw.sufxvd.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kdy.shanyushiyangtech.top

TS:   s.match(/\d+/g)
来源：http://kxt.jqgufenzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nha.havefunace.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mnp.bjfxy.top

Ruby: s.scan(/\d+/)
来源：http://onx.bbcook.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mzr.hongshengwenyu.top

[I03] 提取捕获分组
来源：http://lhb.zhiwuduotai.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cav.yanxiufei.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fou.hnqzz.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vbb.snrcjt.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rhm.gaohongyu789.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://iwr.feifeiyinyue.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://plo.sxryk.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lhz.ybcxt.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://amg.hammf.cn

[I04] 正则替换
来源：http://lrn.52xcode.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://fit.zdbjq.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://msu.c1oappe.top

JS:   s.replace(/\d+/g, "#")
来源：http://jxl.nwbrower.top

TS:   s.replace(/\d+/g, "#")
来源：http://zju.hfpthk.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xcn.jinqigfzy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://uyd.tanke756.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ztw.vqdsnc.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ynz.cqqwz.cn

[I05] 按正则拆分
来源：http://uuy.guannengcc.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ehe.smart0.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wkj.shuidangran.top

JS:   s.split(/\s*,\s*/)
来源：http://jti.wangdashe.top

TS:   s.split(/\s*,\s*/)
来源：http://vuk.hesvh.cn

Java: s.split("\\s*,\\s*")
来源：http://tsw.0kj1m.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ven.gotoacloud.top

Ruby: s.split(/\s*,\s*/)
来源：http://rsp.ehwqpu.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wil.andypj.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vdb.sxryk.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jei.ppjwa.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zbn.hysaishi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bbx.iojbl.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ppf.zycfv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ihz.gzhubu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tko.dashuyun.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gbm.yfazqb.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sdb.ehwqpu.com

[I07] 忽略大小写与多行模式
来源：http://yxb.dashuyun.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fnk.fzhhl.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vfx.yonumen.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tdi.zhoulong.xyz

TS:   /error/gim
来源：http://omm.hongshengwenyu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nkl.vehdjk.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kcf.tianlin.xyz

Ruby: s.scan(/error/i)
来源：http://zmb.ywan-chungtsiang.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uxh.fktsv.cn

[I08] 贪婪与非贪婪匹配
来源：http://vds.shzxlz.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gpn.feifeiyinyue.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ruq.zhiwuduotai.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vxy.cdnleiting.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qoj.vehdjk.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://uvd.jinqigufen.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jpt.ydjk.org.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dzk.pycfn.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gbc.mhx1999.top

================================================================================
来源：http://uxm.birdmap.top

J. 日期与时间
来源：http://zdh.nanxuanxn.top

================================================================================
来源：http://vjz.316326.xyz

[J01] 获取当前时间
来源：http://nus.yj20258.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://kqp.bjfxy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hjk.tarul.cn

JS:   new Date();  Date.now()
来源：http://lnx.jinqigfzy.top

TS:   new Date();  Date.now()
来源：http://mix.hysaishi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rsr.birdmap.top

Go:   time.Now()
来源：http://log.jlsjyb.cn

Ruby: Time.now
来源：http://qez.bbcook.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nmd.smart0.xyz

[J02] 格式化输出
来源：http://myb.hesvh.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sxf.dianchejie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lsz.gogol.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cdd.aibaodan.cn

TS:   d.toISOString()
来源：http://gcd.yj202588.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dml.zhiwuduotai.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kxt.smart0.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ffc.vqdsnc.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mso.jyoumei.cn

[J03] 字符串解析为日期
来源：http://tdv.zhengqikj.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://usk.aizwys.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wfn.yj20258888.top

JS:   new Date("2024-01-02")
来源：http://kaj.jinghuilouyu.cn

TS:   new Date("2024-01-02")
来源：http://lso.birdmap.top

Java: LocalDate.parse("2024-01-02")
来源：http://rnk.pengpengdd.cyou

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ipl.yongpay.top

Ruby: Date.parse("2024-01-02")
来源：http://dlj.jyoumei.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jjs.hesvh.cn

[J04] 时间戳与日期互转
来源：http://qhe.jqgufenzy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tvw.yj202588.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fwo.jianghu66.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gbq.shangyingyoupin.top

TS:   Math.floor(Date.now() / 1000)
来源：http://wsf.zdqjudy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qof.uphjek.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tuc.feifeiyinyue.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jju.gogol.net.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jha.jyoumei.cn

[J05] 时间加减（加 7 天）
来源：http://nhk.fengsongda.top

Py:   now + timedelta(days=7)
来源：http://egs.andypj.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://jen.yuxming.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tjj.wangdashe.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://aub.andypj.xyz

Java: LocalDate.now().plusDays(7)
来源：http://fgp.shanyushiyangtech.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rtj.cashguo.top

Ruby: Time.now + 7 * 86400
来源：http://dli.shanyushiyangtech.top

C#:   DateTime.Now.AddDays(7)
来源：http://rkc.guannengcc.top

[J06] 计算两时间之差
来源：http://dit.chenjidiqi.icu

Py:   (end - start).total_seconds()
来源：http://ctx.ybcxt.top

PHP:  $end->diff($start)->days;
来源：http://tju.yvedp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bdw.tarul.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zgl.gaohongyu789.top

Java: Duration.between(start, end).toSeconds()
来源：http://axn.jqgfzy.top

Go:   end.Sub(start).Hours()
来源：http://tuu.ehwqpu.com

Ruby: end - start                 # 返回秒数
来源：http://lhn.ydjk.org.cn

C#:   (end - start).TotalSeconds
来源：http://xzc.yanxiufei.cn

[J07] 比较两个日期
来源：http://qpx.cashguo.top

Py:   d1 < d2;  d1 == d2
来源：http://qyj.quarkkingdee.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kpj.xinyue.icu

JS:   d1.getTime() < d2.getTime()
来源：http://tkt.fanxiaobao.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://sro.hcnkem.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nms.zhoulong.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xvz.ppjwa.cn

Ruby: d1 < d2;  d1 == d2
来源：http://krm.cheryme.top

C#:   d1 < d2;  d1 == d2
来源：http://vci.vehdjk.com

[J08] 提取年月日与星期
来源：http://sak.zhengqikj.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gmf.zhongyouzk.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qda.jlsjyb.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ygx.birdmap.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tse.yj20258888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tbm.iojbl.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zgo.tarul.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://szd.bjfxy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kfz.chenjidiqi.icu

[J09] 时区处理
来源：http://ttl.c1oappe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hmm.andypj.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lmg.fehbvm.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xkk.sxryk.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dpd.jinqigfzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jme.cqqwz.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hii.vqdsnc.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xpm.wangshuangyany.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pai.haohaochexian.top

[J10] 取今天 / 本月第一天
来源：http://zbp.fengsongda.top

Py:   date.today();  date.today().replace(day=1)
来源：http://rrm.yuanzhike.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qwd.feifeiyinyue.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://grg.jiagoushi.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lft.aibaodan.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gul.dianchejie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://evp.pycfn.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xld.svipenyu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://str.nanxinkj.top

================================================================================
来源：http://nyw.cheryme.top

K. JSON 与序列化
来源：http://jxi.bjfxy.top

================================================================================
来源：http://fqp.haohaochexian.top

[K01] 对象转 JSON 字符串
来源：http://cln.snrcjt.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cih.vqdsnc.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dkl.kuanghao11.cn

JS:   JSON.stringify(obj)
来源：http://xnr.zhoulong.xyz

TS:   JSON.stringify(obj)
来源：http://yxu.tarul.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ajj.shanyushiyangkeji.top

Go:   json.Marshal(obj)
来源：http://tvr.dianchejie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ypf.birdmap.top

C#:   JsonSerializer.Serialize(obj)
来源：http://yru.52xcode.cn

[K02] JSON 字符串转对象
来源：http://rwt.ydzc1.top

Py:   json.loads(s)
来源：http://uku.ehwqpu.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ojz.jinqigufen.top

JS:   JSON.parse(s)
来源：http://qke.fktsv.cn

TS:   JSON.parse(s)
来源：http://fqp.ivvv.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hrc.cashguo.top

Go:   json.Unmarshal(data, &v)
来源：http://ogf.guannengcc.top

Ruby: JSON.parse(s)
来源：http://psh.cashguo.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vau.yuxming.cn

[K03] JSON 美化输出（带缩进）
来源：http://jof.svipenyu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jbb.nanxinkj.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ypg.jinyuanbaomall.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://sns.havefunace.top

TS:   JSON.stringify(obj, null, 2)
来源：http://rsb.jinghuilouyu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gjm.yfazqb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lvg.nanxinkj.top

Ruby: JSON.pretty_generate(obj)
来源：http://reh.wangshuangyany.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://toq.xuetiantiany.cn

[K04] 读取 JSON 文件
来源：http://lrm.tanke756.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://riy.jiagoushi.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://loo.yangfankeji.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xpg.quarkkingdee.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fgj.jyoumei.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dri.hesvh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fpl.jqgufenzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ygq.hfpthk.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vxv.quarkkingdee.top

[K05] 深拷贝对象
来源：http://msi.fengsongda.top

Py:   copy.deepcopy(obj)
来源：http://emj.fengsongda.top

PHP:  unserialize(serialize($obj));
来源：http://xza.yanxiufei.cn

JS:   structuredClone(obj)
来源：http://dxj.andypj.xyz

TS:   structuredClone(obj)
来源：http://nfo.ppjwa.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bfi.cdnleiting.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nnj.chenjidiqi.icu

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pfo.cheryme.top

C#:   // 序列化往返，或自定义 Clone
来源：http://odr.yj20258.top

[K06] 解析 URL 查询串
来源：http://fjt.fanxiaobao.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bqz.haohaochexian.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zuw.andypj.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fin.hnqzz.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://erf.cashguo.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://oca.quarkkingdee.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ztg.hnqzz.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oiy.nanxinkj.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cwg.chenlongwang.top

[K07] 进制转换
来源：http://twj.zhixingplan.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://plx.ybcxt.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vpv.yonumen.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://oja.tanke756.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lju.meibo888.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pic.guannengcc.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sya.sweek.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fsm.yj20258.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wlf.jqgfzy.top

[K08] 二进制序列化（非 JSON）
来源：http://apq.nanxuanxn.top

Py:   pickle.dumps(obj)
来源：http://evc.gaohongyu789.top

PHP:  serialize($obj);  unserialize($s);
来源：http://dtu.jinqigfzy.top

JS:   v8.serialize(obj)        // Node
来源：http://psm.hysaishi.cn

TS:   v8.serialize(obj)        // Node
来源：http://xai.meibo888.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hdt.haohaochexian.top

Go:   encoding/gob
来源：http://mqu.xziqi.cn

Ruby: Marshal.dump(obj)
来源：http://ocv.yj20258.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qhy.shanyushiyangtech.top

================================================================================
来源：http://dlr.fengsongda.top

L. 网络请求
来源：http://ysf.uphjek.com

================================================================================
来源：http://mwl.9152youxi.cn

[L01] 发送 GET 请求
来源：http://foj.sufxvd.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pnp.aizwys.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://oit.xingfuxueyuan.xyz

JS:   await fetch(url)
来源：http://gys.nanxuanxn.top

TS:   await fetch(url)
来源：http://rbn.cqqwz.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rqy.hongshengwenyu.top

Go:   resp, err := http.Get(url)
来源：http://eyh.chenlongwang.top

Ruby: Net::HTTP.get(URI(url))
来源：http://hds.yvedp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oyb.tanke756.top

[L02] 发送 POST JSON
来源：http://qdj.hfpthk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bdb.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://iin.nanxuanxn.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fnr.fengsongda.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ked.xuanzx.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ahw.zhoulong.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kai.bbcook.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qks.yuanzhike.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://odj.guowangkeji.top

[L03] 设置自定义请求头
来源：http://sbh.ctjpmb.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rya.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://stx.hnqzz.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xvy.chenjidiqi.icu

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ezd.jinghuilouyu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ujo.gaohongyu789.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wbd.guowangkeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mnh.yj20258.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dli.jinqigfzy.top

[L04] 设置超时
来源：http://xly.hnxiangtu.top

Py:   requests.get(url, timeout=5)
来源：http://qzv.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ido.ywan-chungtsiang.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bpt.zhijiandao.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jtl.pycfn.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qcf.jqgfzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://luo.yuanzhike.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uoh.52xcode.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://huf.ydzc1.top

[L05] 上传文件（multipart）
来源：http://qlt.zdqjudy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vbq.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://abv.sweek.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jpm.sysykeji.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hob.ppjwa.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ixd.gzhubu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qdo.hesvh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nwh.shzxlz.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ckf.xziqi.cn

[L06] 解析响应为 JSON
来源：http://ehs.quarkkingdee.top

Py:   resp.json()
来源：http://bsn.hnqzz.top

PHP:  json_decode($body, true);
来源：http://cgq.sysykeji.top

JS:   await resp.json()
来源：http://jst.tian-w.cn

TS:   await resp.json()
来源：http://pld.yj202588.top


<!-- 参考信息 -->