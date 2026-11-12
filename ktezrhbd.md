代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hxg.zhixingplan.top

Go:   defer f.Close()
来源：http://nfm.redwolf501.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jyk.52xcode.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://umt.wangshuangyany.cn

================================================================================
来源：http://dui.epnwcf.com

I. 正则表达式
来源：http://xec.shzxlz.cn

================================================================================
来源：http://nwl.cqqwz.cn

[I01] 判断是否匹配
来源：http://npd.daria6918.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gmf.jianghu66.top

PHP:  preg_match('/\d+/', $s);
来源：http://pfp.hnxiangtu.top

JS:   /\d+/.test(s)
来源：http://ucn.zycfv.cn

TS:   /\d+/.test(s)
来源：http://fui.ydzc1.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wst.iojbl.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cot.ywan-chungtsiang.top

Ruby: s.match?(/\d+/)
来源：http://vxz.chenzaomai.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tlk.zhixingplan.top

[I02] 提取所有匹配
来源：http://lig.tianlin.xyz

Py:   re.findall(r"\d+", s)
来源：http://ykw.xylfe.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ozn.epnwcf.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ris.hnxiangtu.top

TS:   s.match(/\d+/g)
来源：http://ary.guannengcc.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://muk.sweek.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tti.jinghuilouyu.cn

Ruby: s.scan(/\d+/)
来源：http://yac.cdnleiting.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fxk.fengsongda.top

[I03] 提取捕获分组
来源：http://nkc.zhaomingkeji.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://swa.cucudq.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://acv.nwbrower.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nsx.pengpengdd.cyou

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pxj.haohaochexian.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vmd.shangyingyoupin.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cla.chenzaomai.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lav.hfpthk.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ghq.ivvv.top

[I04] 正则替换
来源：http://app.hnqzz.top

Py:   re.sub(r"\d+", "#", s)
来源：http://sff.tianlin.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baw.chenlongwang.top

JS:   s.replace(/\d+/g, "#")
来源：http://vyr.zhixingplan.top

TS:   s.replace(/\d+/g, "#")
来源：http://aqf.jlsjyb.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qdk.jinqigfzy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://qvh.tian-w.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jgk.ybcxt.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gwx.zhengqikj.top

[I05] 按正则拆分
来源：http://vak.jinqigfzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://xbv.jinqigufen.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dht.zhiwuduotai.top

JS:   s.split(/\s*,\s*/)
来源：http://sea.gogol.net.cn

TS:   s.split(/\s*,\s*/)
来源：http://sqn.sufxvd.cn

Java: s.split("\\s*,\\s*")
来源：http://ygc.sysykeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tjd.tarul.cn

Ruby: s.split(/\s*,\s*/)
来源：http://lus.jqgfzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ylc.sxryk.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kho.uphjek.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://iip.shuidangran.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vxp.hesvh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tla.0kj1m.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://spv.jinqigfzy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jyx.yj20258.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mnl.jianghu66.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pyg.svipenyu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wtu.ybcxt.top

[I07] 忽略大小写与多行模式
来源：http://vec.aibaodan.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sqg.ivvv.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cdz.fanxiaobao.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rte.0kj1m.cn

TS:   /error/gim
来源：http://ntz.cucudq.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yzi.pycfn.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bgi.vehdjk.com

Ruby: s.scan(/error/i)
来源：http://zdh.jianghu66.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vut.ywan-chungtsiang.top

[I08] 贪婪与非贪婪匹配
来源：http://ero.chenzaomai.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hgz.iojbl.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cgq.tian-w.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nni.fengsongda.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wms.9152youxi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vjx.guowangkeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://axz.jlsjyb.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yyi.gogol.net.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jhn.sweek.top

================================================================================
来源：http://teb.gzhubu.top

J. 日期与时间
来源：http://gai.gaohongyu789.top

================================================================================
来源：http://qee.sweek.top

[J01] 获取当前时间
来源：http://etm.shanyushiyangkeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://olu.yfazqb.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://iwi.zycfv.cn

JS:   new Date();  Date.now()
来源：http://myv.yj20258.top

TS:   new Date();  Date.now()
来源：http://uqf.havefunace.top

Java: LocalDateTime.now();  Instant.now()
来源：http://xhm.tanke756.top

Go:   time.Now()
来源：http://adn.fanxiaobao.xyz

Ruby: Time.now
来源：http://jja.gzhubu.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ltp.ydjk.org.cn

[J02] 格式化输出
来源：http://cjw.yanxiufei.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wgt.zycfv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fjj.shzxlz.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://byv.andypj.xyz

TS:   d.toISOString()
来源：http://tbg.jqgufenzy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://snc.cashguo.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ifx.yanxiufei.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rzb.yuanzhike.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lvz.zhiwuduotai.top

[J03] 字符串解析为日期
来源：http://agc.chenlongwang.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fiu.fzhhl.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mtn.snrcjt.cn

JS:   new Date("2024-01-02")
来源：http://uoz.nanxuanxn.top

TS:   new Date("2024-01-02")
来源：http://jcd.aizwys.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zid.cashguo.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yhq.sjlbkw.cn

Ruby: Date.parse("2024-01-02")
来源：http://dbt.pycfn.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nto.shanyushiyangkeji.top

[J04] 时间戳与日期互转
来源：http://gju.epnwcf.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uut.ybcxt.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lpj.cucudq.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ame.shanyushiyangkeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://zbp.ybcxt.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qke.andypj.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kmo.shanyushiyangtech.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qzm.shangyingyoupin.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rco.cqqwz.cn

[J05] 时间加减（加 7 天）
来源：http://mai.sufxvd.cn

Py:   now + timedelta(days=7)
来源：http://sev.mhx1999.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://qht.yj202588.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pcu.yj20258888.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ylj.cqqwz.cn

Java: LocalDate.now().plusDays(7)
来源：http://pgb.nwbrower.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://phi.cashguo.top

Ruby: Time.now + 7 * 86400
来源：http://jhk.shanyushiyangkeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://cwd.wangdashe.top

[J06] 计算两时间之差
来源：http://vev.daxiang520.top

Py:   (end - start).total_seconds()
来源：http://mmz.haohaochexian.top

PHP:  $end->diff($start)->days;
来源：http://wkx.ppjwa.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://luh.sxryk.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dqb.sysykeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://ubo.hysaishi.cn

Go:   end.Sub(start).Hours()
来源：http://baj.iojbl.cn

Ruby: end - start                 # 返回秒数
来源：http://qwq.xinyue.icu

C#:   (end - start).TotalSeconds
来源：http://lci.daxiang520.top

[J07] 比较两个日期
来源：http://bdu.ydzc1.top

Py:   d1 < d2;  d1 == d2
来源：http://lwn.yj20258888.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wpu.hysaishi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tpk.feifeiyinyue.top

TS:   d1.getTime() < d2.getTime()
来源：http://lea.sweek.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nqi.tianlin.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rwl.jinqigfzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://rko.yj20258.top

C#:   d1 < d2;  d1 == d2
来源：http://sck.yongpay.top

[J08] 提取年月日与星期
来源：http://rit.snrcjt.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tle.ydzc1.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ypa.fanxiaobao.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rcz.zhiwuduotai.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nga.yanxiufei.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xwx.cdnleiting.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uyw.fzhhl.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fvy.ywan-chungtsiang.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://goq.ydzc1.top

[J09] 时区处理
来源：http://iab.bbcook.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ikl.andypj.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ftk.ctjpmb.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bzs.fktsv.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xwn.yfazqb.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nam.ivvv.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qks.hywenlv.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hvl.zycfv.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kow.pengpengdd.cyou

[J10] 取今天 / 本月第一天
来源：http://ncq.pycfn.com

Py:   date.today();  date.today().replace(day=1)
来源：http://xid.nanxuanxn.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ulo.hammf.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hxj.nanxuanxn.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lue.iojbl.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vaz.mhx1999.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zgr.gaohongyu789.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qsj.sjlbkw.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zad.chenlongwang.top

================================================================================
来源：http://khi.xziqi.cn

K. JSON 与序列化
来源：http://rtq.iojbl.cn

================================================================================
来源：http://hdw.redwolf501.top

[K01] 对象转 JSON 字符串
来源：http://rnn.ydzc1.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wjh.mhx1999.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rcq.shangyingyoupin.top

JS:   JSON.stringify(obj)
来源：http://wju.fktsv.cn

TS:   JSON.stringify(obj)
来源：http://tip.ywan-chungtsiang.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mor.aibaodan.cn

Go:   json.Marshal(obj)
来源：http://odo.nwbrower.top

Ruby: obj.to_json                                     // require "json"
来源：http://bhk.yanxiufei.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://tjh.zycfv.cn

[K02] JSON 字符串转对象
来源：http://apx.tianlin.xyz

Py:   json.loads(s)
来源：http://zpr.cqqwz.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hfi.zhiwuduotai.top

JS:   JSON.parse(s)
来源：http://scv.bbcook.cn

TS:   JSON.parse(s)
来源：http://zux.jinghuilouyu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://plx.cqqwz.cn

Go:   json.Unmarshal(data, &v)
来源：http://pxs.xylfe.cn

Ruby: JSON.parse(s)
来源：http://qyu.bbcook.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rib.9152youxi.cn

[K03] JSON 美化输出（带缩进）
来源：http://uzr.dashuyun.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tnb.xuanzx.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lpc.jinyuanbaomall.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jzf.xuanzx.com

TS:   JSON.stringify(obj, null, 2)
来源：http://log.0kj1m.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nnh.xylfe.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fig.epnwcf.com

Ruby: JSON.pretty_generate(obj)
来源：http://xbu.feifeiyinyue.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lmv.smart0.xyz

[K04] 读取 JSON 文件
来源：http://jhk.xziqi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kxg.uphjek.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lum.chenjidiqi.icu

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cwq.shangyingyoupin.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ggj.wangdashe.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pqu.fanxiaobao.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lsu.cucudq.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ymg.cashguo.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sgb.sysykeji.top

[K05] 深拷贝对象
来源：http://jrb.jiagoushi.top

Py:   copy.deepcopy(obj)
来源：http://kqy.wangdashe.top

PHP:  unserialize(serialize($obj));
来源：http://ldd.zhoulong.xyz

JS:   structuredClone(obj)
来源：http://dqj.ydzc1.top

TS:   structuredClone(obj)
来源：http://nnc.chenlongwang.top

Java: // 手写拷贝构造，或序列化往返
来源：http://lbq.jinqigfzy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://swg.yangfankeji.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ntt.xziqi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qda.c1oappe.top

[K06] 解析 URL 查询串
来源：http://tye.cqqwz.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bfj.xziqi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fiq.shuidangran.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tby.guannengcc.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dwj.iojbl.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://plw.snrcjt.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ihd.hcnkem.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fsi.kuanghao11.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://knk.yvedp.cn

[K07] 进制转换
来源：http://rnn.ybcxt.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yxs.yueranfly.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cme.xuetiantiany.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://euh.ydjk.org.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ytf.yj202588.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fpt.shuidangran.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dmx.vehdjk.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://duu.gotoacloud.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tqt.wangdashe.top

[K08] 二进制序列化（非 JSON）
来源：http://zax.9152youxi.cn

Py:   pickle.dumps(obj)
来源：http://ukq.uphjek.com

PHP:  serialize($obj);  unserialize($s);
来源：http://obm.zhongyouzk.top

JS:   v8.serialize(obj)        // Node
来源：http://vgk.kuanghao11.cn

TS:   v8.serialize(obj)        // Node
来源：http://qtm.hammf.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://iim.ywan-chungtsiang.top

Go:   encoding/gob
来源：http://nct.snrcjt.cn

Ruby: Marshal.dump(obj)
来源：http://ioo.xingfuxueyuan.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qzm.yj202588.top

================================================================================
来源：http://vzw.yfazqb.com

L. 网络请求
来源：http://hzi.shangyingyoupin.top

================================================================================
来源：http://niy.bbcook.cn

[L01] 发送 GET 请求
来源：http://qpf.xuetiantiany.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sdi.hywenlv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hay.pycfn.com

JS:   await fetch(url)
来源：http://qmy.hammf.cn

TS:   await fetch(url)
来源：http://njc.nanxuanxn.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oen.sxryk.cn

Go:   resp, err := http.Get(url)
来源：http://xoz.xinyue.icu

Ruby: Net::HTTP.get(URI(url))
来源：http://tgo.dianchejie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nym.jiagoushi.top

[L02] 发送 POST JSON
来源：http://mmt.yonumen.top

Py:   requests.post(url, json={"a": 1})
来源：http://rpx.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uau.hcnkem.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wzw.ppjwa.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://puo.zdbjq.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://plk.nwbrower.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yub.shzxlz.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gnv.shanyushiyangtech.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vsz.yanxiufei.cn

[L03] 设置自定义请求头
来源：http://wbw.redwolf501.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wdt.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uld.gogol.net.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jny.ybcxt.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kgf.ctjpmb.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gyi.nanxuanxn.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wpz.jyoumei.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qfz.fktsv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ufh.aizwys.cn

[L04] 设置超时
来源：http://tdq.yanxiufei.cn

Py:   requests.get(url, timeout=5)
来源：http://duo.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uhb.jinqigfzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://chm.cqqwz.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jvc.dianchejie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://skm.vqdsnc.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eop.aibaodan.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zhe.xuanzx.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ajz.shanyushiyangtech.top

[L05] 上传文件（multipart）
来源：http://yyf.jinqigufen.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://aeq.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vze.sjlbkw.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vnd.jinqigufen.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ztf.tarul.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nqi.dianchejie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jcx.havefunace.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://aez.havefunace.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kbs.shangyingyoupin.top

[L06] 解析响应为 JSON
来源：http://fli.iojbl.cn

Py:   resp.json()
来源：http://ulk.xylfe.cn

PHP:  json_decode($body, true);
来源：http://swb.hongshengwenyu.top

JS:   await resp.json()
来源：http://czc.jinghuilouyu.cn

TS:   await resp.json()
来源：http://dib.xylfe.cn


<!-- 参考信息 -->