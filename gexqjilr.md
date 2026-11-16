代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://dyr.pycfn.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rpv.jinqigfzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://shn.iojbl.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rif.hnxiangtu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dkb.jyoumei.cn

Ruby: raise MyError.new("fail", 500)
来源：http://arp.zhongyouzk.top

C#:   // 自定义异常类中加 Code 属性
来源：http://kfl.sxryk.cn

[H10] 资源自动释放
来源：http://gvp.9152youxi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xrj.xuetiantiany.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cjw.xinyue.icu

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nrg.cucudq.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://agm.aibaodan.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wge.birdmap.top

Go:   defer f.Close()
来源：http://anz.aibaodan.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xoi.zhongyouzk.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dgi.jqgfzy.top

================================================================================
来源：http://uxl.zhijiandao.cn

I. 正则表达式
来源：http://rhx.9152youxi.cn

================================================================================
来源：http://vay.cucudq.cn

[I01] 判断是否匹配
来源：http://dbr.shuidangran.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cbs.chenzaomai.com

PHP:  preg_match('/\d+/', $s);
来源：http://pwv.zhijiandao.cn

JS:   /\d+/.test(s)
来源：http://hmw.aizwys.cn

TS:   /\d+/.test(s)
来源：http://uke.ctjpmb.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wci.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jai.gogol.net.cn

Ruby: s.match?(/\d+/)
来源：http://uas.chenlongwang.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hth.shangyingyoupin.top

[I02] 提取所有匹配
来源：http://ffs.gogol.net.cn

Py:   re.findall(r"\d+", s)
来源：http://pwk.yj20258.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://diw.yongpay.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lhj.gaohongyu789.top

TS:   s.match(/\d+/g)
来源：http://wgn.pycfn.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ggm.9152youxi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bkl.ybcxt.top

Ruby: s.scan(/\d+/)
来源：http://tqh.shangyingyoupin.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pid.snrcjt.cn

[I03] 提取捕获分组
来源：http://gfg.hongshengwenyu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dpb.yj20258888.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://oez.jianghu66.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kpb.cdnleiting.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ywn.fengsongda.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://iif.ivvv.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ybz.bjfxy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pvk.tarul.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ctz.cheryme.top

[I04] 正则替换
来源：http://qpx.gaohongyu789.top

Py:   re.sub(r"\d+", "#", s)
来源：http://fgn.jinghuilouyu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fpl.cqqwz.cn

JS:   s.replace(/\d+/g, "#")
来源：http://juk.zycfv.cn

TS:   s.replace(/\d+/g, "#")
来源：http://erc.yonumen.top

Java: s.replaceAll("\\d+", "#")
来源：http://uqh.chenlongwang.top

Go:   re.ReplaceAllString(s, "#")
来源：http://mln.zycfv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xek.cashguo.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xjv.jiagoushi.top

[I05] 按正则拆分
来源：http://ndg.andypj.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://vnz.yj20258888.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qpp.hysaishi.cn

JS:   s.split(/\s*,\s*/)
来源：http://gjn.bjfxy.top

TS:   s.split(/\s*,\s*/)
来源：http://yfb.tianlin.xyz

Java: s.split("\\s*,\\s*")
来源：http://bfe.ivvv.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://oey.hysaishi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wcl.gaohongyu789.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qbg.zycfv.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://iqg.uphjek.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://soq.haohaochexian.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://odn.xuetiantiany.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jwx.fehbvm.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://izc.jlsjyb.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rtk.sysykeji.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jlw.zycfv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qqr.hesvh.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cxs.xuanzx.com

[I07] 忽略大小写与多行模式
来源：http://jwd.meibo888.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://slt.gaohongyu789.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yyx.yuanzhike.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tup.0kj1m.cn

TS:   /error/gim
来源：http://efo.aibaodan.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kky.kuanghao11.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gyz.mhx1999.top

Ruby: s.scan(/error/i)
来源：http://nbi.epnwcf.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vtv.hywenlv.cn

[I08] 贪婪与非贪婪匹配
来源：http://wxp.zhoulong.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cei.chenzaomai.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gpb.jiagoushi.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zdt.yj202588.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jjn.gaohongyu789.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://zfw.tanke756.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://scr.quarkkingdee.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vla.jqgufenzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lhk.fktsv.cn

================================================================================
来源：http://wiw.hnqzz.top

J. 日期与时间
来源：http://tvc.hywenlv.cn

================================================================================
来源：http://bry.vehdjk.com

[J01] 获取当前时间
来源：http://ctk.birdmap.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ynw.fengsongda.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nvg.tianlin.xyz

JS:   new Date();  Date.now()
来源：http://iao.hesvh.cn

TS:   new Date();  Date.now()
来源：http://kxi.cucudq.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tou.ydjk.org.cn

Go:   time.Now()
来源：http://odq.fehbvm.com

Ruby: Time.now
来源：http://shj.jianghu66.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gbg.sweek.top

[J02] 格式化输出
来源：http://pvx.nanxinkj.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wno.yangfankeji.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gcp.jianghu66.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://max.zhixingplan.top

TS:   d.toISOString()
来源：http://ufd.nanxinkj.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rue.jqgfzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lwz.316326.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fya.316326.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zmv.dianchejie.cn

[J03] 字符串解析为日期
来源：http://oqv.gzhubu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bcw.fktsv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uur.sxryk.cn

JS:   new Date("2024-01-02")
来源：http://yfj.sysykeji.top

TS:   new Date("2024-01-02")
来源：http://hbn.cashguo.top

Java: LocalDate.parse("2024-01-02")
来源：http://acq.fengsongda.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bvv.tarul.cn

Ruby: Date.parse("2024-01-02")
来源：http://yxb.andypj.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rra.cheryme.top

[J04] 时间戳与日期互转
来源：http://qem.nanxinkj.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wtm.iojbl.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cim.gotoacloud.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jpp.birdmap.top

TS:   Math.floor(Date.now() / 1000)
来源：http://vcb.tianlin.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dvh.yuanzhike.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yqn.316326.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://txy.guowangkeji.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vsx.yuanzhike.top

[J05] 时间加减（加 7 天）
来源：http://fnb.bbcook.cn

Py:   now + timedelta(days=7)
来源：http://cvj.hcnkem.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://ifh.jqgfzy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tmw.hesvh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nlg.jinyuanbaomall.cn

Java: LocalDate.now().plusDays(7)
来源：http://idy.feifeiyinyue.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qws.zhijiandao.cn

Ruby: Time.now + 7 * 86400
来源：http://sew.jinyuanbaomall.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ffi.pengpengdd.cyou

[J06] 计算两时间之差
来源：http://hlm.pengpengdd.cyou

Py:   (end - start).total_seconds()
来源：http://npg.jinghuilouyu.cn

PHP:  $end->diff($start)->days;
来源：http://bkh.hcnkem.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kvf.yongpay.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jou.xuanzx.com

Java: Duration.between(start, end).toSeconds()
来源：http://dlz.zhongyouzk.top

Go:   end.Sub(start).Hours()
来源：http://jlk.jinqigufen.top

Ruby: end - start                 # 返回秒数
来源：http://umc.iojbl.cn

C#:   (end - start).TotalSeconds
来源：http://smy.guannengcc.top

[J07] 比较两个日期
来源：http://byq.nanxuanxn.top

Py:   d1 < d2;  d1 == d2
来源：http://oqo.bjfxy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hoi.zhijiandao.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qyx.jinyuanbaomall.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mbd.cucudq.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rxw.svipenyu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vhk.fehbvm.com

Ruby: d1 < d2;  d1 == d2
来源：http://jzk.xuanzx.com

C#:   d1 < d2;  d1 == d2
来源：http://grb.cucudq.cn

[J08] 提取年月日与星期
来源：http://xcp.hongshengwenyu.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gmf.jqgfzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ymw.fzhhl.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jyx.jinyuanbaomall.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gex.birdmap.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yhd.yuxming.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jty.52xcode.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ilm.hnqzz.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://low.gzhubu.top

[J09] 时区处理
来源：http://xov.xuanzx.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dcj.sxryk.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://phi.redwolf501.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ehi.wangdashe.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gpc.jqgufenzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://out.ybcxt.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://szu.snrcjt.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://bvb.fengsongda.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cxc.tarul.cn

[J10] 取今天 / 本月第一天
来源：http://ubl.tanke756.top

Py:   date.today();  date.today().replace(day=1)
来源：http://gkb.bbcook.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qre.0kj1m.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nnl.sufxvd.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ywi.birdmap.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sjt.tian-w.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://stf.uphjek.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pkk.chenzaomai.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ycb.hcnkem.com

================================================================================
来源：http://msc.gaohongyu789.top

K. JSON 与序列化
来源：http://csf.cashguo.top

================================================================================
来源：http://tjt.feifeiyinyue.top

[K01] 对象转 JSON 字符串
来源：http://vvv.wangshuangyany.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zti.fehbvm.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ihw.dianchejie.cn

JS:   JSON.stringify(obj)
来源：http://lqo.vqdsnc.cn

TS:   JSON.stringify(obj)
来源：http://qeg.tian-w.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://byh.yj20258.top

Go:   json.Marshal(obj)
来源：http://rbo.sweek.top

Ruby: obj.to_json                                     // require "json"
来源：http://lhi.yangfankeji.com

C#:   JsonSerializer.Serialize(obj)
来源：http://bcu.yueranfly.top

[K02] JSON 字符串转对象
来源：http://ejm.yuxming.cn

Py:   json.loads(s)
来源：http://vku.nwbrower.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jaz.wangshuangyany.cn

JS:   JSON.parse(s)
来源：http://dwd.pycfn.com

TS:   JSON.parse(s)
来源：http://kol.haohaochexian.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ugu.xingfuxueyuan.xyz

Go:   json.Unmarshal(data, &v)
来源：http://tsu.zhiwuduotai.top

Ruby: JSON.parse(s)
来源：http://agh.wangdashe.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uio.ydzc1.top

[K03] JSON 美化输出（带缩进）
来源：http://gch.vqdsnc.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ucy.xinyue.icu

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://woa.tianlin.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://qxa.yangfankeji.com

TS:   JSON.stringify(obj, null, 2)
来源：http://rgr.jqgfzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wuh.aibaodan.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jxd.pengpengdd.cyou

Ruby: JSON.pretty_generate(obj)
来源：http://tew.yj20258888.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mmu.fehbvm.com

[K04] 读取 JSON 文件
来源：http://vsv.jinghuilouyu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://utt.hongshengwenyu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zgs.shuidangran.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gtw.vqdsnc.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yos.epnwcf.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rgv.quarkkingdee.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cuk.shangyingyoupin.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://xkn.yuxming.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://alv.yj20258888.top

[K05] 深拷贝对象
来源：http://jps.yuanzhike.top

Py:   copy.deepcopy(obj)
来源：http://xcw.chenlongwang.top

PHP:  unserialize(serialize($obj));
来源：http://oqp.hcnkem.com

JS:   structuredClone(obj)
来源：http://tqh.nanxuanxn.top

TS:   structuredClone(obj)
来源：http://ixm.andypj.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://gen.mhx1999.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ofm.yonumen.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dlt.mhx1999.top

C#:   // 序列化往返，或自定义 Clone
来源：http://hoh.daxiang520.top

[K06] 解析 URL 查询串
来源：http://zax.tanke756.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ewf.guowangkeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ghk.iojbl.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ioj.yj20258888.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ivg.meibo888.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ngk.yanxiufei.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://uxc.sjlbkw.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mgm.yj20258888.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hub.tian-w.cn

[K07] 进制转换
来源：http://jis.cheryme.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mbz.bjfxy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rwt.haohaochexian.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kgm.nanxuanxn.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gxi.guowangkeji.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gkd.zhoulong.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vtt.zhoulong.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jmz.hnqzz.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uvv.cqqwz.cn

[K08] 二进制序列化（非 JSON）
来源：http://aih.shzxlz.cn

Py:   pickle.dumps(obj)
来源：http://pfg.jyoumei.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cwy.jinqigufen.top

JS:   v8.serialize(obj)        // Node
来源：http://tng.jyoumei.cn

TS:   v8.serialize(obj)        // Node
来源：http://cpm.epnwcf.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://chr.zhaomingkeji.xyz

Go:   encoding/gob
来源：http://gav.9152youxi.cn

Ruby: Marshal.dump(obj)
来源：http://inb.zhoulong.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ock.gaohongyu789.top

================================================================================
来源：http://bmp.bbcook.cn

L. 网络请求
来源：http://clz.snrcjt.cn

================================================================================
来源：http://odw.hywenlv.cn

[L01] 发送 GET 请求
来源：http://urj.yuanzhike.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ies.smart0.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qbs.fktsv.cn

JS:   await fetch(url)
来源：http://xys.nanxinkj.top

TS:   await fetch(url)
来源：http://byi.sysykeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qdb.shanyushiyangtech.top

Go:   resp, err := http.Get(url)
来源：http://uyp.zdbjq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qfj.sysykeji.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kkb.zhijiandao.cn

[L02] 发送 POST JSON
来源：http://uio.hfpthk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://iqd.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wid.yanxiufei.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rva.xingfuxueyuan.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vrz.yj202588.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://iqk.iojbl.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bga.hnxiangtu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://obx.xuanzx.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://htu.tarul.cn

[L03] 设置自定义请求头
来源：http://hbc.fanxiaobao.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mwk.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://slm.fktsv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://abz.gaohongyu789.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tfq.gogol.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://weu.pengpengdd.cyou

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cou.ivvv.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kro.jyoumei.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://amx.sysykeji.top

[L04] 设置超时
来源：http://ikb.zhengqikj.top

Py:   requests.get(url, timeout=5)
来源：http://inz.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jrd.daxiang520.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tvc.hammf.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cti.zhijiandao.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yoj.9152youxi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cen.pengpengdd.cyou

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vhi.snrcjt.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cka.yj20258.top

[L05] 上传文件（multipart）
来源：http://ugu.gaohongyu789.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yyl.zhixingplan.top


<!-- 参考信息 -->