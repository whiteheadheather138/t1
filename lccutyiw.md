代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ncn.c1oappe.top

Ruby: raise MyError.new("fail", 500)
来源：http://fqn.jyoumei.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yfn.quarkkingdee.top

[H10] 资源自动释放
来源：http://klf.cqqwz.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://utt.shanyushiyangtech.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ldb.sysykeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ddr.xuetiantiany.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mik.tarul.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xhz.chenzaomai.com

Go:   defer f.Close()
来源：http://avo.guowangkeji.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fyk.kuanghao11.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wgt.meibo888.top

================================================================================
来源：http://brb.zhixingplan.top

I. 正则表达式
来源：http://yxs.ywan-chungtsiang.top

================================================================================
来源：http://uhp.jqgfzy.top

[I01] 判断是否匹配
来源：http://hie.feifeiyinyue.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://owy.316326.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://esq.kuanghao11.cn

JS:   /\d+/.test(s)
来源：http://lph.guannengcc.top

TS:   /\d+/.test(s)
来源：http://azk.shzxlz.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rix.fanxiaobao.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mhu.daria6918.cn

Ruby: s.match?(/\d+/)
来源：http://kbg.nwbrower.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sqq.kuanghao11.cn

[I02] 提取所有匹配
来源：http://lap.hnqzz.top

Py:   re.findall(r"\d+", s)
来源：http://wor.sysykeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kcs.snrcjt.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://iua.316326.xyz

TS:   s.match(/\d+/g)
来源：http://syb.hnqzz.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://khn.dashuyun.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sjj.hysaishi.cn

Ruby: s.scan(/\d+/)
来源：http://yei.dianchejie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ivj.nanxinkj.top

[I03] 提取捕获分组
来源：http://pyf.gogol.net.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qes.ybcxt.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sfr.hysaishi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://oal.aizwys.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dgv.havefunace.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://byd.nwbrower.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ujp.ppjwa.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zce.meibo888.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zft.ywan-chungtsiang.top

[I04] 正则替换
来源：http://vow.epnwcf.com

Py:   re.sub(r"\d+", "#", s)
来源：http://xle.quarkkingdee.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ivx.epnwcf.com

JS:   s.replace(/\d+/g, "#")
来源：http://mpg.yuxming.cn

TS:   s.replace(/\d+/g, "#")
来源：http://eoo.zhoulong.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://gqm.chenlongwang.top

Go:   re.ReplaceAllString(s, "#")
来源：http://qmk.daxiang520.top

Ruby: s.gsub(/\d+/, "#")
来源：http://dkv.mhx1999.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kue.sjlbkw.cn

[I05] 按正则拆分
来源：http://tdf.fzhhl.top

Py:   re.split(r"\s*,\s*", s)
来源：http://gmb.ydjk.org.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://omb.ybcxt.top

JS:   s.split(/\s*,\s*/)
来源：http://iim.snrcjt.cn

TS:   s.split(/\s*,\s*/)
来源：http://njr.pycfn.com

Java: s.split("\\s*,\\s*")
来源：http://itp.yj20258.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pxf.ppjwa.cn

Ruby: s.split(/\s*,\s*/)
来源：http://uto.feifeiyinyue.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cip.jinqigfzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mzj.ybcxt.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xeo.pengpengdd.cyou

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vbz.hcnkem.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bla.shangyingyoupin.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uav.yfazqb.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://azs.andypj.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lop.guannengcc.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jlj.tanke756.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hds.bjfxy.top

[I07] 忽略大小写与多行模式
来源：http://fhy.kuanghao11.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xvm.cucudq.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hlb.yj20258.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://klh.shuidangran.top

TS:   /error/gim
来源：http://nqq.ybcxt.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ibp.guowangkeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ywh.shanyushiyangkeji.top

Ruby: s.scan(/error/i)
来源：http://osh.hammf.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://npn.cashguo.top

[I08] 贪婪与非贪婪匹配
来源：http://xag.aibaodan.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zuu.guannengcc.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dul.aizwys.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wyj.sysykeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wrf.andypj.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://egq.hnqzz.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mzp.hfpthk.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cxb.pengpengdd.cyou

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://loi.hcnkem.com

================================================================================
来源：http://uen.sjlbkw.cn

J. 日期与时间
来源：http://ufd.zhengqikj.top

================================================================================
来源：http://izk.hongshengwenyu.top

[J01] 获取当前时间
来源：http://zqy.zycfv.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lki.jiagoushi.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bmh.hnqzz.top

JS:   new Date();  Date.now()
来源：http://sof.sysykeji.top

TS:   new Date();  Date.now()
来源：http://kna.cdnleiting.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ntr.cheryme.top

Go:   time.Now()
来源：http://avh.fktsv.cn

Ruby: Time.now
来源：http://uzz.gaohongyu789.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://myd.xinyue.icu

[J02] 格式化输出
来源：http://xvx.yuxming.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://boh.zhixingplan.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://owb.bbcook.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cyh.xziqi.cn

TS:   d.toISOString()
来源：http://mlt.cheryme.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hiu.yvedp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jyu.jinyuanbaomall.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oqi.yj20258888.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wxa.hesvh.cn

[J03] 字符串解析为日期
来源：http://zfv.svipenyu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qic.xingfuxueyuan.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sxf.fzhhl.top

JS:   new Date("2024-01-02")
来源：http://vqa.iojbl.cn

TS:   new Date("2024-01-02")
来源：http://rmd.zhiwuduotai.top

Java: LocalDate.parse("2024-01-02")
来源：http://nrm.jyoumei.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://utr.jiagoushi.top

Ruby: Date.parse("2024-01-02")
来源：http://rkw.jinqigfzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zsb.shanyushiyangtech.top

[J04] 时间戳与日期互转
来源：http://zey.jianghu66.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://scy.meibo888.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gzn.yanxiufei.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lwp.smart0.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://nml.ywan-chungtsiang.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cxh.nanxuanxn.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://imk.chenlongwang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://psp.quarkkingdee.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vfx.chenjidiqi.icu

[J05] 时间加减（加 7 天）
来源：http://gjx.zdbjq.cn

Py:   now + timedelta(days=7)
来源：http://tmk.chenzaomai.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://zvs.jinqigufen.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lxn.shangyingyoupin.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://upr.hnxiangtu.top

Java: LocalDate.now().plusDays(7)
来源：http://pub.feifeiyinyue.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cir.hnqzz.top

Ruby: Time.now + 7 * 86400
来源：http://bue.yongpay.top

C#:   DateTime.Now.AddDays(7)
来源：http://dhx.0kj1m.cn

[J06] 计算两时间之差
来源：http://avy.wangshuangyany.cn

Py:   (end - start).total_seconds()
来源：http://slj.nanxinkj.top

PHP:  $end->diff($start)->days;
来源：http://lpj.bbcook.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nah.zhongyouzk.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bpt.cqqwz.cn

Java: Duration.between(start, end).toSeconds()
来源：http://eam.9152youxi.cn

Go:   end.Sub(start).Hours()
来源：http://skp.tanke756.top

Ruby: end - start                 # 返回秒数
来源：http://fbp.ydzc1.top

C#:   (end - start).TotalSeconds
来源：http://dnk.epnwcf.com

[J07] 比较两个日期
来源：http://nau.sufxvd.cn

Py:   d1 < d2;  d1 == d2
来源：http://uqd.birdmap.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vcy.zhengqikj.top

JS:   d1.getTime() < d2.getTime()
来源：http://yel.gzhubu.top

TS:   d1.getTime() < d2.getTime()
来源：http://gix.svipenyu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cgq.tarul.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://eox.316326.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://psg.zhongyouzk.top

C#:   d1 < d2;  d1 == d2
来源：http://gmj.ivvv.top

[J08] 提取年月日与星期
来源：http://zyt.vqdsnc.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mur.uphjek.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://aur.dashuyun.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qed.dashuyun.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://par.shanyushiyangtech.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xtp.sweek.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hhf.fktsv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xda.daria6918.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rel.mhx1999.top

[J09] 时区处理
来源：http://mzp.jlsjyb.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vvx.jinqigufen.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://taa.yvedp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bwb.sweek.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gcq.shanyushiyangtech.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://stl.ydzc1.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zqs.xziqi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://bqy.chenzaomai.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ncy.aizwys.cn

[J10] 取今天 / 本月第一天
来源：http://eeo.fzhhl.top

Py:   date.today();  date.today().replace(day=1)
来源：http://gbe.jinqigfzy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rkt.316326.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://aal.wangshuangyany.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://coq.yvedp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pzj.nanxinkj.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mpl.jinqigfzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xud.xuanzx.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://obp.52xcode.cn

================================================================================
来源：http://kye.shzxlz.cn

K. JSON 与序列化
来源：http://haw.nwbrower.top

================================================================================
来源：http://wxc.jianghu66.top

[K01] 对象转 JSON 字符串
来源：http://ayw.yj20258888.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fph.gaohongyu789.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ois.hcnkem.com

JS:   JSON.stringify(obj)
来源：http://rgt.cashguo.top

TS:   JSON.stringify(obj)
来源：http://uvq.xziqi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yut.sweek.top

Go:   json.Marshal(obj)
来源：http://sxl.fehbvm.com

Ruby: obj.to_json                                     // require "json"
来源：http://qwj.yj202588.top

C#:   JsonSerializer.Serialize(obj)
来源：http://bjk.ppjwa.cn

[K02] JSON 字符串转对象
来源：http://ztf.hnqzz.top

Py:   json.loads(s)
来源：http://wuz.sysykeji.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://slw.hesvh.cn

JS:   JSON.parse(s)
来源：http://cek.tianlin.xyz

TS:   JSON.parse(s)
来源：http://ilg.cdnleiting.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://grk.ydjk.org.cn

Go:   json.Unmarshal(data, &v)
来源：http://zfg.fanxiaobao.xyz

Ruby: JSON.parse(s)
来源：http://fax.aizwys.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bmk.0kj1m.cn

[K03] JSON 美化输出（带缩进）
来源：http://jfz.cqqwz.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zza.sufxvd.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hjh.jiagoushi.top

JS:   JSON.stringify(obj, null, 2)
来源：http://bbi.ywan-chungtsiang.top

TS:   JSON.stringify(obj, null, 2)
来源：http://mgv.sweek.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pnc.nanxinkj.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pdt.quarkkingdee.top

Ruby: JSON.pretty_generate(obj)
来源：http://onm.zhengqikj.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gmt.fanxiaobao.xyz

[K04] 读取 JSON 文件
来源：http://mly.tianlin.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rak.gotoacloud.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ysc.hongshengwenyu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qjm.jinqigfzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vdx.cqqwz.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hhe.zhoulong.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ubt.xziqi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xym.birdmap.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kmr.zdbjq.cn

[K05] 深拷贝对象
来源：http://cqg.hesvh.cn

Py:   copy.deepcopy(obj)
来源：http://qqd.jiagoushi.top

PHP:  unserialize(serialize($obj));
来源：http://fsl.kuanghao11.cn

JS:   structuredClone(obj)
来源：http://ahb.shanyushiyangtech.top

TS:   structuredClone(obj)
来源：http://xlu.meibo888.top

Java: // 手写拷贝构造，或序列化往返
来源：http://fik.cqqwz.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hke.fktsv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qsu.guannengcc.top

C#:   // 序列化往返，或自定义 Clone
来源：http://wye.hnxiangtu.top

[K06] 解析 URL 查询串
来源：http://pqa.yfazqb.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://srj.sufxvd.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dud.zhijiandao.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jlk.aizwys.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yxk.fzhhl.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://iaz.52xcode.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://isi.fzhhl.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://etg.ybcxt.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yus.yanxiufei.cn

[K07] 进制转换
来源：http://sov.gaohongyu789.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://naf.gogol.net.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bss.daria6918.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rkm.xuanzx.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jpl.sjlbkw.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tqw.vqdsnc.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ofz.ybcxt.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wnq.jinghuilouyu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cit.iojbl.cn

[K08] 二进制序列化（非 JSON）
来源：http://vru.jinqigufen.top

Py:   pickle.dumps(obj)
来源：http://gvb.shuidangran.top

PHP:  serialize($obj);  unserialize($s);
来源：http://isd.xziqi.cn

JS:   v8.serialize(obj)        // Node
来源：http://xvt.zdbjq.cn

TS:   v8.serialize(obj)        // Node
来源：http://lhw.jqgufenzy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nso.hongshengwenyu.top

Go:   encoding/gob
来源：http://rfk.shuidangran.top

Ruby: Marshal.dump(obj)
来源：http://epz.sweek.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wuv.yueranfly.top

================================================================================
来源：http://orz.gaohongyu789.top

L. 网络请求
来源：http://sct.ehwqpu.com

================================================================================
来源：http://tlf.xziqi.cn

[L01] 发送 GET 请求
来源：http://pfy.jinyuanbaomall.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wwq.fengsongda.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cka.ctjpmb.com

JS:   await fetch(url)
来源：http://phv.xuetiantiany.cn

TS:   await fetch(url)
来源：http://bin.vehdjk.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kyj.daria6918.cn

Go:   resp, err := http.Get(url)
来源：http://giq.jinqigufen.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jki.bbcook.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nlh.yangfankeji.com

[L02] 发送 POST JSON
来源：http://emw.yj202588.top

Py:   requests.post(url, json={"a": 1})
来源：http://yyz.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uux.jiagoushi.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://caf.pengpengdd.cyou

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mmm.bjfxy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yzp.yj202588.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ddl.jlsjyb.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ebe.zhongyouzk.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kzs.yuxming.cn

[L03] 设置自定义请求头
来源：http://gcw.yvedp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hta.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hfe.hysaishi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://emt.andypj.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lmz.jyoumei.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uzk.gaohongyu789.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uqp.yongpay.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nty.ybcxt.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cwi.hywenlv.cn

[L04] 设置超时
来源：http://xpp.chenzaomai.com

Py:   requests.get(url, timeout=5)
来源：http://yns.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xpn.hywenlv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://udd.ybcxt.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mvl.gaohongyu789.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cqi.zhaomingkeji.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vro.zdqjudy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jny.gzhubu.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fvv.cqqwz.cn

[L05] 上传文件（multipart）
来源：http://kvk.chenlongwang.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lzb.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://psb.zhijiandao.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fag.zhoulong.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nkg.daria6918.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sqj.sweek.top


<!-- 参考信息 -->