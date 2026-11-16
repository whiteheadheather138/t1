代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://vtu.zhixingplan.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lzv.jinghuilouyu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sqx.iojbl.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ydi.cqqwz.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nnc.nanxinkj.top

Ruby: raise MyError.new("fail", 500)
来源：http://sol.pycfn.com

C#:   // 自定义异常类中加 Code 属性
来源：http://upr.fehbvm.com

[H10] 资源自动释放
来源：http://iig.yj20258.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://afi.gotoacloud.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hpn.yuanzhike.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://poo.hongshengwenyu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://oof.hysaishi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wsx.wangshuangyany.cn

Go:   defer f.Close()
来源：http://zdj.yvedp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cqp.nanxinkj.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zim.hfpthk.cn

================================================================================
来源：http://hhy.zhijiandao.cn

I. 正则表达式
来源：http://qme.zycfv.cn

================================================================================
来源：http://mlx.dashuyun.cn

[I01] 判断是否匹配
来源：http://bvr.gotoacloud.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xov.aizwys.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hit.feifeiyinyue.top

JS:   /\d+/.test(s)
来源：http://orq.xziqi.cn

TS:   /\d+/.test(s)
来源：http://ort.yonumen.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://syk.fanxiaobao.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kse.wangdashe.top

Ruby: s.match?(/\d+/)
来源：http://psi.gotoacloud.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qzk.cashguo.top

[I02] 提取所有匹配
来源：http://zeq.sxryk.cn

Py:   re.findall(r"\d+", s)
来源：http://jgw.bjfxy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zmi.yueranfly.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://urc.havefunace.top

TS:   s.match(/\d+/g)
来源：http://ckx.zhixingplan.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gap.zhongyouzk.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lnk.aizwys.cn

Ruby: s.scan(/\d+/)
来源：http://ruw.bbcook.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://prm.gaohongyu789.top

[I03] 提取捕获分组
来源：http://scs.cdnleiting.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qas.dianchejie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://esy.cheryme.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mmp.fehbvm.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://thn.daxiang520.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ajl.tian-w.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ucx.52xcode.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lub.zhixingplan.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mim.hysaishi.cn

[I04] 正则替换
来源：http://mgv.shangyingyoupin.top

Py:   re.sub(r"\d+", "#", s)
来源：http://pqu.hywenlv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gew.9152youxi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mjb.kuanghao11.cn

TS:   s.replace(/\d+/g, "#")
来源：http://syu.meibo888.top

Java: s.replaceAll("\\d+", "#")
来源：http://aka.yuanzhike.top

Go:   re.ReplaceAllString(s, "#")
来源：http://hjt.fengsongda.top

Ruby: s.gsub(/\d+/, "#")
来源：http://clu.zhixingplan.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://eie.fehbvm.com

[I05] 按正则拆分
来源：http://jxp.zhoulong.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://yej.yongpay.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ahu.mhx1999.top

JS:   s.split(/\s*,\s*/)
来源：http://pja.gzhubu.top

TS:   s.split(/\s*,\s*/)
来源：http://xuw.aizwys.cn

Java: s.split("\\s*,\\s*")
来源：http://gtw.zdqjudy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://akk.yuxming.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hzf.cucudq.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fea.jiagoushi.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ory.zdbjq.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gux.smart0.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tcc.hesvh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kbt.yfazqb.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jdn.dashuyun.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cso.nanxinkj.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zvh.birdmap.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nst.jiagoushi.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nhp.uphjek.com

[I07] 忽略大小写与多行模式
来源：http://suv.ybcxt.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rqq.pycfn.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rky.redwolf501.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pcc.mhx1999.top

TS:   /error/gim
来源：http://xad.havefunace.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rkh.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://elx.52xcode.cn

Ruby: s.scan(/error/i)
来源：http://hjv.cheryme.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jzr.ydjk.org.cn

[I08] 贪婪与非贪婪匹配
来源：http://syl.pycfn.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wgr.jianghu66.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fag.meibo888.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qqw.wangshuangyany.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ltw.aizwys.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://eaj.sysykeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gfq.zdbjq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wkl.zdbjq.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qza.gzhubu.top

================================================================================
来源：http://jbf.cdnleiting.top

J. 日期与时间
来源：http://dwe.shangyingyoupin.top

================================================================================
来源：http://xiy.pycfn.com

[J01] 获取当前时间
来源：http://zwf.zhaomingkeji.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://ixk.jianghu66.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jsz.ywan-chungtsiang.top

JS:   new Date();  Date.now()
来源：http://cux.pycfn.com

TS:   new Date();  Date.now()
来源：http://ipv.kuanghao11.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pdn.havefunace.top

Go:   time.Now()
来源：http://acf.epnwcf.com

Ruby: Time.now
来源：http://kpx.yj20258.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lcc.shanyushiyangtech.top

[J02] 格式化输出
来源：http://ikn.hammf.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qvg.daria6918.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pfo.yfazqb.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fxg.ehwqpu.com

TS:   d.toISOString()
来源：http://acb.pycfn.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jsw.kuanghao11.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yrm.c1oappe.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rgq.guowangkeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jku.chenjidiqi.icu

[J03] 字符串解析为日期
来源：http://iwm.dianchejie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mzg.0kj1m.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zuv.zdqjudy.top

JS:   new Date("2024-01-02")
来源：http://wtp.yj20258.top

TS:   new Date("2024-01-02")
来源：http://hxb.yj20258.top

Java: LocalDate.parse("2024-01-02")
来源：http://hnz.nwbrower.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mmc.chenjidiqi.icu

Ruby: Date.parse("2024-01-02")
来源：http://aja.ppjwa.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kdc.vqdsnc.cn

[J04] 时间戳与日期互转
来源：http://zpn.zycfv.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xvr.yangfankeji.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qkd.redwolf501.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kjs.quarkkingdee.top

TS:   Math.floor(Date.now() / 1000)
来源：http://brb.quarkkingdee.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mqw.zhongyouzk.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dfp.sweek.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://buw.xylfe.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ftw.uphjek.com

[J05] 时间加减（加 7 天）
来源：http://ffw.hesvh.cn

Py:   now + timedelta(days=7)
来源：http://vvn.meibo888.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://vvp.daria6918.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vzx.ehwqpu.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rlj.cqqwz.cn

Java: LocalDate.now().plusDays(7)
来源：http://xbr.shzxlz.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wyj.hysaishi.cn

Ruby: Time.now + 7 * 86400
来源：http://npc.jianghu66.top

C#:   DateTime.Now.AddDays(7)
来源：http://zaz.jyoumei.cn

[J06] 计算两时间之差
来源：http://uxc.vehdjk.com

Py:   (end - start).total_seconds()
来源：http://qcl.fzhhl.top

PHP:  $end->diff($start)->days;
来源：http://ocp.cheryme.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nbn.shanyushiyangtech.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qot.xziqi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lqo.andypj.xyz

Go:   end.Sub(start).Hours()
来源：http://duh.sxryk.cn

Ruby: end - start                 # 返回秒数
来源：http://olg.xuetiantiany.cn

C#:   (end - start).TotalSeconds
来源：http://oym.vehdjk.com

[J07] 比较两个日期
来源：http://zxe.yonumen.top

Py:   d1 < d2;  d1 == d2
来源：http://mfx.jqgfzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tqn.jinqigfzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://xvs.hysaishi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zti.xziqi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gmm.yfazqb.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ktd.dashuyun.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kkn.havefunace.top

C#:   d1 < d2;  d1 == d2
来源：http://kkk.sxryk.cn

[J08] 提取年月日与星期
来源：http://mtr.gzhubu.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fyy.ehwqpu.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://psa.zdqjudy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tnd.hesvh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pso.haohaochexian.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cur.kuanghao11.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zjc.yongpay.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hlf.jinqigfzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zzn.yangfankeji.com

[J09] 时区处理
来源：http://rmj.yuxming.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rne.shangyingyoupin.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tpt.jyoumei.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uyb.smart0.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tbz.zdqjudy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qhv.shanyushiyangtech.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ele.birdmap.top

Ruby: Time.now.getlocal("+08:00")
来源：http://yaw.zdqjudy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ujk.guannengcc.top

[J10] 取今天 / 本月第一天
来源：http://bms.cashguo.top

Py:   date.today();  date.today().replace(day=1)
来源：http://jmz.mhx1999.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://prg.jianghu66.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tvy.cqqwz.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fwc.tanke756.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rhw.zdqjudy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sry.chenzaomai.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://eet.feifeiyinyue.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://djg.gzhubu.top

================================================================================
来源：http://zyc.jinyuanbaomall.cn

K. JSON 与序列化
来源：http://fht.yonumen.top

================================================================================
来源：http://fjv.yj20258888.top

[K01] 对象转 JSON 字符串
来源：http://zam.gogol.net.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://szd.hongshengwenyu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lta.epnwcf.com

JS:   JSON.stringify(obj)
来源：http://own.hnxiangtu.top

TS:   JSON.stringify(obj)
来源：http://cgf.hysaishi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zoy.yangfankeji.com

Go:   json.Marshal(obj)
来源：http://mys.yvedp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cem.xziqi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://phg.birdmap.top

[K02] JSON 字符串转对象
来源：http://jbm.yvedp.cn

Py:   json.loads(s)
来源：http://ayc.bbcook.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kld.hcnkem.com

JS:   JSON.parse(s)
来源：http://afs.cdnleiting.top

TS:   JSON.parse(s)
来源：http://tke.cheryme.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nvy.jinghuilouyu.cn

Go:   json.Unmarshal(data, &v)
来源：http://jzl.meibo888.top

Ruby: JSON.parse(s)
来源：http://pdt.52xcode.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gir.0kj1m.cn

[K03] JSON 美化输出（带缩进）
来源：http://hvy.cashguo.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dji.zhaomingkeji.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://chl.hesvh.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kyw.9152youxi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vkx.svipenyu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kts.jinyuanbaomall.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://iij.daxiang520.top

Ruby: JSON.pretty_generate(obj)
来源：http://kdt.sweek.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://anc.andypj.xyz

[K04] 读取 JSON 文件
来源：http://rob.zdbjq.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://enz.bjfxy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bmq.ctjpmb.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vcf.fzhhl.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://shv.pengpengdd.cyou

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bsu.chenzaomai.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dlj.ctjpmb.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://vbv.nanxinkj.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pwq.xinyue.icu

[K05] 深拷贝对象
来源：http://qfw.jiagoushi.top

Py:   copy.deepcopy(obj)
来源：http://zml.gaohongyu789.top

PHP:  unserialize(serialize($obj));
来源：http://xeu.jinqigfzy.top

JS:   structuredClone(obj)
来源：http://flm.zdbjq.cn

TS:   structuredClone(obj)
来源：http://hfd.cucudq.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zqv.sweek.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vcm.pengpengdd.cyou

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ses.cucudq.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://atx.ehwqpu.com

[K06] 解析 URL 查询串
来源：http://qba.zdqjudy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ylt.zhoulong.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tfq.daria6918.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://got.chenzaomai.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pdu.52xcode.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uip.birdmap.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jbm.jqgufenzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ckh.c1oappe.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qry.sweek.top

[K07] 进制转换
来源：http://ydl.yfazqb.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hgr.yj20258888.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fyc.ywan-chungtsiang.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lxc.sysykeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://szr.mhx1999.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wjp.smart0.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cwo.fanxiaobao.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hoy.ehwqpu.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vtb.guowangkeji.top

[K08] 二进制序列化（非 JSON）
来源：http://ijc.hcnkem.com

Py:   pickle.dumps(obj)
来源：http://edv.tanke756.top

PHP:  serialize($obj);  unserialize($s);
来源：http://kcg.redwolf501.top

JS:   v8.serialize(obj)        // Node
来源：http://qfv.zhengqikj.top

TS:   v8.serialize(obj)        // Node
来源：http://rkz.ydzc1.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lqh.yonumen.top

Go:   encoding/gob
来源：http://igd.yuxming.cn

Ruby: Marshal.dump(obj)
来源：http://sjp.yj20258.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fkw.quarkkingdee.top

================================================================================
来源：http://sdy.fengsongda.top

L. 网络请求
来源：http://hlf.jinghuilouyu.cn

================================================================================
来源：http://qpq.zhijiandao.cn

[L01] 发送 GET 请求
来源：http://gzi.meibo888.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://esi.hfpthk.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://euc.ppjwa.cn

JS:   await fetch(url)
来源：http://cjt.gaohongyu789.top

TS:   await fetch(url)
来源：http://pwe.shanyushiyangtech.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bry.cashguo.top

Go:   resp, err := http.Get(url)
来源：http://ubr.svipenyu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tzp.jqgfzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ifk.yongpay.top

[L02] 发送 POST JSON
来源：http://wbv.bjfxy.top

Py:   requests.post(url, json={"a": 1})
来源：http://ceb.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://eyl.svipenyu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nfo.fzhhl.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hon.cdnleiting.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://olr.gogol.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ygi.nwbrower.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hdj.xinyue.icu

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jkg.yj20258888.top

[L03] 设置自定义请求头
来源：http://xhj.yvedp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qcr.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wgj.guowangkeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xob.epnwcf.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cfy.yfazqb.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zuh.gotoacloud.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jkw.jiagoushi.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mrh.hysaishi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zmx.yuxming.cn

[L04] 设置超时
来源：http://sec.fktsv.cn

Py:   requests.get(url, timeout=5)
来源：http://rit.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sfn.yueranfly.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://snu.birdmap.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jha.pengpengdd.cyou

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ugj.sjlbkw.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tot.daria6918.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://geo.ctjpmb.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://men.gotoacloud.top

[L05] 上传文件（multipart）
来源：http://rkd.sjlbkw.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hci.bbcook.cn


<!-- 参考信息 -->