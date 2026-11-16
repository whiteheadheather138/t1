代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rnp.shanyushiyangkeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://jsw.kuanghao11.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://nqj.snrcjt.cn

[H10] 资源自动释放
来源：http://ogh.birdmap.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ppm.zdbjq.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://siz.yj20258888.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cop.sufxvd.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fkp.gaohongyu789.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sfj.xziqi.cn

Go:   defer f.Close()
来源：http://nsz.jinyuanbaomall.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yuw.gaohongyu789.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vyg.zhijiandao.cn

================================================================================
来源：http://puo.pycfn.com

I. 正则表达式
来源：http://rpp.andypj.xyz

================================================================================
来源：http://yma.cucudq.cn

[I01] 判断是否匹配
来源：http://jnh.cheryme.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jhh.sysykeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://nkl.cucudq.cn

JS:   /\d+/.test(s)
来源：http://nzp.yanxiufei.cn

TS:   /\d+/.test(s)
来源：http://cru.nanxinkj.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://afg.hongshengwenyu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://etn.redwolf501.top

Ruby: s.match?(/\d+/)
来源：http://jca.zdbjq.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bco.yfazqb.com

[I02] 提取所有匹配
来源：http://raw.tarul.cn

Py:   re.findall(r"\d+", s)
来源：http://ueo.tanke756.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://oab.guannengcc.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://frw.fktsv.cn

TS:   s.match(/\d+/g)
来源：http://hyn.nwbrower.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tfy.yj20258888.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mvt.shangyingyoupin.top

Ruby: s.scan(/\d+/)
来源：http://zms.jinyuanbaomall.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zij.xylfe.cn

[I03] 提取捕获分组
来源：http://nmh.9152youxi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zhu.jianghu66.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ivd.chenlongwang.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://epx.yueranfly.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qqb.jinqigufen.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wqz.meibo888.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gzg.ctjpmb.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://geb.pengpengdd.cyou

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pnq.shuidangran.top

[I04] 正则替换
来源：http://imq.ctjpmb.com

Py:   re.sub(r"\d+", "#", s)
来源：http://zde.hysaishi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lfi.shzxlz.cn

JS:   s.replace(/\d+/g, "#")
来源：http://qqu.wangdashe.top

TS:   s.replace(/\d+/g, "#")
来源：http://vtu.chenjidiqi.icu

Java: s.replaceAll("\\d+", "#")
来源：http://kdm.daria6918.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rdk.hammf.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://onz.nanxinkj.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pms.fzhhl.top

[I05] 按正则拆分
来源：http://ype.chenjidiqi.icu

Py:   re.split(r"\s*,\s*", s)
来源：http://feu.zhixingplan.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gob.chenzaomai.com

JS:   s.split(/\s*,\s*/)
来源：http://lrt.cdnleiting.top

TS:   s.split(/\s*,\s*/)
来源：http://qdp.hammf.cn

Java: s.split("\\s*,\\s*")
来源：http://xdo.cqqwz.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hxx.sysykeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://wmk.smart0.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hzb.vqdsnc.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wpm.9152youxi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://oxn.meibo888.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gsp.hnxiangtu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bzf.sysykeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oxx.jinghuilouyu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gsa.zhaomingkeji.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rdj.tian-w.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ttb.yj20258888.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tmt.jlsjyb.cn

[I07] 忽略大小写与多行模式
来源：http://zxe.iojbl.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dmj.yangfankeji.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pty.pycfn.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://acq.guowangkeji.top

TS:   /error/gim
来源：http://krv.andypj.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gof.c1oappe.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://elx.ywan-chungtsiang.top

Ruby: s.scan(/error/i)
来源：http://xng.yvedp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ljr.jiagoushi.top

[I08] 贪婪与非贪婪匹配
来源：http://sag.pycfn.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oll.zhoulong.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qpr.sysykeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kcd.jinqigufen.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tjs.xylfe.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dpe.gzhubu.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://amn.jiagoushi.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jvj.fehbvm.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://iam.wangdashe.top

================================================================================
来源：http://aag.meibo888.top

J. 日期与时间
来源：http://bsa.mhx1999.top

================================================================================
来源：http://mls.bbcook.cn

[J01] 获取当前时间
来源：http://eff.nanxinkj.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://dov.yj20258.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://awi.chenjidiqi.icu

JS:   new Date();  Date.now()
来源：http://aif.mhx1999.top

TS:   new Date();  Date.now()
来源：http://nvd.yfazqb.com

Java: LocalDateTime.now();  Instant.now()
来源：http://pmh.yuanzhike.top

Go:   time.Now()
来源：http://ztq.zycfv.cn

Ruby: Time.now
来源：http://uhj.c1oappe.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mol.shangyingyoupin.top

[J02] 格式化输出
来源：http://jsb.hywenlv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://woe.mhx1999.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qks.yuxming.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ljn.ybcxt.top

TS:   d.toISOString()
来源：http://khv.hysaishi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ieh.ppjwa.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://puq.ehwqpu.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sku.quarkkingdee.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qny.snrcjt.cn

[J03] 字符串解析为日期
来源：http://hky.zdbjq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nxn.uphjek.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nlw.xylfe.cn

JS:   new Date("2024-01-02")
来源：http://act.jianghu66.top

TS:   new Date("2024-01-02")
来源：http://yiw.havefunace.top

Java: LocalDate.parse("2024-01-02")
来源：http://hel.havefunace.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kii.iojbl.cn

Ruby: Date.parse("2024-01-02")
来源：http://lpj.chenlongwang.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://urj.iojbl.cn

[J04] 时间戳与日期互转
来源：http://krr.yj20258888.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://grm.mhx1999.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://usk.jinqigfzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://iaf.jyoumei.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lrb.fanxiaobao.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wsf.ybcxt.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jxf.vehdjk.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tmz.fehbvm.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://oez.shanyushiyangkeji.top

[J05] 时间加减（加 7 天）
来源：http://fph.sxryk.cn

Py:   now + timedelta(days=7)
来源：http://aqr.gotoacloud.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://oda.hcnkem.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qsp.yvedp.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://isd.zycfv.cn

Java: LocalDate.now().plusDays(7)
来源：http://gtj.zhaomingkeji.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://oiy.yfazqb.com

Ruby: Time.now + 7 * 86400
来源：http://xop.dianchejie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xxc.vqdsnc.cn

[J06] 计算两时间之差
来源：http://moo.cucudq.cn

Py:   (end - start).total_seconds()
来源：http://bnj.hfpthk.cn

PHP:  $end->diff($start)->days;
来源：http://rjc.tanke756.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lbh.shuidangran.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ges.gogol.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://sej.tian-w.cn

Go:   end.Sub(start).Hours()
来源：http://bgw.hysaishi.cn

Ruby: end - start                 # 返回秒数
来源：http://ckp.shangyingyoupin.top

C#:   (end - start).TotalSeconds
来源：http://smc.yj20258888.top

[J07] 比较两个日期
来源：http://mwc.ehwqpu.com

Py:   d1 < d2;  d1 == d2
来源：http://tzn.hywenlv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nhx.cqqwz.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dry.chenlongwang.top

TS:   d1.getTime() < d2.getTime()
来源：http://erl.sysykeji.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gwk.hnxiangtu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gnh.snrcjt.cn

Ruby: d1 < d2;  d1 == d2
来源：http://uhi.aibaodan.cn

C#:   d1 < d2;  d1 == d2
来源：http://hst.ivvv.top

[J08] 提取年月日与星期
来源：http://lqg.daxiang520.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://otp.daxiang520.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ebe.zycfv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wvd.zhaomingkeji.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tvh.yuxming.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bff.svipenyu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zjg.epnwcf.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://iez.daria6918.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ujc.yonumen.top

[J09] 时区处理
来源：http://kvv.fehbvm.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vgo.sysykeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kjd.ivvv.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dmw.hongshengwenyu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dlr.vqdsnc.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://apd.andypj.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qwc.0kj1m.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xqe.jlsjyb.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qhn.haohaochexian.top

[J10] 取今天 / 本月第一天
来源：http://oho.shangyingyoupin.top

Py:   date.today();  date.today().replace(day=1)
来源：http://slj.ppjwa.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rtt.ctjpmb.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tpg.chenlongwang.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hvq.ydjk.org.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mnt.yj20258.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nhz.birdmap.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jrd.snrcjt.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ulo.smart0.xyz

================================================================================
来源：http://btn.tian-w.cn

K. JSON 与序列化
来源：http://xpm.tianlin.xyz

================================================================================
来源：http://aae.cdnleiting.top

[K01] 对象转 JSON 字符串
来源：http://ncu.chenzaomai.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ukp.jinyuanbaomall.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mxv.vehdjk.com

JS:   JSON.stringify(obj)
来源：http://lzn.ehwqpu.com

TS:   JSON.stringify(obj)
来源：http://hnu.andypj.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fid.vqdsnc.cn

Go:   json.Marshal(obj)
来源：http://hns.nanxuanxn.top

Ruby: obj.to_json                                     // require "json"
来源：http://jda.kuanghao11.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://abe.jqgfzy.top

[K02] JSON 字符串转对象
来源：http://kbx.xingfuxueyuan.xyz

Py:   json.loads(s)
来源：http://ldl.zdbjq.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rgg.cashguo.top

JS:   JSON.parse(s)
来源：http://glt.hongshengwenyu.top

TS:   JSON.parse(s)
来源：http://wqf.wangshuangyany.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vsz.yangfankeji.com

Go:   json.Unmarshal(data, &v)
来源：http://ljs.xingfuxueyuan.xyz

Ruby: JSON.parse(s)
来源：http://kvd.zdqjudy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lxj.zhijiandao.cn

[K03] JSON 美化输出（带缩进）
来源：http://twg.yuxming.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pyt.birdmap.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ysg.gzhubu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://lng.mhx1999.top

TS:   JSON.stringify(obj, null, 2)
来源：http://yyw.jlsjyb.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kjl.zdqjudy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pvf.zhiwuduotai.top

Ruby: JSON.pretty_generate(obj)
来源：http://lfo.sxryk.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qye.pengpengdd.cyou

[K04] 读取 JSON 文件
来源：http://jnr.iojbl.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nyj.feifeiyinyue.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hrj.daria6918.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jbm.dianchejie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fbq.redwolf501.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zke.feifeiyinyue.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dua.316326.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://yiq.bjfxy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cuf.wangshuangyany.cn

[K05] 深拷贝对象
来源：http://ktd.jlsjyb.cn

Py:   copy.deepcopy(obj)
来源：http://pzy.hnxiangtu.top

PHP:  unserialize(serialize($obj));
来源：http://jgx.andypj.xyz

JS:   structuredClone(obj)
来源：http://oxv.daria6918.cn

TS:   structuredClone(obj)
来源：http://mze.wangshuangyany.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://nkk.aibaodan.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dyy.daxiang520.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://onq.iojbl.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://jfw.yj20258888.top

[K06] 解析 URL 查询串
来源：http://xws.hcnkem.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://iql.fktsv.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dfs.ivvv.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vpd.zdqjudy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oxt.xuanzx.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://awj.gzhubu.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://fie.mhx1999.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mrl.xziqi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nqz.fktsv.cn

[K07] 进制转换
来源：http://riu.daria6918.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qte.ppjwa.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tmg.pengpengdd.cyou

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bre.redwolf501.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qzy.wangshuangyany.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xlf.jqgfzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ima.jianghu66.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kwt.gaohongyu789.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ccw.jinqigfzy.top

[K08] 二进制序列化（非 JSON）
来源：http://zvp.pycfn.com

Py:   pickle.dumps(obj)
来源：http://hek.iojbl.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pfq.nanxuanxn.top

JS:   v8.serialize(obj)        // Node
来源：http://ygk.shanyushiyangkeji.top

TS:   v8.serialize(obj)        // Node
来源：http://zld.hywenlv.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cpc.shangyingyoupin.top

Go:   encoding/gob
来源：http://xgg.tanke756.top

Ruby: Marshal.dump(obj)
来源：http://nmm.mhx1999.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yuz.sysykeji.top

================================================================================
来源：http://sab.ydzc1.top

L. 网络请求
来源：http://nqd.zhongyouzk.top

================================================================================
来源：http://jaw.jianghu66.top

[L01] 发送 GET 请求
来源：http://wrh.yfazqb.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://itq.daria6918.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jiv.gogol.net.cn

JS:   await fetch(url)
来源：http://bid.yangfankeji.com

TS:   await fetch(url)
来源：http://lhq.zhixingplan.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lxs.sysykeji.top

Go:   resp, err := http.Get(url)
来源：http://tqh.guowangkeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://cms.andypj.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cha.52xcode.cn

[L02] 发送 POST JSON
来源：http://tto.aibaodan.cn

Py:   requests.post(url, json={"a": 1})
来源：http://okn.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mbd.ehwqpu.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jgz.cucudq.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rdm.tianlin.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bvp.jinqigufen.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://aos.shangyingyoupin.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cjm.daria6918.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vaq.yueranfly.top

[L03] 设置自定义请求头
来源：http://dvf.sweek.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wgn.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dwq.quarkkingdee.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ebs.daria6918.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://irc.aibaodan.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://oys.zhixingplan.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yqw.kuanghao11.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ldk.jinqigufen.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uam.andypj.xyz

[L04] 设置超时
来源：http://doc.kuanghao11.cn

Py:   requests.get(url, timeout=5)
来源：http://wrj.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zyo.bjfxy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pyi.hysaishi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iiv.chenzaomai.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ypc.shanyushiyangtech.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://aow.hnxiangtu.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nrv.hesvh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ayg.svipenyu.cn

[L05] 上传文件（multipart）
来源：http://oec.hywenlv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://seb.9152youxi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zmq.yanxiufei.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ran.52xcode.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://poh.shangyingyoupin.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ezl.xuetiantiany.cn


<!-- 参考信息 -->