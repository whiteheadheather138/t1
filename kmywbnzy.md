代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://iqa.tarul.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tba.jqgfzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jaz.jqgfzy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vfv.hysaishi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://onj.hysaishi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://shr.jiagoushi.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xkp.gogol.net.cn

[H10] 资源自动释放
来源：http://jte.chenlongwang.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://zvd.nanxinkj.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vqg.yvedp.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kmv.meibo888.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xrb.zhengqikj.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lca.0kj1m.cn

Go:   defer f.Close()
来源：http://xjs.ydzc1.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fdx.ydjk.org.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lxv.zdbjq.cn

================================================================================
来源：http://hhg.0kj1m.cn

I. 正则表达式
来源：http://zit.redwolf501.top

================================================================================
来源：http://udj.fehbvm.com

[I01] 判断是否匹配
来源：http://mdi.yj202588.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://slb.kuanghao11.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rby.tarul.cn

JS:   /\d+/.test(s)
来源：http://iys.jinghuilouyu.cn

TS:   /\d+/.test(s)
来源：http://nws.wangshuangyany.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gee.tian-w.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zyw.jinqigufen.top

Ruby: s.match?(/\d+/)
来源：http://nnh.vqdsnc.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kzn.nanxuanxn.top

[I02] 提取所有匹配
来源：http://jgk.zhengqikj.top

Py:   re.findall(r"\d+", s)
来源：http://zwl.tarul.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tcm.yfazqb.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qrr.yj202588.top

TS:   s.match(/\d+/g)
来源：http://yfk.guannengcc.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hxc.hnxiangtu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://skb.epnwcf.com

Ruby: s.scan(/\d+/)
来源：http://rnw.aibaodan.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kwx.yueranfly.top

[I03] 提取捕获分组
来源：http://chp.quarkkingdee.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uzk.yanxiufei.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rre.yueranfly.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kbo.zdbjq.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sna.hfpthk.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fuh.xingfuxueyuan.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://aok.fehbvm.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nfc.daria6918.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://skj.yj20258.top

[I04] 正则替换
来源：http://qdh.jinqigfzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://zmo.wangshuangyany.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fdc.jinyuanbaomall.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ksi.daxiang520.top

TS:   s.replace(/\d+/g, "#")
来源：http://iwb.nwbrower.top

Java: s.replaceAll("\\d+", "#")
来源：http://ndy.cashguo.top

Go:   re.ReplaceAllString(s, "#")
来源：http://kmp.9152youxi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://knk.aizwys.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://otj.ywan-chungtsiang.top

[I05] 按正则拆分
来源：http://nvl.wangdashe.top

Py:   re.split(r"\s*,\s*", s)
来源：http://jfz.iojbl.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nao.snrcjt.cn

JS:   s.split(/\s*,\s*/)
来源：http://djs.shuidangran.top

TS:   s.split(/\s*,\s*/)
来源：http://cui.jinqigfzy.top

Java: s.split("\\s*,\\s*")
来源：http://ugu.hysaishi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jtg.ydjk.org.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sjt.wangdashe.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kdg.9152youxi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://snz.yueranfly.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fwd.cashguo.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cwd.ivvv.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ciy.hnqzz.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fqm.sjlbkw.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jwi.sufxvd.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://otn.c1oappe.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://icz.yuxming.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://iik.cashguo.top

[I07] 忽略大小写与多行模式
来源：http://zsv.daxiang520.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mrb.chenjidiqi.icu

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qzb.wangdashe.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bdn.dashuyun.cn

TS:   /error/gim
来源：http://ljl.fengsongda.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bjq.jqgfzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bze.jinqigufen.top

Ruby: s.scan(/error/i)
来源：http://vax.fanxiaobao.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rkq.gotoacloud.top

[I08] 贪婪与非贪婪匹配
来源：http://ntu.guowangkeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oph.jlsjyb.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cpr.zhengqikj.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bra.ydjk.org.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tro.ydzc1.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://rjy.zhiwuduotai.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://npf.yonumen.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kgh.yuxming.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gxl.jianghu66.top

================================================================================
来源：http://pal.jiagoushi.top

J. 日期与时间
来源：http://qbv.redwolf501.top

================================================================================
来源：http://psr.jinqigfzy.top

[J01] 获取当前时间
来源：http://tdi.yanxiufei.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wob.vehdjk.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qtb.jiagoushi.top

JS:   new Date();  Date.now()
来源：http://muu.uphjek.com

TS:   new Date();  Date.now()
来源：http://ecb.birdmap.top

Java: LocalDateTime.now();  Instant.now()
来源：http://lqm.ehwqpu.com

Go:   time.Now()
来源：http://edo.ydjk.org.cn

Ruby: Time.now
来源：http://uht.tianlin.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://knh.cqqwz.cn

[J02] 格式化输出
来源：http://psn.tianlin.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jsr.sufxvd.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zco.yanxiufei.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xtf.bbcook.cn

TS:   d.toISOString()
来源：http://qzx.xingfuxueyuan.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://djz.xinyue.icu

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jpj.yonumen.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iph.cqqwz.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kox.wangdashe.top

[J03] 字符串解析为日期
来源：http://vbj.guannengcc.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jmp.zhongyouzk.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://arr.jqgfzy.top

JS:   new Date("2024-01-02")
来源：http://nog.nanxuanxn.top

TS:   new Date("2024-01-02")
来源：http://eec.yonumen.top

Java: LocalDate.parse("2024-01-02")
来源：http://sna.hongshengwenyu.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ozu.jiagoushi.top

Ruby: Date.parse("2024-01-02")
来源：http://dki.tianlin.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gwr.gogol.net.cn

[J04] 时间戳与日期互转
来源：http://twa.hywenlv.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qiq.tarul.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ejo.shanyushiyangtech.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vhh.yonumen.top

TS:   Math.floor(Date.now() / 1000)
来源：http://woz.uphjek.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hnp.zhaomingkeji.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cmx.yangfankeji.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yqi.redwolf501.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xyx.sufxvd.cn

[J05] 时间加减（加 7 天）
来源：http://hpp.gotoacloud.top

Py:   now + timedelta(days=7)
来源：http://lnh.hcnkem.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://xhm.shanyushiyangkeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vxe.tarul.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jvl.gzhubu.top

Java: LocalDate.now().plusDays(7)
来源：http://xfi.xziqi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yyq.tanke756.top

Ruby: Time.now + 7 * 86400
来源：http://idt.quarkkingdee.top

C#:   DateTime.Now.AddDays(7)
来源：http://fmp.316326.xyz

[J06] 计算两时间之差
来源：http://wsd.chenlongwang.top

Py:   (end - start).total_seconds()
来源：http://qqf.fktsv.cn

PHP:  $end->diff($start)->days;
来源：http://fop.0kj1m.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gzq.yangfankeji.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mex.9152youxi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pll.zycfv.cn

Go:   end.Sub(start).Hours()
来源：http://imp.xuetiantiany.cn

Ruby: end - start                 # 返回秒数
来源：http://are.chenzaomai.com

C#:   (end - start).TotalSeconds
来源：http://ytw.yj20258.top

[J07] 比较两个日期
来源：http://bul.fzhhl.top

Py:   d1 < d2;  d1 == d2
来源：http://hmr.snrcjt.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qbq.hnqzz.top

JS:   d1.getTime() < d2.getTime()
来源：http://auv.xinyue.icu

TS:   d1.getTime() < d2.getTime()
来源：http://dgl.sjlbkw.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vah.wangshuangyany.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pem.xuanzx.com

Ruby: d1 < d2;  d1 == d2
来源：http://yja.yj20258.top

C#:   d1 < d2;  d1 == d2
来源：http://xsc.smart0.xyz

[J08] 提取年月日与星期
来源：http://gzn.zhixingplan.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fao.ppjwa.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ctn.bbcook.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pyz.ctjpmb.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ios.vqdsnc.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cth.yj20258888.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sbs.jqgfzy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lrh.tian-w.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fhq.xylfe.cn

[J09] 时区处理
来源：http://ijr.chenzaomai.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zvi.52xcode.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uml.fanxiaobao.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fgu.gogol.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://omh.cqqwz.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wmu.yfazqb.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cbd.cqqwz.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gkz.shanyushiyangkeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uao.zhaomingkeji.xyz

[J10] 取今天 / 本月第一天
来源：http://ooi.hesvh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://von.andypj.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zzf.jyoumei.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://obg.tianlin.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tbk.yj202588.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ixc.yueranfly.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://byr.jinqigufen.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sqn.zdqjudy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bns.tanke756.top

================================================================================
来源：http://osm.vqdsnc.cn

K. JSON 与序列化
来源：http://ubq.ydzc1.top

================================================================================
来源：http://ehh.gotoacloud.top

[K01] 对象转 JSON 字符串
来源：http://bct.hammf.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vtf.vehdjk.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rwf.tarul.cn

JS:   JSON.stringify(obj)
来源：http://waf.ivvv.top

TS:   JSON.stringify(obj)
来源：http://cch.hesvh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sxr.hfpthk.cn

Go:   json.Marshal(obj)
来源：http://psw.shangyingyoupin.top

Ruby: obj.to_json                                     // require "json"
来源：http://lzo.birdmap.top

C#:   JsonSerializer.Serialize(obj)
来源：http://prb.jyoumei.cn

[K02] JSON 字符串转对象
来源：http://zmq.tarul.cn

Py:   json.loads(s)
来源：http://hso.svipenyu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ozd.pengpengdd.cyou

JS:   JSON.parse(s)
来源：http://zoa.ywan-chungtsiang.top

TS:   JSON.parse(s)
来源：http://gmp.ydzc1.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://egg.jinqigufen.top

Go:   json.Unmarshal(data, &v)
来源：http://zca.gaohongyu789.top

Ruby: JSON.parse(s)
来源：http://dec.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nhe.jqgfzy.top

[K03] JSON 美化输出（带缩进）
来源：http://flq.jinqigfzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fli.zhijiandao.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://far.yongpay.top

JS:   JSON.stringify(obj, null, 2)
来源：http://wfh.yfazqb.com

TS:   JSON.stringify(obj, null, 2)
来源：http://lmg.shangyingyoupin.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gec.cqqwz.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ldc.jyoumei.cn

Ruby: JSON.pretty_generate(obj)
来源：http://mhf.hongshengwenyu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://say.yfazqb.com

[K04] 读取 JSON 文件
来源：http://iaq.vqdsnc.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ctz.ywan-chungtsiang.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ppg.shzxlz.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eju.gotoacloud.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kyo.ivvv.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ygw.hcnkem.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://iok.fanxiaobao.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://gzu.hywenlv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cmx.hywenlv.cn

[K05] 深拷贝对象
来源：http://pii.pycfn.com

Py:   copy.deepcopy(obj)
来源：http://mfp.52xcode.cn

PHP:  unserialize(serialize($obj));
来源：http://rvk.bjfxy.top

JS:   structuredClone(obj)
来源：http://vta.wangshuangyany.cn

TS:   structuredClone(obj)
来源：http://mxu.zdbjq.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://icb.xuetiantiany.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fae.jlsjyb.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://egt.0kj1m.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://bvg.zycfv.cn

[K06] 解析 URL 查询串
来源：http://azk.shangyingyoupin.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xlz.yfazqb.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rgk.sweek.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sta.birdmap.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oze.cdnleiting.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wig.yonumen.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://yse.zhiwuduotai.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://azc.fanxiaobao.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fma.tian-w.cn

[K07] 进制转换
来源：http://aot.chenzaomai.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://aym.gzhubu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wgu.redwolf501.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://abr.yanxiufei.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://iof.chenjidiqi.icu

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bdi.shzxlz.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dnq.aizwys.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zmo.chenzaomai.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xnm.yuxming.cn

[K08] 二进制序列化（非 JSON）
来源：http://bbs.52xcode.cn

Py:   pickle.dumps(obj)
来源：http://gcs.smart0.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://vfl.bjfxy.top

JS:   v8.serialize(obj)        // Node
来源：http://vrk.pengpengdd.cyou

TS:   v8.serialize(obj)        // Node
来源：http://dtx.sxryk.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vnl.hesvh.cn

Go:   encoding/gob
来源：http://srg.ppjwa.cn

Ruby: Marshal.dump(obj)
来源：http://vrd.ctjpmb.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ptk.yongpay.top

================================================================================
来源：http://sum.fanxiaobao.xyz

L. 网络请求
来源：http://ccj.shangyingyoupin.top

================================================================================
来源：http://zsb.jlsjyb.cn

[L01] 发送 GET 请求
来源：http://nph.shanyushiyangkeji.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gcy.zhiwuduotai.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ana.yj202588.top

JS:   await fetch(url)
来源：http://ewy.zhijiandao.cn

TS:   await fetch(url)
来源：http://upu.snrcjt.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hdl.ybcxt.top

Go:   resp, err := http.Get(url)
来源：http://fjz.nanxuanxn.top

Ruby: Net::HTTP.get(URI(url))
来源：http://txr.redwolf501.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://haz.hnxiangtu.top

[L02] 发送 POST JSON
来源：http://kok.bjfxy.top

Py:   requests.post(url, json={"a": 1})
来源：http://mmm.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hsc.xingfuxueyuan.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qlc.shanyushiyangkeji.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ucx.ydzc1.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://onz.xingfuxueyuan.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lcs.feifeiyinyue.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://eiu.hesvh.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jqk.smart0.xyz

[L03] 设置自定义请求头
来源：http://qei.nanxinkj.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kcl.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sxk.ybcxt.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://crp.ctjpmb.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nyr.ydzc1.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nyc.fengsongda.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kqe.xuanzx.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xvd.zhongyouzk.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xgq.ywan-chungtsiang.top

[L04] 设置超时
来源：http://aih.yfazqb.com

Py:   requests.get(url, timeout=5)
来源：http://bil.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ers.nwbrower.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wux.hammf.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mig.meibo888.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dgk.dashuyun.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xzj.zhiwuduotai.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bkq.yuxming.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ves.uphjek.com

[L05] 上传文件（multipart）
来源：http://dbu.jinyuanbaomall.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://alf.chenlongwang.top


<!-- 参考信息 -->