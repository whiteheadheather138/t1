代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mcx.haohaochexian.top

Go:   defer f.Close()
来源：http://dgf.zhiwuduotai.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sxx.snrcjt.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ylz.shangyingyoupin.top

================================================================================
来源：http://fec.cashguo.top

I. 正则表达式
来源：http://woe.vqdsnc.cn

================================================================================
来源：http://blq.hysaishi.cn

[I01] 判断是否匹配
来源：http://qii.sjlbkw.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ptf.havefunace.top

PHP:  preg_match('/\d+/', $s);
来源：http://qli.0kj1m.cn

JS:   /\d+/.test(s)
来源：http://imi.snrcjt.cn

TS:   /\d+/.test(s)
来源：http://ibs.yonumen.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cpl.iojbl.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lxc.yj20258888.top

Ruby: s.match?(/\d+/)
来源：http://vin.yvedp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bno.bbcook.cn

[I02] 提取所有匹配
来源：http://brb.bjfxy.top

Py:   re.findall(r"\d+", s)
来源：http://yyp.xziqi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bzx.0kj1m.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jbx.sxryk.cn

TS:   s.match(/\d+/g)
来源：http://wvo.ywan-chungtsiang.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ycf.gogol.net.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yui.hysaishi.cn

Ruby: s.scan(/\d+/)
来源：http://ncy.nanxuanxn.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mys.ybcxt.top

[I03] 提取捕获分组
来源：http://qrh.feifeiyinyue.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xfv.9152youxi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wna.wangdashe.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://giz.daria6918.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zqb.xylfe.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nir.ydjk.org.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nbh.xuetiantiany.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rna.sweek.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tvj.zhengqikj.top

[I04] 正则替换
来源：http://bdb.chenjidiqi.icu

Py:   re.sub(r"\d+", "#", s)
来源：http://rem.yvedp.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uym.fktsv.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ead.jianghu66.top

TS:   s.replace(/\d+/g, "#")
来源：http://lao.yj20258888.top

Java: s.replaceAll("\\d+", "#")
来源：http://bww.jlsjyb.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://nki.pycfn.com

Ruby: s.gsub(/\d+/, "#")
来源：http://lys.pycfn.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sir.dashuyun.cn

[I05] 按正则拆分
来源：http://vie.tian-w.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tfw.ehwqpu.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vdn.hnxiangtu.top

JS:   s.split(/\s*,\s*/)
来源：http://uwu.hnxiangtu.top

TS:   s.split(/\s*,\s*/)
来源：http://dav.yanxiufei.cn

Java: s.split("\\s*,\\s*")
来源：http://gbj.sxryk.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://srz.cqqwz.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nij.vqdsnc.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yyv.pengpengdd.cyou

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sly.shzxlz.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nby.zycfv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://svu.gotoacloud.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rdy.hnqzz.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://opm.xziqi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xjf.wangshuangyany.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://eqr.yj202588.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vvu.yj202588.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gmn.hnxiangtu.top

[I07] 忽略大小写与多行模式
来源：http://udl.sufxvd.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wrp.havefunace.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sdi.smart0.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ixi.yj20258888.top

TS:   /error/gim
来源：http://fgu.daxiang520.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://iey.xylfe.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://slx.yuanzhike.top

Ruby: s.scan(/error/i)
来源：http://pig.gaohongyu789.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hdc.fktsv.cn

[I08] 贪婪与非贪婪匹配
来源：http://hoc.shanyushiyangkeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://whl.nanxinkj.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kyb.jianghu66.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://iir.vqdsnc.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dtg.wangdashe.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ynx.svipenyu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wbo.shangyingyoupin.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xqy.zhixingplan.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kze.svipenyu.cn

================================================================================
来源：http://szi.yj20258.top

J. 日期与时间
来源：http://byo.cqqwz.cn

================================================================================
来源：http://fki.tarul.cn

[J01] 获取当前时间
来源：http://zmf.xinyue.icu

Py:   datetime.now();  datetime.now(UTC)
来源：http://guh.epnwcf.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wox.guannengcc.top

JS:   new Date();  Date.now()
来源：http://jja.zhengqikj.top

TS:   new Date();  Date.now()
来源：http://xts.yj20258888.top

Java: LocalDateTime.now();  Instant.now()
来源：http://dab.52xcode.cn

Go:   time.Now()
来源：http://uxw.gotoacloud.top

Ruby: Time.now
来源：http://kni.fktsv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://epx.yanxiufei.cn

[J02] 格式化输出
来源：http://htj.nwbrower.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ktt.yongpay.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mum.hfpthk.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vfn.hywenlv.cn

TS:   d.toISOString()
来源：http://gje.zhengqikj.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://daz.zhaomingkeji.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sff.xziqi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vhn.hnxiangtu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pgt.yuxming.cn

[J03] 字符串解析为日期
来源：http://mjr.jyoumei.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ckq.cashguo.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://smg.kuanghao11.cn

JS:   new Date("2024-01-02")
来源：http://jpl.shangyingyoupin.top

TS:   new Date("2024-01-02")
来源：http://jdi.ehwqpu.com

Java: LocalDate.parse("2024-01-02")
来源：http://moe.hywenlv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://enf.svipenyu.cn

Ruby: Date.parse("2024-01-02")
来源：http://zzm.yj20258888.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qdt.gogol.net.cn

[J04] 时间戳与日期互转
来源：http://eij.yj202588.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ouv.jqgufenzy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fec.xinyue.icu

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xxr.iojbl.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dri.zdqjudy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kdf.feifeiyinyue.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oft.9152youxi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lyo.tian-w.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://srz.zhongyouzk.top

[J05] 时间加减（加 7 天）
来源：http://bcz.jinqigufen.top

Py:   now + timedelta(days=7)
来源：http://pgd.jinqigufen.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://kyk.yonumen.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://npq.nwbrower.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mzl.yonumen.top

Java: LocalDate.now().plusDays(7)
来源：http://pqe.daria6918.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gwj.bbcook.cn

Ruby: Time.now + 7 * 86400
来源：http://zft.zhoulong.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://mae.aibaodan.cn

[J06] 计算两时间之差
来源：http://irg.yuxming.cn

Py:   (end - start).total_seconds()
来源：http://bxj.zdbjq.cn

PHP:  $end->diff($start)->days;
来源：http://lkb.wangshuangyany.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ssq.yangfankeji.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ryh.svipenyu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wla.vqdsnc.cn

Go:   end.Sub(start).Hours()
来源：http://izz.vehdjk.com

Ruby: end - start                 # 返回秒数
来源：http://rzh.9152youxi.cn

C#:   (end - start).TotalSeconds
来源：http://zcc.redwolf501.top

[J07] 比较两个日期
来源：http://jis.gaohongyu789.top

Py:   d1 < d2;  d1 == d2
来源：http://nou.wangshuangyany.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uzq.svipenyu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tos.hysaishi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lwn.redwolf501.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ous.gogol.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zgt.chenlongwang.top

Ruby: d1 < d2;  d1 == d2
来源：http://qvm.c1oappe.top

C#:   d1 < d2;  d1 == d2
来源：http://quq.shanyushiyangtech.top

[J08] 提取年月日与星期
来源：http://fbp.daxiang520.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kpv.jinqigfzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://acj.zdbjq.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kmm.jinghuilouyu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tkd.jqgfzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://huh.jlsjyb.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zbl.dianchejie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://aix.fanxiaobao.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fei.cdnleiting.top

[J09] 时区处理
来源：http://xvz.xuanzx.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hcd.zdqjudy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nww.yuanzhike.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qkh.zhoulong.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bps.sjlbkw.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ubw.sysykeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://itf.zdbjq.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://kam.quarkkingdee.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qtm.pycfn.com

[J10] 取今天 / 本月第一天
来源：http://sos.ywan-chungtsiang.top

Py:   date.today();  date.today().replace(day=1)
来源：http://lwu.zdqjudy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fej.0kj1m.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xff.zhongyouzk.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jrf.bjfxy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ayo.yj20258888.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vud.zycfv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fhu.zhaomingkeji.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://but.sysykeji.top

================================================================================
来源：http://hkk.ywan-chungtsiang.top

K. JSON 与序列化
来源：http://swn.fehbvm.com

================================================================================
来源：http://yxj.hammf.cn

[K01] 对象转 JSON 字符串
来源：http://imu.jinghuilouyu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fwu.sjlbkw.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mis.vqdsnc.cn

JS:   JSON.stringify(obj)
来源：http://ent.hesvh.cn

TS:   JSON.stringify(obj)
来源：http://pnq.jinqigufen.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wqz.sysykeji.top

Go:   json.Marshal(obj)
来源：http://uuk.wangdashe.top

Ruby: obj.to_json                                     // require "json"
来源：http://tdh.ywan-chungtsiang.top

C#:   JsonSerializer.Serialize(obj)
来源：http://mvz.tanke756.top

[K02] JSON 字符串转对象
来源：http://iwu.xuetiantiany.cn

Py:   json.loads(s)
来源：http://hen.316326.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://duh.zdqjudy.top

JS:   JSON.parse(s)
来源：http://dit.316326.xyz

TS:   JSON.parse(s)
来源：http://urc.zhixingplan.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hty.svipenyu.cn

Go:   json.Unmarshal(data, &v)
来源：http://tsf.jqgfzy.top

Ruby: JSON.parse(s)
来源：http://wyr.guowangkeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ojp.yj20258.top

[K03] JSON 美化输出（带缩进）
来源：http://phr.hammf.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vgd.havefunace.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fbq.bbcook.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://mki.havefunace.top

TS:   JSON.stringify(obj, null, 2)
来源：http://czr.yuxming.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://moi.aizwys.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://etx.nanxuanxn.top

Ruby: JSON.pretty_generate(obj)
来源：http://svu.guannengcc.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vcj.smart0.xyz

[K04] 读取 JSON 文件
来源：http://mwa.quarkkingdee.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wby.ybcxt.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qvu.haohaochexian.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vlu.hysaishi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sbn.birdmap.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jga.sysykeji.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rlb.fzhhl.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://dml.fengsongda.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zph.xingfuxueyuan.xyz

[K05] 深拷贝对象
来源：http://unk.fzhhl.top

Py:   copy.deepcopy(obj)
来源：http://xmw.meibo888.top

PHP:  unserialize(serialize($obj));
来源：http://ali.sjlbkw.cn

JS:   structuredClone(obj)
来源：http://wdr.shangyingyoupin.top

TS:   structuredClone(obj)
来源：http://ykm.xylfe.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://yfq.yonumen.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nzx.havefunace.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://klk.meibo888.top

C#:   // 序列化往返，或自定义 Clone
来源：http://pxe.gotoacloud.top

[K06] 解析 URL 查询串
来源：http://xie.hongshengwenyu.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bxd.gotoacloud.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ejd.wangdashe.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vdx.zhengqikj.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hsl.fengsongda.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://agl.guannengcc.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://mhr.zhengqikj.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uzk.shzxlz.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nfa.aizwys.cn

[K07] 进制转换
来源：http://sbi.zhaomingkeji.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wrz.cheryme.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ykm.9152youxi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hfq.tianlin.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kxj.nwbrower.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://alc.uphjek.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ldv.zhixingplan.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fnh.shanyushiyangkeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zif.tian-w.cn

[K08] 二进制序列化（非 JSON）
来源：http://ihf.jqgufenzy.top

Py:   pickle.dumps(obj)
来源：http://rky.tianlin.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://too.hnqzz.top

JS:   v8.serialize(obj)        // Node
来源：http://yqg.fanxiaobao.xyz

TS:   v8.serialize(obj)        // Node
来源：http://lgq.xylfe.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dfg.zhiwuduotai.top

Go:   encoding/gob
来源：http://gtv.tianlin.xyz

Ruby: Marshal.dump(obj)
来源：http://vzt.zhijiandao.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://msh.zdbjq.cn

================================================================================
来源：http://tio.havefunace.top

L. 网络请求
来源：http://aio.wangdashe.top

================================================================================
来源：http://fki.gaohongyu789.top

[L01] 发送 GET 请求
来源：http://axm.uphjek.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://otz.zhengqikj.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ndu.jinqigfzy.top

JS:   await fetch(url)
来源：http://izb.yueranfly.top

TS:   await fetch(url)
来源：http://zpv.sweek.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://afi.shzxlz.cn

Go:   resp, err := http.Get(url)
来源：http://vvs.fehbvm.com

Ruby: Net::HTTP.get(URI(url))
来源：http://mbr.zdqjudy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ywr.pycfn.com

[L02] 发送 POST JSON
来源：http://vft.shanyushiyangtech.top

Py:   requests.post(url, json={"a": 1})
来源：http://xws.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nak.c1oappe.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ewq.uphjek.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://niz.yangfankeji.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bgv.fengsongda.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dci.hesvh.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mvp.xingfuxueyuan.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yqw.jinghuilouyu.cn

[L03] 设置自定义请求头
来源：http://rmo.smart0.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pjf.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://eck.havefunace.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vys.aizwys.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://clj.jianghu66.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uwh.tian-w.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tna.bjfxy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kre.jiagoushi.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lhk.epnwcf.com

[L04] 设置超时
来源：http://ziq.ehwqpu.com

Py:   requests.get(url, timeout=5)
来源：http://ymt.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xyv.redwolf501.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://myw.yueranfly.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pee.zycfv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bee.dashuyun.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hox.zhaomingkeji.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://olp.tian-w.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kiu.fzhhl.top

[L05] 上传文件（multipart）
来源：http://tcc.hongshengwenyu.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mdc.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sfb.jlsjyb.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mej.dianchejie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://atb.vehdjk.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vdz.gogol.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vzx.chenlongwang.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://iax.zhongyouzk.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zxk.cdnleiting.top

[L06] 解析响应为 JSON
来源：http://pzv.xziqi.cn

Py:   resp.json()
来源：http://vvs.zdbjq.cn

PHP:  json_decode($body, true);
来源：http://rtv.fengsongda.top

JS:   await resp.json()
来源：http://nkx.nanxuanxn.top

TS:   await resp.json()
来源：http://lrq.316326.xyz


<!-- 参考信息 -->