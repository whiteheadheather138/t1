代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://ilj.chenlongwang.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dtl.jinqigfzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fri.316326.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xxk.yangfankeji.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gpm.jiagoushi.top

Ruby: raise MyError.new("fail", 500)
来源：http://edf.zhengqikj.top

C#:   // 自定义异常类中加 Code 属性
来源：http://zhp.jinghuilouyu.cn

[H10] 资源自动释放
来源：http://kmq.yvedp.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://luf.hywenlv.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jch.feifeiyinyue.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tjg.52xcode.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yvo.ppjwa.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uwy.zhijiandao.cn

Go:   defer f.Close()
来源：http://vzh.zhoulong.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://azs.tianlin.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://foi.ppjwa.cn

================================================================================
来源：http://wnq.uphjek.com

I. 正则表达式
来源：http://xdy.yuanzhike.top

================================================================================
来源：http://phs.yuxming.cn

[I01] 判断是否匹配
来源：http://gpz.bjfxy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://czy.cqqwz.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zjh.cqqwz.cn

JS:   /\d+/.test(s)
来源：http://ber.meibo888.top

TS:   /\d+/.test(s)
来源：http://saz.tian-w.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://trk.jinghuilouyu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gwp.sweek.top

Ruby: s.match?(/\d+/)
来源：http://lru.chenlongwang.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hiv.gzhubu.top

[I02] 提取所有匹配
来源：http://plc.chenlongwang.top

Py:   re.findall(r"\d+", s)
来源：http://irw.havefunace.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yqs.haohaochexian.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fta.cqqwz.cn

TS:   s.match(/\d+/g)
来源：http://udj.ppjwa.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cww.feifeiyinyue.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gti.jiagoushi.top

Ruby: s.scan(/\d+/)
来源：http://kor.jinyuanbaomall.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nwq.yfazqb.com

[I03] 提取捕获分组
来源：http://eqp.smart0.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://izg.feifeiyinyue.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pfw.zhoulong.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cby.zhongyouzk.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gpg.ctjpmb.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jxy.cqqwz.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fir.yj20258.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rsy.vqdsnc.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ykw.jqgfzy.top

[I04] 正则替换
来源：http://dzz.xylfe.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://grd.chenzaomai.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://aza.jianghu66.top

JS:   s.replace(/\d+/g, "#")
来源：http://jmu.ydzc1.top

TS:   s.replace(/\d+/g, "#")
来源：http://hdp.fzhhl.top

Java: s.replaceAll("\\d+", "#")
来源：http://kah.c1oappe.top

Go:   re.ReplaceAllString(s, "#")
来源：http://msl.yongpay.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ede.jinqigfzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vfl.hnqzz.top

[I05] 按正则拆分
来源：http://yqf.nanxuanxn.top

Py:   re.split(r"\s*,\s*", s)
来源：http://uhf.xuanzx.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pky.fzhhl.top

JS:   s.split(/\s*,\s*/)
来源：http://ulb.shuidangran.top

TS:   s.split(/\s*,\s*/)
来源：http://kul.zdqjudy.top

Java: s.split("\\s*,\\s*")
来源：http://zbp.xylfe.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yrz.gogol.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://cch.sysykeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ceg.iojbl.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dmw.mhx1999.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bbx.9152youxi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://crr.yuxming.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mne.aizwys.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ntg.pycfn.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gdk.nwbrower.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qtg.svipenyu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://emq.hesvh.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wlk.cdnleiting.top

[I07] 忽略大小写与多行模式
来源：http://dab.gaohongyu789.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bef.gzhubu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tlc.haohaochexian.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oat.shuidangran.top

TS:   /error/gim
来源：http://jet.bjfxy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://edn.bbcook.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://slr.zhoulong.xyz

Ruby: s.scan(/error/i)
来源：http://dpx.xinyue.icu

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wft.yueranfly.top

[I08] 贪婪与非贪婪匹配
来源：http://wln.aibaodan.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zih.shanyushiyangtech.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cmv.sweek.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://las.dianchejie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fdi.zycfv.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bpc.xuanzx.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dbc.yanxiufei.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gbr.hongshengwenyu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cbe.ctjpmb.com

================================================================================
来源：http://viy.wangshuangyany.cn

J. 日期与时间
来源：http://yxo.ybcxt.top

================================================================================
来源：http://jew.daxiang520.top

[J01] 获取当前时间
来源：http://bvy.316326.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://ywf.hesvh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://igb.shangyingyoupin.top

JS:   new Date();  Date.now()
来源：http://jcx.zhoulong.xyz

TS:   new Date();  Date.now()
来源：http://bke.snrcjt.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://exg.yangfankeji.com

Go:   time.Now()
来源：http://ijj.yj20258888.top

Ruby: Time.now
来源：http://qah.ctjpmb.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ybl.jiagoushi.top

[J02] 格式化输出
来源：http://tbg.bbcook.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mvq.yj202588.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tms.ppjwa.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fhb.shanyushiyangkeji.top

TS:   d.toISOString()
来源：http://szk.hammf.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zja.aizwys.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qfy.yvedp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://flt.yongpay.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hkk.aibaodan.cn

[J03] 字符串解析为日期
来源：http://vas.hesvh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://flu.tarul.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hey.wangshuangyany.cn

JS:   new Date("2024-01-02")
来源：http://ens.hysaishi.cn

TS:   new Date("2024-01-02")
来源：http://thd.cashguo.top

Java: LocalDate.parse("2024-01-02")
来源：http://wdl.xingfuxueyuan.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mbi.ydzc1.top

Ruby: Date.parse("2024-01-02")
来源：http://cgf.jinghuilouyu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bor.daria6918.cn

[J04] 时间戳与日期互转
来源：http://bex.chenjidiqi.icu

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://low.uphjek.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://koz.fengsongda.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://php.hammf.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dvc.yvedp.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fzx.snrcjt.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vxi.hnqzz.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://axq.jqgufenzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ugt.sysykeji.top

[J05] 时间加减（加 7 天）
来源：http://gyv.zhengqikj.top

Py:   now + timedelta(days=7)
来源：http://fyr.uphjek.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://uco.tian-w.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ong.dashuyun.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ybz.hywenlv.cn

Java: LocalDate.now().plusDays(7)
来源：http://esw.jlsjyb.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bcs.fengsongda.top

Ruby: Time.now + 7 * 86400
来源：http://ubh.pycfn.com

C#:   DateTime.Now.AddDays(7)
来源：http://hjy.9152youxi.cn

[J06] 计算两时间之差
来源：http://wng.yuanzhike.top

Py:   (end - start).total_seconds()
来源：http://jhg.sufxvd.cn

PHP:  $end->diff($start)->days;
来源：http://ajk.jinqigufen.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ghj.zycfv.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gvt.cucudq.cn

Java: Duration.between(start, end).toSeconds()
来源：http://tqj.xuanzx.com

Go:   end.Sub(start).Hours()
来源：http://fni.jinghuilouyu.cn

Ruby: end - start                 # 返回秒数
来源：http://hue.c1oappe.top

C#:   (end - start).TotalSeconds
来源：http://lzw.kuanghao11.cn

[J07] 比较两个日期
来源：http://mrk.daria6918.cn

Py:   d1 < d2;  d1 == d2
来源：http://qmu.hnxiangtu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://osb.jinqigufen.top

JS:   d1.getTime() < d2.getTime()
来源：http://gky.fanxiaobao.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://xkf.sufxvd.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zid.zhiwuduotai.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://szb.tanke756.top

Ruby: d1 < d2;  d1 == d2
来源：http://fuf.c1oappe.top

C#:   d1 < d2;  d1 == d2
来源：http://uyp.zycfv.cn

[J08] 提取年月日与星期
来源：http://eic.ybcxt.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sxi.hfpthk.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cna.zhijiandao.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pfn.ywan-chungtsiang.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://iaf.zhongyouzk.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gqz.dianchejie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hfa.uphjek.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lax.yfazqb.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gpm.aibaodan.cn

[J09] 时区处理
来源：http://tdw.zhaomingkeji.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rxq.hammf.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gym.shuidangran.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jtu.chenjidiqi.icu

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://htk.xingfuxueyuan.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bbc.quarkkingdee.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ujq.chenlongwang.top

Ruby: Time.now.getlocal("+08:00")
来源：http://mse.shanyushiyangkeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://iwx.zhiwuduotai.top

[J10] 取今天 / 本月第一天
来源：http://hlw.yangfankeji.com

Py:   date.today();  date.today().replace(day=1)
来源：http://xth.xuanzx.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ulw.hammf.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pjn.jqgufenzy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://emv.smart0.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://stc.wangshuangyany.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ivw.hongshengwenyu.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ppb.bbcook.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tby.c1oappe.top

================================================================================
来源：http://mtk.sufxvd.cn

K. JSON 与序列化
来源：http://axl.gogol.net.cn

================================================================================
来源：http://vnx.tian-w.cn

[K01] 对象转 JSON 字符串
来源：http://rwr.uphjek.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xek.yueranfly.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zsn.0kj1m.cn

JS:   JSON.stringify(obj)
来源：http://rrn.bjfxy.top

TS:   JSON.stringify(obj)
来源：http://ijg.mhx1999.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bqj.zhijiandao.cn

Go:   json.Marshal(obj)
来源：http://ewt.wangdashe.top

Ruby: obj.to_json                                     // require "json"
来源：http://nyi.yueranfly.top

C#:   JsonSerializer.Serialize(obj)
来源：http://hyl.epnwcf.com

[K02] JSON 字符串转对象
来源：http://tiv.uphjek.com

Py:   json.loads(s)
来源：http://pkb.sufxvd.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nxz.ivvv.top

JS:   JSON.parse(s)
来源：http://rjo.jqgufenzy.top

TS:   JSON.parse(s)
来源：http://gcb.chenjidiqi.icu

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mst.pengpengdd.cyou

Go:   json.Unmarshal(data, &v)
来源：http://krw.aibaodan.cn

Ruby: JSON.parse(s)
来源：http://ntb.dianchejie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fwp.jqgfzy.top

[K03] JSON 美化输出（带缩进）
来源：http://yeg.smart0.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://moo.gogol.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rqk.ppjwa.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jin.mhx1999.top

TS:   JSON.stringify(obj, null, 2)
来源：http://jmv.fktsv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ykn.hesvh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://diq.xylfe.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nto.sxryk.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://okk.hnqzz.top

[K04] 读取 JSON 文件
来源：http://swh.guowangkeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wth.hnxiangtu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://stb.0kj1m.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hzu.shanyushiyangkeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lvz.yj20258888.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ubi.yonumen.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://obj.shzxlz.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hyi.aizwys.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tkd.jiagoushi.top

[K05] 深拷贝对象
来源：http://zxd.guowangkeji.top

Py:   copy.deepcopy(obj)
来源：http://cdp.sysykeji.top

PHP:  unserialize(serialize($obj));
来源：http://opx.xylfe.cn

JS:   structuredClone(obj)
来源：http://hhz.fanxiaobao.xyz

TS:   structuredClone(obj)
来源：http://mrl.nanxinkj.top

Java: // 手写拷贝构造，或序列化往返
来源：http://oaa.chenlongwang.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hlw.yj20258888.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://aju.shangyingyoupin.top

C#:   // 序列化往返，或自定义 Clone
来源：http://otj.yj20258.top

[K06] 解析 URL 查询串
来源：http://qsc.yvedp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zcr.guannengcc.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qef.xziqi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ggh.yueranfly.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iwu.yuxming.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dmk.hammf.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ugm.daxiang520.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tlf.sufxvd.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://owr.tanke756.top

[K07] 进制转换
来源：http://xls.316326.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ihn.chenzaomai.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wjw.tian-w.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gls.yongpay.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ciy.jqgfzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mhd.fktsv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://efa.dashuyun.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yzj.fzhhl.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ooz.xziqi.cn

[K08] 二进制序列化（非 JSON）
来源：http://eow.xuetiantiany.cn

Py:   pickle.dumps(obj)
来源：http://lhv.snrcjt.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ouz.hammf.cn

JS:   v8.serialize(obj)        // Node
来源：http://mzg.c1oappe.top

TS:   v8.serialize(obj)        // Node
来源：http://ouc.yj20258888.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qto.pengpengdd.cyou

Go:   encoding/gob
来源：http://kpw.shanyushiyangtech.top

Ruby: Marshal.dump(obj)
来源：http://cmj.guannengcc.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rcg.guannengcc.top

================================================================================
来源：http://fuv.yongpay.top

L. 网络请求
来源：http://zzy.fengsongda.top

================================================================================
来源：http://ywi.hongshengwenyu.top

[L01] 发送 GET 请求
来源：http://xlu.fanxiaobao.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ssj.yfazqb.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uts.jinqigufen.top

JS:   await fetch(url)
来源：http://bit.hnxiangtu.top

TS:   await fetch(url)
来源：http://sig.ydzc1.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ssw.vqdsnc.cn

Go:   resp, err := http.Get(url)
来源：http://oca.tianlin.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://gfp.pengpengdd.cyou

C#:   await new HttpClient().GetStringAsync(url)
来源：http://aff.zhiwuduotai.top

[L02] 发送 POST JSON
来源：http://cps.ctjpmb.com

Py:   requests.post(url, json={"a": 1})
来源：http://tjx.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://num.jinyuanbaomall.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://plg.sweek.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zgn.ppjwa.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uxl.zhaomingkeji.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jvr.gzhubu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zgk.sweek.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://njz.guannengcc.top

[L03] 设置自定义请求头
来源：http://dhw.bbcook.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ndd.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fxd.yj20258888.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yci.zycfv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gaf.sufxvd.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zvb.ctjpmb.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nhr.guowangkeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bqp.sufxvd.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vpc.yuxming.cn

[L04] 设置超时
来源：http://zqm.fanxiaobao.xyz

Py:   requests.get(url, timeout=5)
来源：http://gje.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cjl.tanke756.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rsf.tian-w.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ygz.ydjk.org.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ucr.jinqigfzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fuh.iojbl.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yuo.shanyushiyangtech.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sio.yfazqb.com

[L05] 上传文件（multipart）
来源：http://qjf.xuanzx.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bfd.yuanzhike.top


<!-- 参考信息 -->