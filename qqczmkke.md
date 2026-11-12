代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://vjp.meibo888.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://eii.yfazqb.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wjp.yangfankeji.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nyn.nwbrower.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pgg.cheryme.top

Ruby: raise MyError.new("fail", 500)
来源：http://daw.nanxinkj.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ubn.yuxming.cn

[H10] 资源自动释放
来源：http://fmq.hcnkem.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://tjq.zhongyouzk.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yae.jinqigfzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fmw.yfazqb.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bxw.yj202588.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xly.feifeiyinyue.top

Go:   defer f.Close()
来源：http://fjh.jiagoushi.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mnr.jqgufenzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jln.gaohongyu789.top

================================================================================
来源：http://clj.ydzc1.top

I. 正则表达式
来源：http://qrg.gaohongyu789.top

================================================================================
来源：http://ozb.nanxinkj.top

[I01] 判断是否匹配
来源：http://uke.uphjek.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ewd.sweek.top

PHP:  preg_match('/\d+/', $s);
来源：http://ono.zhongyouzk.top

JS:   /\d+/.test(s)
来源：http://iqt.gaohongyu789.top

TS:   /\d+/.test(s)
来源：http://wvq.bjfxy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xqu.jqgufenzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://iqw.jinghuilouyu.cn

Ruby: s.match?(/\d+/)
来源：http://ycj.xuetiantiany.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dop.shzxlz.cn

[I02] 提取所有匹配
来源：http://kto.bjfxy.top

Py:   re.findall(r"\d+", s)
来源：http://ifp.fengsongda.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sby.aibaodan.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vwl.gogol.net.cn

TS:   s.match(/\d+/g)
来源：http://sat.shanyushiyangtech.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qik.yueranfly.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gpz.hysaishi.cn

Ruby: s.scan(/\d+/)
来源：http://gnj.jianghu66.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sac.hesvh.cn

[I03] 提取捕获分组
来源：http://szz.jianghu66.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bmn.cqqwz.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ejz.daxiang520.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://eau.guannengcc.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fqr.chenjidiqi.icu

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tsh.ehwqpu.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fro.jlsjyb.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bsu.xuanzx.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jps.zhengqikj.top

[I04] 正则替换
来源：http://cte.sweek.top

Py:   re.sub(r"\d+", "#", s)
来源：http://bit.ybcxt.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cru.hcnkem.com

JS:   s.replace(/\d+/g, "#")
来源：http://aiy.wangdashe.top

TS:   s.replace(/\d+/g, "#")
来源：http://qfn.xziqi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vzc.svipenyu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://mob.gaohongyu789.top

Ruby: s.gsub(/\d+/, "#")
来源：http://boy.hammf.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wcz.tianlin.xyz

[I05] 按正则拆分
来源：http://rnt.hnxiangtu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://yvn.hnqzz.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://grc.dashuyun.cn

JS:   s.split(/\s*,\s*/)
来源：http://fgh.guowangkeji.top

TS:   s.split(/\s*,\s*/)
来源：http://qbp.yj20258888.top

Java: s.split("\\s*,\\s*")
来源：http://kxl.haohaochexian.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jce.wangshuangyany.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pjj.zycfv.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sqv.zhiwuduotai.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://imc.sweek.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qfz.birdmap.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wwt.dianchejie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hdb.guannengcc.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gxe.ppjwa.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pts.daxiang520.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gab.dianchejie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://axx.zdbjq.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cnp.mhx1999.top

[I07] 忽略大小写与多行模式
来源：http://owp.fengsongda.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cyo.shanyushiyangtech.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qkj.ppjwa.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qpi.tarul.cn

TS:   /error/gim
来源：http://ams.hongshengwenyu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vcd.zhiwuduotai.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://itm.cucudq.cn

Ruby: s.scan(/error/i)
来源：http://tts.yuxming.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gnn.meibo888.top

[I08] 贪婪与非贪婪匹配
来源：http://qhx.jqgufenzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ntz.jlsjyb.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kem.tarul.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lyh.yuanzhike.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cpt.hammf.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://feq.hywenlv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ezw.shzxlz.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ezm.feifeiyinyue.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sxu.gotoacloud.top

================================================================================
来源：http://wpl.zhixingplan.top

J. 日期与时间
来源：http://qze.zhiwuduotai.top

================================================================================
来源：http://mql.epnwcf.com

[J01] 获取当前时间
来源：http://dnt.xinyue.icu

Py:   datetime.now();  datetime.now(UTC)
来源：http://qyh.fehbvm.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vei.fengsongda.top

JS:   new Date();  Date.now()
来源：http://afb.zycfv.cn

TS:   new Date();  Date.now()
来源：http://vcu.yongpay.top

Java: LocalDateTime.now();  Instant.now()
来源：http://kow.hcnkem.com

Go:   time.Now()
来源：http://wfw.zhijiandao.cn

Ruby: Time.now
来源：http://inu.yanxiufei.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fsb.quarkkingdee.top

[J02] 格式化输出
来源：http://nbo.hfpthk.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bci.ehwqpu.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xhd.52xcode.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dwp.zhongyouzk.top

TS:   d.toISOString()
来源：http://ktr.fehbvm.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fux.svipenyu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bvw.daxiang520.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ycm.havefunace.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://skb.shanyushiyangtech.top

[J03] 字符串解析为日期
来源：http://qnd.snrcjt.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qyr.316326.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lgn.iojbl.cn

JS:   new Date("2024-01-02")
来源：http://xlp.mhx1999.top

TS:   new Date("2024-01-02")
来源：http://yde.yonumen.top

Java: LocalDate.parse("2024-01-02")
来源：http://hhh.zdqjudy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dqq.gaohongyu789.top

Ruby: Date.parse("2024-01-02")
来源：http://yha.fehbvm.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rpv.dashuyun.cn

[J04] 时间戳与日期互转
来源：http://jnv.sufxvd.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ivz.zdbjq.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kzm.jinghuilouyu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hxf.yanxiufei.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tzm.bbcook.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://msh.nanxuanxn.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pqh.yonumen.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pik.wangdashe.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mki.nanxinkj.top

[J05] 时间加减（加 7 天）
来源：http://zwi.fktsv.cn

Py:   now + timedelta(days=7)
来源：http://ysv.gaohongyu789.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://riq.bbcook.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dca.jqgufenzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wvi.redwolf501.top

Java: LocalDate.now().plusDays(7)
来源：http://ogn.daxiang520.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nqx.zycfv.cn

Ruby: Time.now + 7 * 86400
来源：http://ddb.kuanghao11.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vnx.hywenlv.cn

[J06] 计算两时间之差
来源：http://unz.jlsjyb.cn

Py:   (end - start).total_seconds()
来源：http://wig.ydjk.org.cn

PHP:  $end->diff($start)->days;
来源：http://iix.xuetiantiany.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tvb.hnqzz.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://twp.shzxlz.cn

Java: Duration.between(start, end).toSeconds()
来源：http://erl.zhengqikj.top

Go:   end.Sub(start).Hours()
来源：http://dza.havefunace.top

Ruby: end - start                 # 返回秒数
来源：http://qvk.gogol.net.cn

C#:   (end - start).TotalSeconds
来源：http://hou.bbcook.cn

[J07] 比较两个日期
来源：http://wdi.wangshuangyany.cn

Py:   d1 < d2;  d1 == d2
来源：http://whb.ydjk.org.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xec.redwolf501.top

JS:   d1.getTime() < d2.getTime()
来源：http://kbc.tarul.cn

TS:   d1.getTime() < d2.getTime()
来源：http://cmg.tianlin.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cxm.bjfxy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nic.cashguo.top

Ruby: d1 < d2;  d1 == d2
来源：http://dxs.haohaochexian.top

C#:   d1 < d2;  d1 == d2
来源：http://ojd.fehbvm.com

[J08] 提取年月日与星期
来源：http://hlz.daria6918.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ojr.tian-w.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qie.yuanzhike.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ois.jlsjyb.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sgq.yanxiufei.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tgt.cucudq.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kug.fengsongda.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dyc.tianlin.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://idv.wangdashe.top

[J09] 时区处理
来源：http://gcq.meibo888.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vws.hysaishi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cjp.chenzaomai.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mun.chenzaomai.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://adt.vqdsnc.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kde.hcnkem.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xrk.kuanghao11.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://kyu.feifeiyinyue.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cye.jinghuilouyu.cn

[J10] 取今天 / 本月第一天
来源：http://viz.guannengcc.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ojs.c1oappe.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://erf.yuxming.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://evv.vqdsnc.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dek.ehwqpu.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://okg.quarkkingdee.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://udi.sxryk.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nda.xuetiantiany.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wnk.shangyingyoupin.top

================================================================================
来源：http://jls.yanxiufei.cn

K. JSON 与序列化
来源：http://fgw.yanxiufei.cn

================================================================================
来源：http://itq.yj20258.top

[K01] 对象转 JSON 字符串
来源：http://ngd.jinqigufen.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hip.guowangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://evb.cashguo.top

JS:   JSON.stringify(obj)
来源：http://kbr.zhengqikj.top

TS:   JSON.stringify(obj)
来源：http://akw.ydzc1.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bzz.vqdsnc.cn

Go:   json.Marshal(obj)
来源：http://bdg.tarul.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fud.52xcode.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zvt.mhx1999.top

[K02] JSON 字符串转对象
来源：http://vei.gotoacloud.top

Py:   json.loads(s)
来源：http://dia.jinqigfzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sro.nanxuanxn.top

JS:   JSON.parse(s)
来源：http://wpw.cheryme.top

TS:   JSON.parse(s)
来源：http://afo.yonumen.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://djy.gaohongyu789.top

Go:   json.Unmarshal(data, &v)
来源：http://idi.xingfuxueyuan.xyz

Ruby: JSON.parse(s)
来源：http://wtz.svipenyu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ocp.jlsjyb.cn

[K03] JSON 美化输出（带缩进）
来源：http://han.sweek.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://maz.chenjidiqi.icu

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wgl.cqqwz.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qpw.fzhhl.top

TS:   JSON.stringify(obj, null, 2)
来源：http://elh.zhiwuduotai.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ovh.nwbrower.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mzx.hesvh.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kil.ivvv.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gtv.ivvv.top

[K04] 读取 JSON 文件
来源：http://wis.hcnkem.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sve.guannengcc.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gan.fengsongda.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://alf.xziqi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lku.hnqzz.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://huu.birdmap.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xfi.bjfxy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ggf.havefunace.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cly.316326.xyz

[K05] 深拷贝对象
来源：http://iys.meibo888.top

Py:   copy.deepcopy(obj)
来源：http://rqk.snrcjt.cn

PHP:  unserialize(serialize($obj));
来源：http://lsv.hesvh.cn

JS:   structuredClone(obj)
来源：http://bgm.sxryk.cn

TS:   structuredClone(obj)
来源：http://one.feifeiyinyue.top

Java: // 手写拷贝构造，或序列化往返
来源：http://poy.ydjk.org.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://upo.yanxiufei.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ujh.ppjwa.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://eip.ehwqpu.com

[K06] 解析 URL 查询串
来源：http://wcu.cqqwz.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qhp.jinqigfzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://slh.yuanzhike.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ezs.haohaochexian.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ifu.jinyuanbaomall.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://chl.birdmap.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://sgk.fktsv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mmo.xylfe.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://iyi.yueranfly.top

[K07] 进制转换
来源：http://zeg.yuanzhike.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lsr.fengsongda.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jep.hammf.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yub.hfpthk.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mko.316326.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qyz.guannengcc.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://trj.xziqi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fzu.zhongyouzk.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ouw.yfazqb.com

[K08] 二进制序列化（非 JSON）
来源：http://bkn.vqdsnc.cn

Py:   pickle.dumps(obj)
来源：http://tik.zdqjudy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://mdw.zhoulong.xyz

JS:   v8.serialize(obj)        // Node
来源：http://cuu.haohaochexian.top

TS:   v8.serialize(obj)        // Node
来源：http://bjh.cucudq.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hhg.yj202588.top

Go:   encoding/gob
来源：http://lbm.hnqzz.top

Ruby: Marshal.dump(obj)
来源：http://fyx.zhijiandao.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://oyh.jinghuilouyu.cn

================================================================================
来源：http://yyo.jlsjyb.cn

L. 网络请求
来源：http://klp.yfazqb.com

================================================================================
来源：http://wbi.zhaomingkeji.xyz

[L01] 发送 GET 请求
来源：http://uxf.yvedp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://skg.feifeiyinyue.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uhq.c1oappe.top

JS:   await fetch(url)
来源：http://ekn.gotoacloud.top

TS:   await fetch(url)
来源：http://dvq.iojbl.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://scv.haohaochexian.top

Go:   resp, err := http.Get(url)
来源：http://lgj.xingfuxueyuan.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://hgx.zhengqikj.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hwb.vehdjk.com

[L02] 发送 POST JSON
来源：http://fya.hcnkem.com

Py:   requests.post(url, json={"a": 1})
来源：http://aei.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qee.uphjek.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wiy.ywan-chungtsiang.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cjd.yuxming.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://crj.9152youxi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://keh.fktsv.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://eti.bbcook.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dnv.c1oappe.top

[L03] 设置自定义请求头
来源：http://ris.0kj1m.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gpd.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bgm.yonumen.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sqm.epnwcf.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://asq.jyoumei.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lnt.chenlongwang.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uee.xuetiantiany.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mft.ydjk.org.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pxl.ctjpmb.com

[L04] 设置超时
来源：http://zha.jqgfzy.top

Py:   requests.get(url, timeout=5)
来源：http://wws.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kgc.sxryk.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sec.gotoacloud.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ewg.kuanghao11.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rsg.0kj1m.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mwr.52xcode.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lgk.smart0.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hfk.jyoumei.cn

[L05] 上传文件（multipart）
来源：http://wie.shuidangran.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pdg.cucudq.cn


<!-- 参考信息 -->