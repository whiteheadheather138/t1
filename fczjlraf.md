代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pmp.yonumen.top

Ruby: raise MyError.new("fail", 500)
来源：http://imc.zdqjudy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://owh.yuanzhike.top

[H10] 资源自动释放
来源：http://mco.52xcode.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://mog.chenzaomai.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uby.zhaomingkeji.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lan.hfpthk.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xso.jinqigfzy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yxe.uphjek.com

Go:   defer f.Close()
来源：http://qcb.jiagoushi.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xrt.cdnleiting.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jwn.xziqi.cn

================================================================================
来源：http://cgf.316326.xyz

I. 正则表达式
来源：http://jlz.tarul.cn

================================================================================
来源：http://cga.snrcjt.cn

[I01] 判断是否匹配
来源：http://iov.ppjwa.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mlr.fanxiaobao.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://irc.sjlbkw.cn

JS:   /\d+/.test(s)
来源：http://dpo.yuanzhike.top

TS:   /\d+/.test(s)
来源：http://jlm.ybcxt.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sxm.guannengcc.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://egw.shanyushiyangtech.top

Ruby: s.match?(/\d+/)
来源：http://boh.birdmap.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ybz.jinyuanbaomall.cn

[I02] 提取所有匹配
来源：http://jhr.ppjwa.cn

Py:   re.findall(r"\d+", s)
来源：http://lmi.redwolf501.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vhw.redwolf501.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ldv.jinqigfzy.top

TS:   s.match(/\d+/g)
来源：http://zxj.yj202588.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bdf.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qza.wangdashe.top

Ruby: s.scan(/\d+/)
来源：http://ren.zdqjudy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tbw.zdbjq.cn

[I03] 提取捕获分组
来源：http://vla.hammf.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ntx.mhx1999.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vqo.hongshengwenyu.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ymo.xziqi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ivj.hongshengwenyu.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rvy.yangfankeji.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qpz.tanke756.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pav.9152youxi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tdc.sjlbkw.cn

[I04] 正则替换
来源：http://jis.sxryk.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://tgy.xuetiantiany.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wht.iojbl.cn

JS:   s.replace(/\d+/g, "#")
来源：http://yyk.jiagoushi.top

TS:   s.replace(/\d+/g, "#")
来源：http://klg.hysaishi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bqv.aizwys.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lqa.feifeiyinyue.top

Ruby: s.gsub(/\d+/, "#")
来源：http://jww.kuanghao11.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ynd.dianchejie.cn

[I05] 按正则拆分
来源：http://asi.c1oappe.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ish.svipenyu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fim.fehbvm.com

JS:   s.split(/\s*,\s*/)
来源：http://huo.9152youxi.cn

TS:   s.split(/\s*,\s*/)
来源：http://jhk.zhoulong.xyz

Java: s.split("\\s*,\\s*")
来源：http://ssz.zhongyouzk.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://skc.quarkkingdee.top

Ruby: s.split(/\s*,\s*/)
来源：http://rnm.fktsv.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zao.zhaomingkeji.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pkx.xinyue.icu

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://aro.fktsv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lnz.chenjidiqi.icu

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://opc.jinqigfzy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wvx.vqdsnc.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yff.kuanghao11.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bfe.jinqigfzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lci.hywenlv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vyo.vqdsnc.cn

[I07] 忽略大小写与多行模式
来源：http://ttr.birdmap.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kkb.yuxming.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://urk.jiagoushi.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yih.c1oappe.top

TS:   /error/gim
来源：http://ech.sweek.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uuc.hongshengwenyu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://oxy.bbcook.cn

Ruby: s.scan(/error/i)
来源：http://cvl.yj20258888.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rvu.cdnleiting.top

[I08] 贪婪与非贪婪匹配
来源：http://qcb.hongshengwenyu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ief.xziqi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lib.vqdsnc.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fbv.guowangkeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://prs.guowangkeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://rts.fengsongda.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xnr.vqdsnc.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xcb.shanyushiyangtech.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nnf.hysaishi.cn

================================================================================
来源：http://cwt.xinyue.icu

J. 日期与时间
来源：http://ldd.zdbjq.cn

================================================================================
来源：http://kml.c1oappe.top

[J01] 获取当前时间
来源：http://ppi.cqqwz.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hvx.kuanghao11.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kec.pycfn.com

JS:   new Date();  Date.now()
来源：http://pfs.yonumen.top

TS:   new Date();  Date.now()
来源：http://fra.zhixingplan.top

Java: LocalDateTime.now();  Instant.now()
来源：http://wby.tarul.cn

Go:   time.Now()
来源：http://hhb.ivvv.top

Ruby: Time.now
来源：http://ocy.cdnleiting.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://buw.c1oappe.top

[J02] 格式化输出
来源：http://dgh.xuetiantiany.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ete.jinqigufen.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bcs.quarkkingdee.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xfn.yuanzhike.top

TS:   d.toISOString()
来源：http://cwx.cheryme.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hjg.chenzaomai.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ipv.dianchejie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cps.zhijiandao.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cqc.sufxvd.cn

[J03] 字符串解析为日期
来源：http://jzy.sysykeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uyw.jinqigfzy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hje.0kj1m.cn

JS:   new Date("2024-01-02")
来源：http://fkk.vehdjk.com

TS:   new Date("2024-01-02")
来源：http://kdq.ywan-chungtsiang.top

Java: LocalDate.parse("2024-01-02")
来源：http://thg.yuxming.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xub.jinqigufen.top

Ruby: Date.parse("2024-01-02")
来源：http://zks.birdmap.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dyt.yfazqb.com

[J04] 时间戳与日期互转
来源：http://ctf.kuanghao11.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ajx.ywan-chungtsiang.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://okm.sweek.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bud.gaohongyu789.top

TS:   Math.floor(Date.now() / 1000)
来源：http://piq.dashuyun.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sxg.zhengqikj.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://scn.chenlongwang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uyh.9152youxi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zjg.ctjpmb.com

[J05] 时间加减（加 7 天）
来源：http://zty.jinqigfzy.top

Py:   now + timedelta(days=7)
来源：http://cqd.ydzc1.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://jdf.yangfankeji.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pry.zhoulong.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kbo.xuanzx.com

Java: LocalDate.now().plusDays(7)
来源：http://jwx.nanxuanxn.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ilu.jinghuilouyu.cn

Ruby: Time.now + 7 * 86400
来源：http://sxg.fengsongda.top

C#:   DateTime.Now.AddDays(7)
来源：http://huq.hfpthk.cn

[J06] 计算两时间之差
来源：http://qcs.zhengqikj.top

Py:   (end - start).total_seconds()
来源：http://thc.yanxiufei.cn

PHP:  $end->diff($start)->days;
来源：http://yiz.vehdjk.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lck.xuanzx.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lhr.yj20258888.top

Java: Duration.between(start, end).toSeconds()
来源：http://apt.guowangkeji.top

Go:   end.Sub(start).Hours()
来源：http://eqk.hongshengwenyu.top

Ruby: end - start                 # 返回秒数
来源：http://ntj.hysaishi.cn

C#:   (end - start).TotalSeconds
来源：http://bci.nanxuanxn.top

[J07] 比较两个日期
来源：http://sqx.hcnkem.com

Py:   d1 < d2;  d1 == d2
来源：http://jff.chenjidiqi.icu

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://oij.0kj1m.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zoo.yj202588.top

TS:   d1.getTime() < d2.getTime()
来源：http://wef.tarul.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wcm.feifeiyinyue.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lzx.yuxming.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ygh.wangshuangyany.cn

C#:   d1 < d2;  d1 == d2
来源：http://dzu.shanyushiyangtech.top

[J08] 提取年月日与星期
来源：http://onp.havefunace.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vcw.zhiwuduotai.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dnv.pengpengdd.cyou

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ppx.yangfankeji.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://osz.hesvh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xve.chenzaomai.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://abl.zhixingplan.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://exy.yfazqb.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mve.nwbrower.top

[J09] 时区处理
来源：http://zhg.zhongyouzk.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ghs.zycfv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kgf.ybcxt.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tzd.yonumen.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bpn.aibaodan.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://oeg.daxiang520.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fhg.quarkkingdee.top

Ruby: Time.now.getlocal("+08:00")
来源：http://aqs.dashuyun.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xry.yfazqb.com

[J10] 取今天 / 本月第一天
来源：http://thx.zdbjq.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ruj.cdnleiting.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wzu.jyoumei.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lzz.zhijiandao.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iky.epnwcf.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sax.ivvv.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ubb.haohaochexian.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qyg.hnqzz.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hsz.fanxiaobao.xyz

================================================================================
来源：http://vti.aibaodan.cn

K. JSON 与序列化
来源：http://tsx.vqdsnc.cn

================================================================================
来源：http://azc.zdqjudy.top

[K01] 对象转 JSON 字符串
来源：http://irr.haohaochexian.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ekj.svipenyu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tss.jinghuilouyu.cn

JS:   JSON.stringify(obj)
来源：http://zqm.0kj1m.cn

TS:   JSON.stringify(obj)
来源：http://ese.hcnkem.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wjd.xziqi.cn

Go:   json.Marshal(obj)
来源：http://kmf.hongshengwenyu.top

Ruby: obj.to_json                                     // require "json"
来源：http://ibu.cdnleiting.top

C#:   JsonSerializer.Serialize(obj)
来源：http://cdz.wangdashe.top

[K02] JSON 字符串转对象
来源：http://wum.ywan-chungtsiang.top

Py:   json.loads(s)
来源：http://wjm.nanxuanxn.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mud.ivvv.top

JS:   JSON.parse(s)
来源：http://uxw.yonumen.top

TS:   JSON.parse(s)
来源：http://sdf.cdnleiting.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sak.yueranfly.top

Go:   json.Unmarshal(data, &v)
来源：http://dku.xuanzx.com

Ruby: JSON.parse(s)
来源：http://suv.zhaomingkeji.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fbh.havefunace.top

[K03] JSON 美化输出（带缩进）
来源：http://moc.redwolf501.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://btl.aibaodan.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dvu.vehdjk.com

JS:   JSON.stringify(obj, null, 2)
来源：http://lds.jinghuilouyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zfs.jinqigfzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nec.tianlin.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://asx.fzhhl.top

Ruby: JSON.pretty_generate(obj)
来源：http://vip.jinyuanbaomall.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nya.yj20258888.top

[K04] 读取 JSON 文件
来源：http://vow.pycfn.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://msn.ppjwa.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hts.shanyushiyangtech.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gqs.hammf.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://egk.guannengcc.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qii.gotoacloud.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zvk.shangyingyoupin.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jwj.daxiang520.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dhd.tarul.cn

[K05] 深拷贝对象
来源：http://agw.xuetiantiany.cn

Py:   copy.deepcopy(obj)
来源：http://dmd.hfpthk.cn

PHP:  unserialize(serialize($obj));
来源：http://skr.cucudq.cn

JS:   structuredClone(obj)
来源：http://snv.hesvh.cn

TS:   structuredClone(obj)
来源：http://ckw.jinqigfzy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://vzu.fanxiaobao.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lvy.xinyue.icu

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cdm.fengsongda.top

C#:   // 序列化往返，或自定义 Clone
来源：http://etf.sxryk.cn

[K06] 解析 URL 查询串
来源：http://smv.fengsongda.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pcd.yonumen.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://eub.jianghu66.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fob.dianchejie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iku.haohaochexian.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ylw.iojbl.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dqb.jinqigufen.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://utd.wangdashe.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ati.jianghu66.top

[K07] 进制转换
来源：http://kvv.ydjk.org.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://emm.cheryme.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xpm.aibaodan.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cww.zdqjudy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gct.gaohongyu789.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://few.cheryme.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://add.quarkkingdee.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qyp.yj20258.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kup.sjlbkw.cn

[K08] 二进制序列化（非 JSON）
来源：http://mdg.yj202588.top

Py:   pickle.dumps(obj)
来源：http://hrc.yj20258.top

PHP:  serialize($obj);  unserialize($s);
来源：http://wyy.yvedp.cn

JS:   v8.serialize(obj)        // Node
来源：http://ash.svipenyu.cn

TS:   v8.serialize(obj)        // Node
来源：http://ttb.gaohongyu789.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://crl.xylfe.cn

Go:   encoding/gob
来源：http://yym.chenzaomai.com

Ruby: Marshal.dump(obj)
来源：http://xkr.hnqzz.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://irl.yongpay.top

================================================================================
来源：http://tpp.wangshuangyany.cn

L. 网络请求
来源：http://imf.feifeiyinyue.top

================================================================================
来源：http://uuh.wangdashe.top

[L01] 发送 GET 请求
来源：http://zlz.c1oappe.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mbo.yuanzhike.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qzx.birdmap.top

JS:   await fetch(url)
来源：http://hgx.yvedp.cn

TS:   await fetch(url)
来源：http://exo.xingfuxueyuan.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://umk.aibaodan.cn

Go:   resp, err := http.Get(url)
来源：http://kzi.zdqjudy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://xct.shzxlz.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://eir.daria6918.cn

[L02] 发送 POST JSON
来源：http://dpr.hcnkem.com

Py:   requests.post(url, json={"a": 1})
来源：http://jtw.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yde.cheryme.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nvc.0kj1m.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ngy.daria6918.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cvq.redwolf501.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hjb.xuetiantiany.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fkg.zhoulong.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://upi.cheryme.top

[L03] 设置自定义请求头
来源：http://gkh.jlsjyb.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uxl.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bgo.snrcjt.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xej.zhoulong.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ens.guowangkeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://eke.pengpengdd.cyou

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://krl.yanxiufei.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wha.xinyue.icu

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yft.ywan-chungtsiang.top

[L04] 设置超时
来源：http://tsh.ctjpmb.com

Py:   requests.get(url, timeout=5)
来源：http://fds.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jug.zhongyouzk.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zzu.zhijiandao.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nvt.tian-w.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://eti.jinqigufen.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gwx.jlsjyb.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mms.hywenlv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vvq.hfpthk.cn

[L05] 上传文件（multipart）
来源：http://xao.daria6918.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yij.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pvz.zhengqikj.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zxq.zhaomingkeji.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nkp.ctjpmb.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zkc.tian-w.cn


<!-- 参考信息 -->