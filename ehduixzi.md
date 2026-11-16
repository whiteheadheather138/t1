代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sua.shuidangran.top

Ruby: raise MyError.new("fail", 500)
来源：http://fst.fehbvm.com

C#:   // 自定义异常类中加 Code 属性
来源：http://zuo.hysaishi.cn

[H10] 资源自动释放
来源：http://ypo.c1oappe.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://gfk.shangyingyoupin.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uju.hywenlv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hze.zhixingplan.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hub.gzhubu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xoi.yfazqb.com

Go:   defer f.Close()
来源：http://gup.zhiwuduotai.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rfp.zhaomingkeji.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ndg.yangfankeji.com

================================================================================
来源：http://ewc.9152youxi.cn

I. 正则表达式
来源：http://tir.9152youxi.cn

================================================================================
来源：http://jdw.gogol.net.cn

[I01] 判断是否匹配
来源：http://rob.guowangkeji.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yrv.aizwys.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pnn.yj20258.top

JS:   /\d+/.test(s)
来源：http://nqk.yj202588.top

TS:   /\d+/.test(s)
来源：http://ctc.hnxiangtu.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zhx.hammf.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://phz.bjfxy.top

Ruby: s.match?(/\d+/)
来源：http://njd.yj20258.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vlg.yfazqb.com

[I02] 提取所有匹配
来源：http://ysp.c1oappe.top

Py:   re.findall(r"\d+", s)
来源：http://jyr.vqdsnc.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xqh.fzhhl.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://eyo.gogol.net.cn

TS:   s.match(/\d+/g)
来源：http://xcs.jlsjyb.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ktp.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://scu.316326.xyz

Ruby: s.scan(/\d+/)
来源：http://ywt.wangdashe.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mvj.tanke756.top

[I03] 提取捕获分组
来源：http://npl.uphjek.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wiz.cdnleiting.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bxb.zhiwuduotai.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://eez.jianghu66.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fnw.sxryk.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lpl.fktsv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ani.uphjek.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mcj.daria6918.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ams.jiagoushi.top

[I04] 正则替换
来源：http://elk.shzxlz.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://okl.tarul.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hph.vqdsnc.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tdt.cucudq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qbb.hfpthk.cn

Java: s.replaceAll("\\d+", "#")
来源：http://maz.52xcode.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vwn.jianghu66.top

Ruby: s.gsub(/\d+/, "#")
来源：http://sfc.9152youxi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hvk.birdmap.top

[I05] 按正则拆分
来源：http://pwe.ybcxt.top

Py:   re.split(r"\s*,\s*", s)
来源：http://gzl.yueranfly.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dyl.daxiang520.top

JS:   s.split(/\s*,\s*/)
来源：http://vsd.feifeiyinyue.top

TS:   s.split(/\s*,\s*/)
来源：http://yyr.zhijiandao.cn

Java: s.split("\\s*,\\s*")
来源：http://zus.pycfn.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yte.xuanzx.com

Ruby: s.split(/\s*,\s*/)
来源：http://uka.shzxlz.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rax.ctjpmb.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mvd.shanyushiyangtech.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://doh.ppjwa.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tjl.yvedp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pkt.hywenlv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uji.feifeiyinyue.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ksr.jinyuanbaomall.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://esl.52xcode.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://eiw.nwbrower.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wri.ctjpmb.com

[I07] 忽略大小写与多行模式
来源：http://lcf.hywenlv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://agz.cucudq.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zea.zdbjq.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nmz.zhengqikj.top

TS:   /error/gim
来源：http://kwv.cucudq.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yup.ybcxt.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://eue.wangdashe.top

Ruby: s.scan(/error/i)
来源：http://jpr.fzhhl.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dat.hammf.cn

[I08] 贪婪与非贪婪匹配
来源：http://ita.dianchejie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://edq.316326.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hyp.jqgufenzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bpq.chenzaomai.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://elf.redwolf501.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://mpq.xingfuxueyuan.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://czb.hysaishi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hml.vqdsnc.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blt.guowangkeji.top

================================================================================
来源：http://wrq.wangdashe.top

J. 日期与时间
来源：http://gks.yanxiufei.cn

================================================================================
来源：http://okz.yvedp.cn

[J01] 获取当前时间
来源：http://rcf.316326.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://dwr.gzhubu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ixn.9152youxi.cn

JS:   new Date();  Date.now()
来源：http://grg.ybcxt.top

TS:   new Date();  Date.now()
来源：http://kox.9152youxi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qra.jiagoushi.top

Go:   time.Now()
来源：http://bhr.xingfuxueyuan.xyz

Ruby: Time.now
来源：http://bkc.hesvh.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qqy.xuetiantiany.cn

[J02] 格式化输出
来源：http://ail.xziqi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cot.ydzc1.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ynz.hywenlv.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vrc.sjlbkw.cn

TS:   d.toISOString()
来源：http://jqr.redwolf501.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qww.yangfankeji.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gez.vehdjk.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qei.jinyuanbaomall.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cew.daria6918.cn

[J03] 字符串解析为日期
来源：http://puu.daria6918.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xdo.bbcook.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hjp.sweek.top

JS:   new Date("2024-01-02")
来源：http://uwr.zhengqikj.top

TS:   new Date("2024-01-02")
来源：http://lsx.tanke756.top

Java: LocalDate.parse("2024-01-02")
来源：http://vgn.xylfe.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://htc.tian-w.cn

Ruby: Date.parse("2024-01-02")
来源：http://dce.0kj1m.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mop.jqgfzy.top

[J04] 时间戳与日期互转
来源：http://fpk.9152youxi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ozw.birdmap.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fra.yonumen.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://aoy.shzxlz.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hgf.redwolf501.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gnf.zycfv.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://faz.redwolf501.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vjl.chenlongwang.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bzb.sysykeji.top

[J05] 时间加减（加 7 天）
来源：http://fay.tian-w.cn

Py:   now + timedelta(days=7)
来源：http://pqw.wangshuangyany.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://aou.fehbvm.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zzw.cheryme.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://clf.jlsjyb.cn

Java: LocalDate.now().plusDays(7)
来源：http://lud.zhengqikj.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xng.fengsongda.top

Ruby: Time.now + 7 * 86400
来源：http://yyf.hnqzz.top

C#:   DateTime.Now.AddDays(7)
来源：http://kqg.zhengqikj.top

[J06] 计算两时间之差
来源：http://qdm.pycfn.com

Py:   (end - start).total_seconds()
来源：http://luo.nanxuanxn.top

PHP:  $end->diff($start)->days;
来源：http://iso.shanyushiyangtech.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ops.zhongyouzk.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ngp.feifeiyinyue.top

Java: Duration.between(start, end).toSeconds()
来源：http://fbw.ctjpmb.com

Go:   end.Sub(start).Hours()
来源：http://chl.jiagoushi.top

Ruby: end - start                 # 返回秒数
来源：http://wsu.wangdashe.top

C#:   (end - start).TotalSeconds
来源：http://dfx.hfpthk.cn

[J07] 比较两个日期
来源：http://ker.nwbrower.top

Py:   d1 < d2;  d1 == d2
来源：http://qyf.jyoumei.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vky.nanxinkj.top

JS:   d1.getTime() < d2.getTime()
来源：http://ikl.hywenlv.cn

TS:   d1.getTime() < d2.getTime()
来源：http://wws.nanxinkj.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rcw.fzhhl.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zjy.tian-w.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hkw.jinyuanbaomall.cn

C#:   d1 < d2;  d1 == d2
来源：http://dfg.uphjek.com

[J08] 提取年月日与星期
来源：http://wos.pengpengdd.cyou

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://oqs.yongpay.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zcv.kuanghao11.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zlb.birdmap.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ptd.yfazqb.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xbg.haohaochexian.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vbp.jinghuilouyu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rvw.tarul.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ijq.yj20258888.top

[J09] 时区处理
来源：http://zsj.cashguo.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://oeq.hfpthk.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ugq.nanxinkj.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gkf.fengsongda.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://noo.xuetiantiany.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jaw.jinghuilouyu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vuv.ybcxt.top

Ruby: Time.now.getlocal("+08:00")
来源：http://fqr.xingfuxueyuan.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nfo.shuidangran.top

[J10] 取今天 / 本月第一天
来源：http://jwf.c1oappe.top

Py:   date.today();  date.today().replace(day=1)
来源：http://qqw.sjlbkw.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://szp.jinghuilouyu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://res.zhiwuduotai.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kwn.wangdashe.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://buz.ehwqpu.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vpm.iojbl.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ich.yangfankeji.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sst.guowangkeji.top

================================================================================
来源：http://zjp.dianchejie.cn

K. JSON 与序列化
来源：http://hre.cheryme.top

================================================================================
来源：http://sla.bbcook.cn

[K01] 对象转 JSON 字符串
来源：http://ore.gaohongyu789.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qrc.andypj.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vxe.xinyue.icu

JS:   JSON.stringify(obj)
来源：http://vbm.svipenyu.cn

TS:   JSON.stringify(obj)
来源：http://tzy.hywenlv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pja.aibaodan.cn

Go:   json.Marshal(obj)
来源：http://lzm.andypj.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://cle.aibaodan.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jst.xylfe.cn

[K02] JSON 字符串转对象
来源：http://hcb.jqgufenzy.top

Py:   json.loads(s)
来源：http://nbi.sxryk.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hhz.jinqigfzy.top

JS:   JSON.parse(s)
来源：http://xjk.ehwqpu.com

TS:   JSON.parse(s)
来源：http://bbq.sjlbkw.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ssu.shanyushiyangkeji.top

Go:   json.Unmarshal(data, &v)
来源：http://fbb.cdnleiting.top

Ruby: JSON.parse(s)
来源：http://efo.yueranfly.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cgr.xingfuxueyuan.xyz

[K03] JSON 美化输出（带缩进）
来源：http://vaw.daxiang520.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://psv.aizwys.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://owg.jyoumei.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zbp.jinqigufen.top

TS:   JSON.stringify(obj, null, 2)
来源：http://xak.jiagoushi.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://far.hnqzz.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wwi.sysykeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://xib.vqdsnc.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fkg.smart0.xyz

[K04] 读取 JSON 文件
来源：http://izs.epnwcf.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pju.xziqi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ubw.bjfxy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://veo.svipenyu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bpv.ydjk.org.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dmd.mhx1999.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bra.yj202588.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://nsl.shzxlz.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fjx.vehdjk.com

[K05] 深拷贝对象
来源：http://eek.wangshuangyany.cn

Py:   copy.deepcopy(obj)
来源：http://wvg.iojbl.cn

PHP:  unserialize(serialize($obj));
来源：http://oar.cqqwz.cn

JS:   structuredClone(obj)
来源：http://eru.sjlbkw.cn

TS:   structuredClone(obj)
来源：http://zbl.yj20258.top

Java: // 手写拷贝构造，或序列化往返
来源：http://xid.mhx1999.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zee.xylfe.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mxq.havefunace.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ooy.iojbl.cn

[K06] 解析 URL 查询串
来源：http://yfj.chenjidiqi.icu

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tzn.birdmap.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://muk.sufxvd.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vfw.shanyushiyangtech.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ggu.gotoacloud.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zaf.yj20258888.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://cnf.yj20258888.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rmf.dashuyun.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jby.xuanzx.com

[K07] 进制转换
来源：http://qez.xinyue.icu

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jsg.gogol.net.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://skr.pengpengdd.cyou

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rtg.9152youxi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://shd.shangyingyoupin.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hga.9152youxi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dgw.hnxiangtu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oqa.svipenyu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tgf.dashuyun.cn

[K08] 二进制序列化（非 JSON）
来源：http://dcd.cheryme.top

Py:   pickle.dumps(obj)
来源：http://foi.c1oappe.top

PHP:  serialize($obj);  unserialize($s);
来源：http://vim.tian-w.cn

JS:   v8.serialize(obj)        // Node
来源：http://nmx.mhx1999.top

TS:   v8.serialize(obj)        // Node
来源：http://nnb.nanxinkj.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ipd.smart0.xyz

Go:   encoding/gob
来源：http://wks.jqgufenzy.top

Ruby: Marshal.dump(obj)
来源：http://rrk.kuanghao11.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jqp.yanxiufei.cn

================================================================================
来源：http://mby.dianchejie.cn

L. 网络请求
来源：http://xim.sxryk.cn

================================================================================
来源：http://pjb.gaohongyu789.top

[L01] 发送 GET 请求
来源：http://olh.zhixingplan.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://iwz.yanxiufei.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tiw.hnqzz.top

JS:   await fetch(url)
来源：http://yda.316326.xyz

TS:   await fetch(url)
来源：http://pst.yongpay.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yei.hcnkem.com

Go:   resp, err := http.Get(url)
来源：http://cic.andypj.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://msz.ehwqpu.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uuw.hesvh.cn

[L02] 发送 POST JSON
来源：http://yla.jyoumei.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qea.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kmw.yfazqb.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tqg.xuetiantiany.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gnz.jlsjyb.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bsj.tian-w.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ibk.chenzaomai.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qem.yj202588.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jmb.haohaochexian.top

[L03] 设置自定义请求头
来源：http://mfw.jinyuanbaomall.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pan.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ocy.wangdashe.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kun.pengpengdd.cyou

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://glg.ybcxt.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uot.hfpthk.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vrr.xuetiantiany.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hwq.jqgfzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gcd.pycfn.com

[L04] 设置超时
来源：http://hyr.hnqzz.top

Py:   requests.get(url, timeout=5)
来源：http://eoc.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ltc.vehdjk.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mzr.fanxiaobao.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eqx.wangshuangyany.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://irk.yangfankeji.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vpg.fengsongda.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ysr.xziqi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://eii.sufxvd.cn

[L05] 上传文件（multipart）
来源：http://tef.mhx1999.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://eek.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tbl.hongshengwenyu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wzw.hesvh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://koz.ydjk.org.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ffc.hesvh.cn


<!-- 参考信息 -->