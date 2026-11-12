代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://pps.birdmap.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ejr.bbcook.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hox.tian-w.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vjr.yj20258888.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wjt.jinqigfzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://kfd.sysykeji.top

C#:   // 自定义异常类中加 Code 属性
来源：http://kts.zhixingplan.top

[H10] 资源自动释放
来源：http://gxi.uphjek.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://edl.yanxiufei.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xom.c1oappe.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qtq.dianchejie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fzb.sysykeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wzj.fanxiaobao.xyz

Go:   defer f.Close()
来源：http://cay.yuanzhike.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dbo.sxryk.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://all.ivvv.top

================================================================================
来源：http://rie.yj202588.top

I. 正则表达式
来源：http://tqr.ybcxt.top

================================================================================
来源：http://cbp.cashguo.top

[I01] 判断是否匹配
来源：http://vyk.kuanghao11.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://txw.zhijiandao.cn

PHP:  preg_match('/\d+/', $s);
来源：http://yrq.gotoacloud.top

JS:   /\d+/.test(s)
来源：http://mxa.havefunace.top

TS:   /\d+/.test(s)
来源：http://prp.daxiang520.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rbl.jqgufenzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jzi.chenzaomai.com

Ruby: s.match?(/\d+/)
来源：http://rro.xuetiantiany.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wpv.mhx1999.top

[I02] 提取所有匹配
来源：http://dyc.zhengqikj.top

Py:   re.findall(r"\d+", s)
来源：http://rni.sjlbkw.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cpu.yj20258.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://awl.sysykeji.top

TS:   s.match(/\d+/g)
来源：http://ucs.sysykeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hpi.jqgufenzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rpa.uphjek.com

Ruby: s.scan(/\d+/)
来源：http://syy.ehwqpu.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sem.chenlongwang.top

[I03] 提取捕获分组
来源：http://zbh.yongpay.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rke.svipenyu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bbd.jlsjyb.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vhh.hongshengwenyu.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wxm.tanke756.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qmg.havefunace.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hvd.sxryk.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zic.yonumen.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qif.shangyingyoupin.top

[I04] 正则替换
来源：http://ixk.xuetiantiany.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://duy.andypj.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ahr.gzhubu.top

JS:   s.replace(/\d+/g, "#")
来源：http://fug.aibaodan.cn

TS:   s.replace(/\d+/g, "#")
来源：http://bwr.yj202588.top

Java: s.replaceAll("\\d+", "#")
来源：http://dka.xuanzx.com

Go:   re.ReplaceAllString(s, "#")
来源：http://kux.nwbrower.top

Ruby: s.gsub(/\d+/, "#")
来源：http://rgs.hcnkem.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xiu.ivvv.top

[I05] 按正则拆分
来源：http://wma.zhaomingkeji.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://ldo.epnwcf.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://apx.cdnleiting.top

JS:   s.split(/\s*,\s*/)
来源：http://nmk.hesvh.cn

TS:   s.split(/\s*,\s*/)
来源：http://tdq.hysaishi.cn

Java: s.split("\\s*,\\s*")
来源：http://yvw.pycfn.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vxv.feifeiyinyue.top

Ruby: s.split(/\s*,\s*/)
来源：http://cet.nanxinkj.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nxq.yuxming.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yao.jyoumei.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://acg.ybcxt.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tof.yvedp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iiv.jqgfzy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kav.sjlbkw.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://scq.jianghu66.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vcb.quarkkingdee.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yxp.birdmap.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xno.cheryme.top

[I07] 忽略大小写与多行模式
来源：http://swl.xuanzx.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://orc.pengpengdd.cyou

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://omb.birdmap.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hua.sysykeji.top

TS:   /error/gim
来源：http://qah.zhoulong.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://sxf.nanxinkj.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://idh.shuidangran.top

Ruby: s.scan(/error/i)
来源：http://adj.shanyushiyangtech.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ipz.daxiang520.top

[I08] 贪婪与非贪婪匹配
来源：http://csa.xziqi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rhn.chenjidiqi.icu

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://alj.guannengcc.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cnt.svipenyu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zhz.feifeiyinyue.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://wal.wangdashe.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://opb.316326.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ojr.aizwys.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jbt.fehbvm.com

================================================================================
来源：http://qwo.316326.xyz

J. 日期与时间
来源：http://vhh.jqgfzy.top

================================================================================
来源：http://rsu.zhongyouzk.top

[J01] 获取当前时间
来源：http://awf.sufxvd.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gzm.shangyingyoupin.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xyc.fzhhl.top

JS:   new Date();  Date.now()
来源：http://dcb.sjlbkw.cn

TS:   new Date();  Date.now()
来源：http://pqo.fktsv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://efh.meibo888.top

Go:   time.Now()
来源：http://ych.shzxlz.cn

Ruby: Time.now
来源：http://bfs.smart0.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://how.jiagoushi.top

[J02] 格式化输出
来源：http://bsg.xuanzx.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fdd.fzhhl.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://eti.pengpengdd.cyou

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sgy.havefunace.top

TS:   d.toISOString()
来源：http://fpv.svipenyu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pff.aibaodan.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sfg.tianlin.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bni.zdqjudy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bkg.fzhhl.top

[J03] 字符串解析为日期
来源：http://pyf.sjlbkw.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tbr.pycfn.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hiz.zdqjudy.top

JS:   new Date("2024-01-02")
来源：http://ybo.gaohongyu789.top

TS:   new Date("2024-01-02")
来源：http://jbn.redwolf501.top

Java: LocalDate.parse("2024-01-02")
来源：http://shy.zhijiandao.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xhv.hywenlv.cn

Ruby: Date.parse("2024-01-02")
来源：http://hhx.hammf.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zgl.xinyue.icu

[J04] 时间戳与日期互转
来源：http://hfp.sxryk.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://oba.shanyushiyangkeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://syb.xinyue.icu

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rdi.hesvh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://krc.sufxvd.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fak.xziqi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nzi.snrcjt.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://son.aibaodan.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ixi.pengpengdd.cyou

[J05] 时间加减（加 7 天）
来源：http://zsm.jinghuilouyu.cn

Py:   now + timedelta(days=7)
来源：http://seu.hysaishi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xbx.shzxlz.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hql.jinqigfzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://isd.daxiang520.top

Java: LocalDate.now().plusDays(7)
来源：http://mox.dianchejie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://umv.yj20258.top

Ruby: Time.now + 7 * 86400
来源：http://vti.cdnleiting.top

C#:   DateTime.Now.AddDays(7)
来源：http://eum.zhiwuduotai.top

[J06] 计算两时间之差
来源：http://npy.cucudq.cn

Py:   (end - start).total_seconds()
来源：http://htd.chenjidiqi.icu

PHP:  $end->diff($start)->days;
来源：http://ekh.havefunace.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dqq.bjfxy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uda.nanxuanxn.top

Java: Duration.between(start, end).toSeconds()
来源：http://djk.yuanzhike.top

Go:   end.Sub(start).Hours()
来源：http://woj.shanyushiyangtech.top

Ruby: end - start                 # 返回秒数
来源：http://dgh.yangfankeji.com

C#:   (end - start).TotalSeconds
来源：http://qer.sjlbkw.cn

[J07] 比较两个日期
来源：http://xcv.jqgufenzy.top

Py:   d1 < d2;  d1 == d2
来源：http://wlv.cqqwz.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tuo.shzxlz.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lrc.epnwcf.com

TS:   d1.getTime() < d2.getTime()
来源：http://gqs.meibo888.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dsa.xuetiantiany.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zlz.shanyushiyangtech.top

Ruby: d1 < d2;  d1 == d2
来源：http://hsk.yj20258888.top

C#:   d1 < d2;  d1 == d2
来源：http://rhf.dianchejie.cn

[J08] 提取年月日与星期
来源：http://wto.zhengqikj.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dpw.316326.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uxi.nwbrower.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uro.fanxiaobao.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vjk.zycfv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mau.sjlbkw.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://axy.hnxiangtu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ojx.zdqjudy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rtt.yuxming.cn

[J09] 时区处理
来源：http://hxd.fzhhl.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bsn.hysaishi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://drr.jinyuanbaomall.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lof.mhx1999.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zry.9152youxi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mum.zdbjq.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ttn.ydjk.org.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wpp.hesvh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://swp.gzhubu.top

[J10] 取今天 / 本月第一天
来源：http://klw.jlsjyb.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vdj.zhijiandao.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://feu.zhaomingkeji.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fmn.vqdsnc.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bjw.yonumen.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://laz.redwolf501.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ntw.jyoumei.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vvv.dianchejie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nlo.yuxming.cn

================================================================================
来源：http://gbt.yvedp.cn

K. JSON 与序列化
来源：http://cwj.haohaochexian.top

================================================================================
来源：http://xsr.feifeiyinyue.top

[K01] 对象转 JSON 字符串
来源：http://fko.nwbrower.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://amx.feifeiyinyue.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fvj.xziqi.cn

JS:   JSON.stringify(obj)
来源：http://ngn.guannengcc.top

TS:   JSON.stringify(obj)
来源：http://fph.tanke756.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ctn.gaohongyu789.top

Go:   json.Marshal(obj)
来源：http://teh.pengpengdd.cyou

Ruby: obj.to_json                                     // require "json"
来源：http://uti.316326.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://esw.yueranfly.top

[K02] JSON 字符串转对象
来源：http://nus.yonumen.top

Py:   json.loads(s)
来源：http://cua.ydzc1.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nry.shzxlz.cn

JS:   JSON.parse(s)
来源：http://qun.uphjek.com

TS:   JSON.parse(s)
来源：http://jqc.hnqzz.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qqh.ywan-chungtsiang.top

Go:   json.Unmarshal(data, &v)
来源：http://uos.sysykeji.top

Ruby: JSON.parse(s)
来源：http://gll.yj202588.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ohv.gotoacloud.top

[K03] JSON 美化输出（带缩进）
来源：http://owg.jinqigufen.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nic.hnqzz.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xwq.daxiang520.top

JS:   JSON.stringify(obj, null, 2)
来源：http://sba.xinyue.icu

TS:   JSON.stringify(obj, null, 2)
来源：http://ulw.aibaodan.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jne.shanyushiyangkeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kni.smart0.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://qdj.cdnleiting.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ipm.zhengqikj.top

[K04] 读取 JSON 文件
来源：http://mwn.iojbl.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zlr.shanyushiyangkeji.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dgl.jinqigfzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ykk.redwolf501.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ocw.yueranfly.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xas.0kj1m.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rly.jqgufenzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://qpn.xuanzx.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gwe.yfazqb.com

[K05] 深拷贝对象
来源：http://upa.guowangkeji.top

Py:   copy.deepcopy(obj)
来源：http://ctd.gaohongyu789.top

PHP:  unserialize(serialize($obj));
来源：http://ycz.jlsjyb.cn

JS:   structuredClone(obj)
来源：http://vvb.xingfuxueyuan.xyz

TS:   structuredClone(obj)
来源：http://pui.vqdsnc.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qqy.kuanghao11.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pwp.jqgufenzy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sda.316326.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://ojp.andypj.xyz

[K06] 解析 URL 查询串
来源：http://tyy.quarkkingdee.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fea.pengpengdd.cyou

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wvp.zhengqikj.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xdl.xuanzx.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cpb.vehdjk.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zpy.yanxiufei.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vft.cheryme.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://odm.sufxvd.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://iut.epnwcf.com

[K07] 进制转换
来源：http://mdo.hammf.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://grj.nwbrower.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hos.yuanzhike.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dcq.havefunace.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://adj.redwolf501.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rxv.guannengcc.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cer.guowangkeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xjd.yueranfly.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zpf.yongpay.top

[K08] 二进制序列化（非 JSON）
来源：http://qvy.jiagoushi.top

Py:   pickle.dumps(obj)
来源：http://ymo.pycfn.com

PHP:  serialize($obj);  unserialize($s);
来源：http://zze.uphjek.com

JS:   v8.serialize(obj)        // Node
来源：http://lcr.ydjk.org.cn

TS:   v8.serialize(obj)        // Node
来源：http://qcx.redwolf501.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lmc.yj202588.top

Go:   encoding/gob
来源：http://utg.zhiwuduotai.top

Ruby: Marshal.dump(obj)
来源：http://cam.svipenyu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wbr.aibaodan.cn

================================================================================
来源：http://foo.zhiwuduotai.top

L. 网络请求
来源：http://ttx.fzhhl.top

================================================================================
来源：http://dvm.tarul.cn

[L01] 发送 GET 请求
来源：http://bxq.hammf.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tos.haohaochexian.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ons.dashuyun.cn

JS:   await fetch(url)
来源：http://vgq.shzxlz.cn

TS:   await fetch(url)
来源：http://jbb.tianlin.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nzi.yuxming.cn

Go:   resp, err := http.Get(url)
来源：http://xzr.sufxvd.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kiy.zycfv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qbk.shangyingyoupin.top

[L02] 发送 POST JSON
来源：http://ici.dashuyun.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xbg.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cnx.hywenlv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nce.ydzc1.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lpg.jqgfzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://njw.c1oappe.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jtw.iojbl.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nam.fanxiaobao.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uxf.iojbl.cn

[L03] 设置自定义请求头
来源：http://tqd.sxryk.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://htw.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://grf.jlsjyb.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mrn.tianlin.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://got.yanxiufei.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mox.uphjek.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hrc.hnxiangtu.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ble.shangyingyoupin.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tqa.yj202588.top

[L04] 设置超时
来源：http://azw.fengsongda.top

Py:   requests.get(url, timeout=5)
来源：http://hnu.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vnl.gotoacloud.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ctw.9152youxi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zsa.jinqigfzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vhp.sufxvd.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dkm.fehbvm.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pcv.gogol.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wmm.andypj.xyz

[L05] 上传文件（multipart）
来源：http://fgn.ydzc1.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ewd.ivvv.top


<!-- 参考信息 -->