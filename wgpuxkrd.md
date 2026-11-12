代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://guc.shuidangran.top

Ruby: raise MyError.new("fail", 500)
来源：http://hjo.ivvv.top

C#:   // 自定义异常类中加 Code 属性
来源：http://daf.nanxinkj.top

[H10] 资源自动释放
来源：http://vig.sysykeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://dxj.fanxiaobao.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kjh.zdqjudy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vbr.zdqjudy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zrd.shangyingyoupin.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bgo.gotoacloud.top

Go:   defer f.Close()
来源：http://gvn.daxiang520.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://swm.xuanzx.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dgo.hfpthk.cn

================================================================================
来源：http://xco.hywenlv.cn

I. 正则表达式
来源：http://xgu.shuidangran.top

================================================================================
来源：http://qck.chenjidiqi.icu

[I01] 判断是否匹配
来源：http://tkf.fzhhl.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wff.pengpengdd.cyou

PHP:  preg_match('/\d+/', $s);
来源：http://wip.jlsjyb.cn

JS:   /\d+/.test(s)
来源：http://rwl.wangdashe.top

TS:   /\d+/.test(s)
来源：http://toc.hnqzz.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mgi.zycfv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xfa.jyoumei.cn

Ruby: s.match?(/\d+/)
来源：http://sba.aibaodan.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nel.yj20258888.top

[I02] 提取所有匹配
来源：http://wok.zdbjq.cn

Py:   re.findall(r"\d+", s)
来源：http://ynp.xinyue.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gno.jiagoushi.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kro.quarkkingdee.top

TS:   s.match(/\d+/g)
来源：http://mhp.shangyingyoupin.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uda.yangfankeji.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fox.shanyushiyangtech.top

Ruby: s.scan(/\d+/)
来源：http://dta.dashuyun.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uvi.ybcxt.top

[I03] 提取捕获分组
来源：http://zrv.0kj1m.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://umq.hnqzz.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gwv.zhongyouzk.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dhd.snrcjt.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ywq.tianlin.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nut.cucudq.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jqb.ehwqpu.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dhe.ywan-chungtsiang.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ess.shuidangran.top

[I04] 正则替换
来源：http://ubo.c1oappe.top

Py:   re.sub(r"\d+", "#", s)
来源：http://gvi.hammf.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://isk.hnqzz.top

JS:   s.replace(/\d+/g, "#")
来源：http://bfp.jianghu66.top

TS:   s.replace(/\d+/g, "#")
来源：http://bbr.mhx1999.top

Java: s.replaceAll("\\d+", "#")
来源：http://mas.yj202588.top

Go:   re.ReplaceAllString(s, "#")
来源：http://cbq.daxiang520.top

Ruby: s.gsub(/\d+/, "#")
来源：http://pgt.sysykeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://aic.aizwys.cn

[I05] 按正则拆分
来源：http://bmt.jyoumei.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://lxd.tianlin.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://icf.jinqigufen.top

JS:   s.split(/\s*,\s*/)
来源：http://gyw.zycfv.cn

TS:   s.split(/\s*,\s*/)
来源：http://hhr.yj20258.top

Java: s.split("\\s*,\\s*")
来源：http://prt.zhixingplan.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nft.xziqi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dku.jianghu66.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zyd.sweek.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xqd.c1oappe.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zaq.ivvv.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wpb.jqgufenzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kzk.iojbl.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ldo.zhijiandao.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ehl.bbcook.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dnr.daria6918.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xei.haohaochexian.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tvp.zdbjq.cn

[I07] 忽略大小写与多行模式
来源：http://qay.jianghu66.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://afj.sufxvd.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://twf.xuanzx.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tnn.zhengqikj.top

TS:   /error/gim
来源：http://ucf.jlsjyb.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vir.yangfankeji.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://iyu.zhongyouzk.top

Ruby: s.scan(/error/i)
来源：http://dut.mhx1999.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ujd.jinqigufen.top

[I08] 贪婪与非贪婪匹配
来源：http://vzk.quarkkingdee.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cem.fehbvm.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rro.hcnkem.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://oac.yj20258888.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yfh.cdnleiting.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://den.gotoacloud.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wtk.jinqigufen.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://eol.chenlongwang.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fmn.uphjek.com

================================================================================
来源：http://nir.sxryk.cn

J. 日期与时间
来源：http://yat.tarul.cn

================================================================================
来源：http://ldu.guowangkeji.top

[J01] 获取当前时间
来源：http://vey.hfpthk.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://sdx.xuetiantiany.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rev.xinyue.icu

JS:   new Date();  Date.now()
来源：http://hza.fengsongda.top

TS:   new Date();  Date.now()
来源：http://yyq.meibo888.top

Java: LocalDateTime.now();  Instant.now()
来源：http://yfq.svipenyu.cn

Go:   time.Now()
来源：http://lcn.ydjk.org.cn

Ruby: Time.now
来源：http://gps.cashguo.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uub.nwbrower.top

[J02] 格式化输出
来源：http://stf.yanxiufei.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lwh.zhengqikj.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://iyp.chenzaomai.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qqb.yvedp.cn

TS:   d.toISOString()
来源：http://zpo.zhengqikj.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tfh.nanxuanxn.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xkj.xziqi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ipa.smart0.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://isn.9152youxi.cn

[J03] 字符串解析为日期
来源：http://zxj.birdmap.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yud.ydjk.org.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wlj.yj202588.top

JS:   new Date("2024-01-02")
来源：http://utz.shanyushiyangtech.top

TS:   new Date("2024-01-02")
来源：http://tvn.havefunace.top

Java: LocalDate.parse("2024-01-02")
来源：http://cnj.quarkkingdee.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://imd.tian-w.cn

Ruby: Date.parse("2024-01-02")
来源：http://pig.aibaodan.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zbh.iojbl.cn

[J04] 时间戳与日期互转
来源：http://fpk.cdnleiting.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lig.dashuyun.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yqu.yuxming.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gyg.snrcjt.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fke.guowangkeji.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ebq.dianchejie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wob.zhongyouzk.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ygs.haohaochexian.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bve.gogol.net.cn

[J05] 时间加减（加 7 天）
来源：http://yfi.mhx1999.top

Py:   now + timedelta(days=7)
来源：http://djo.shanyushiyangtech.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://sve.havefunace.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gok.fanxiaobao.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vxx.hnxiangtu.top

Java: LocalDate.now().plusDays(7)
来源：http://gid.316326.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nqe.jqgfzy.top

Ruby: Time.now + 7 * 86400
来源：http://qix.ydjk.org.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ylp.ppjwa.cn

[J06] 计算两时间之差
来源：http://kxa.iojbl.cn

Py:   (end - start).total_seconds()
来源：http://euy.hesvh.cn

PHP:  $end->diff($start)->days;
来源：http://yso.fanxiaobao.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vxy.0kj1m.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vpz.zhijiandao.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xjx.shzxlz.cn

Go:   end.Sub(start).Hours()
来源：http://czy.yonumen.top

Ruby: end - start                 # 返回秒数
来源：http://ppw.svipenyu.cn

C#:   (end - start).TotalSeconds
来源：http://onc.jyoumei.cn

[J07] 比较两个日期
来源：http://xua.zhoulong.xyz

Py:   d1 < d2;  d1 == d2
来源：http://nzy.shzxlz.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wlc.jqgfzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://hlf.ywan-chungtsiang.top

TS:   d1.getTime() < d2.getTime()
来源：http://esi.yfazqb.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nfr.jianghu66.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bpf.yangfankeji.com

Ruby: d1 < d2;  d1 == d2
来源：http://hle.bjfxy.top

C#:   d1 < d2;  d1 == d2
来源：http://uxy.yuxming.cn

[J08] 提取年月日与星期
来源：http://syb.nanxuanxn.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rvb.birdmap.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bkk.hnqzz.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zsc.jyoumei.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ymp.ywan-chungtsiang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://inm.xingfuxueyuan.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ohb.yangfankeji.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rsy.guowangkeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hhk.zhiwuduotai.top

[J09] 时区处理
来源：http://mky.gaohongyu789.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kvx.zhaomingkeji.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mts.xingfuxueyuan.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nuf.gaohongyu789.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tkv.hongshengwenyu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://doa.uphjek.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vsh.guannengcc.top

Ruby: Time.now.getlocal("+08:00")
来源：http://mhq.zhiwuduotai.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cbu.xinyue.icu

[J10] 取今天 / 本月第一天
来源：http://xju.c1oappe.top

Py:   date.today();  date.today().replace(day=1)
来源：http://gvg.redwolf501.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://apz.shuidangran.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://did.yonumen.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cuq.sysykeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yyq.zhengqikj.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qqk.jinghuilouyu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dka.9152youxi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hqh.hfpthk.cn

================================================================================
来源：http://jva.cucudq.cn

K. JSON 与序列化
来源：http://abl.hysaishi.cn

================================================================================
来源：http://faq.shanyushiyangkeji.top

[K01] 对象转 JSON 字符串
来源：http://veq.haohaochexian.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fes.hcnkem.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xcv.zhixingplan.top

JS:   JSON.stringify(obj)
来源：http://cvm.0kj1m.cn

TS:   JSON.stringify(obj)
来源：http://obd.jinqigfzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bqj.shzxlz.cn

Go:   json.Marshal(obj)
来源：http://azf.zhaomingkeji.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://adg.snrcjt.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wji.cashguo.top

[K02] JSON 字符串转对象
来源：http://tch.c1oappe.top

Py:   json.loads(s)
来源：http://dxe.yfazqb.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ccy.dianchejie.cn

JS:   JSON.parse(s)
来源：http://grm.nanxinkj.top

TS:   JSON.parse(s)
来源：http://soi.meibo888.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nlc.xinyue.icu

Go:   json.Unmarshal(data, &v)
来源：http://etw.chenlongwang.top

Ruby: JSON.parse(s)
来源：http://kcf.zhiwuduotai.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://quy.yj20258888.top

[K03] JSON 美化输出（带缩进）
来源：http://baa.hesvh.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wkh.9152youxi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ber.wangshuangyany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://adw.zdbjq.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yhf.ehwqpu.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wku.tanke756.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ape.xinyue.icu

Ruby: JSON.pretty_generate(obj)
来源：http://xio.cashguo.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kce.xuetiantiany.cn

[K04] 读取 JSON 文件
来源：http://xqh.yonumen.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uqn.xziqi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://agc.pycfn.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://muz.sweek.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dti.hysaishi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://aic.yueranfly.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qhp.yangfankeji.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://jkv.yuxming.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tkc.nwbrower.top

[K05] 深拷贝对象
来源：http://zzk.jqgfzy.top

Py:   copy.deepcopy(obj)
来源：http://iuc.nwbrower.top

PHP:  unserialize(serialize($obj));
来源：http://vmd.fzhhl.top

JS:   structuredClone(obj)
来源：http://ykd.cdnleiting.top

TS:   structuredClone(obj)
来源：http://smz.sufxvd.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://omn.yj20258888.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lnu.ywan-chungtsiang.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vba.52xcode.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tdu.ywan-chungtsiang.top

[K06] 解析 URL 查询串
来源：http://ush.vqdsnc.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://btg.mhx1999.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dcl.yongpay.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rtj.mhx1999.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fbk.52xcode.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ijx.ivvv.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://bsm.havefunace.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://abq.zhiwuduotai.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://spe.jinqigufen.top

[K07] 进制转换
来源：http://fuq.kuanghao11.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qzf.yongpay.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bpx.shzxlz.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bml.ctjpmb.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://byo.hnxiangtu.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rrt.hfpthk.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://itk.shuidangran.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zjp.aibaodan.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://slx.ppjwa.cn

[K08] 二进制序列化（非 JSON）
来源：http://vah.shzxlz.cn

Py:   pickle.dumps(obj)
来源：http://xik.jinqigufen.top

PHP:  serialize($obj);  unserialize($s);
来源：http://vpy.yfazqb.com

JS:   v8.serialize(obj)        // Node
来源：http://osr.cheryme.top

TS:   v8.serialize(obj)        // Node
来源：http://blc.hnqzz.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zlv.hnqzz.top

Go:   encoding/gob
来源：http://odu.chenzaomai.com

Ruby: Marshal.dump(obj)
来源：http://ofi.hammf.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yxe.yongpay.top

================================================================================
来源：http://sag.meibo888.top

L. 网络请求
来源：http://jag.meibo888.top

================================================================================
来源：http://ppi.hammf.cn

[L01] 发送 GET 请求
来源：http://ubf.9152youxi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xjy.hammf.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wda.ydjk.org.cn

JS:   await fetch(url)
来源：http://coi.sxryk.cn

TS:   await fetch(url)
来源：http://yfl.daxiang520.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ykx.sweek.top

Go:   resp, err := http.Get(url)
来源：http://ekn.yuxming.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hou.sufxvd.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mdu.vehdjk.com

[L02] 发送 POST JSON
来源：http://hhw.fehbvm.com

Py:   requests.post(url, json={"a": 1})
来源：http://ywq.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dmo.dashuyun.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://adz.tian-w.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kaj.ydzc1.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vrj.ivvv.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pfj.hysaishi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xnc.iojbl.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ibv.aizwys.cn

[L03] 设置自定义请求头
来源：http://fhp.shuidangran.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mrh.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vbm.zhongyouzk.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jhu.jinyuanbaomall.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ags.tanke756.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bmk.vqdsnc.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pbr.ctjpmb.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ivs.zhaomingkeji.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xlw.zhengqikj.top

[L04] 设置超时
来源：http://mpf.snrcjt.cn

Py:   requests.get(url, timeout=5)
来源：http://isu.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zro.ydjk.org.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ezw.aibaodan.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zea.mhx1999.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://noe.svipenyu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hud.tarul.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ulm.gotoacloud.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lpa.hysaishi.cn

[L05] 上传文件（multipart）
来源：http://sxg.sysykeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sfd.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://feb.snrcjt.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sro.hnqzz.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jij.uphjek.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ztd.hfpthk.cn


<!-- 参考信息 -->