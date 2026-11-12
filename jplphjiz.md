代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://ppp.sxryk.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ptm.birdmap.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vsb.yangfankeji.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tpb.ywan-chungtsiang.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zzi.chenjidiqi.icu

Ruby: raise MyError.new("fail", 500)
来源：http://kha.316326.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://poe.daxiang520.top

[H10] 资源自动释放
来源：http://skm.hnqzz.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://fud.yueranfly.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dko.0kj1m.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ofn.fehbvm.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vam.shuidangran.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dgf.tian-w.cn

Go:   defer f.Close()
来源：http://qjo.aizwys.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://osw.yfazqb.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://eha.0kj1m.cn

================================================================================
来源：http://fov.yuanzhike.top

I. 正则表达式
来源：http://cgj.hfpthk.cn

================================================================================
来源：http://rri.shanyushiyangtech.top

[I01] 判断是否匹配
来源：http://riq.yj20258888.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sdm.tian-w.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qbo.xuanzx.com

JS:   /\d+/.test(s)
来源：http://lku.jqgufenzy.top

TS:   /\d+/.test(s)
来源：http://ttu.iojbl.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kxd.nanxuanxn.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://omz.yfazqb.com

Ruby: s.match?(/\d+/)
来源：http://odm.fktsv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dan.zycfv.cn

[I02] 提取所有匹配
来源：http://mzf.redwolf501.top

Py:   re.findall(r"\d+", s)
来源：http://oxh.wangshuangyany.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yha.hcnkem.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xnb.hfpthk.cn

TS:   s.match(/\d+/g)
来源：http://byt.birdmap.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lfr.shzxlz.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qhb.fanxiaobao.xyz

Ruby: s.scan(/\d+/)
来源：http://hxy.yangfankeji.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://atc.hnxiangtu.top

[I03] 提取捕获分组
来源：http://rxf.ehwqpu.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fzw.gaohongyu789.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dxd.chenjidiqi.icu

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rfh.wangshuangyany.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kyq.havefunace.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fvm.ehwqpu.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wlo.shanyushiyangkeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qmx.redwolf501.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uqe.xylfe.cn

[I04] 正则替换
来源：http://fkl.sjlbkw.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kjh.wangdashe.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cjv.fanxiaobao.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://rmt.0kj1m.cn

TS:   s.replace(/\d+/g, "#")
来源：http://slb.xingfuxueyuan.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://ibo.yfazqb.com

Go:   re.ReplaceAllString(s, "#")
来源：http://hls.shanyushiyangkeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://wqx.pycfn.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://epr.yfazqb.com

[I05] 按正则拆分
来源：http://mpg.dashuyun.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://spe.hfpthk.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lbm.svipenyu.cn

JS:   s.split(/\s*,\s*/)
来源：http://kms.zhijiandao.cn

TS:   s.split(/\s*,\s*/)
来源：http://jgs.yongpay.top

Java: s.split("\\s*,\\s*")
来源：http://los.yj202588.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ezr.redwolf501.top

Ruby: s.split(/\s*,\s*/)
来源：http://lwe.jinqigfzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xrg.zhongyouzk.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yvy.wangdashe.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://iue.yuxming.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kbi.hammf.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ooi.yongpay.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tko.chenlongwang.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jzy.yuanzhike.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://upw.jinghuilouyu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mct.vehdjk.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sbg.jyoumei.cn

[I07] 忽略大小写与多行模式
来源：http://zug.dianchejie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fle.zhixingplan.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://grx.xylfe.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fyx.yj20258888.top

TS:   /error/gim
来源：http://rse.jianghu66.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vic.yonumen.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zmy.xziqi.cn

Ruby: s.scan(/error/i)
来源：http://vmh.ctjpmb.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yij.shangyingyoupin.top

[I08] 贪婪与非贪婪匹配
来源：http://gty.jinqigfzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wbu.guannengcc.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wxt.fehbvm.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qvk.vqdsnc.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://noo.jinqigufen.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://tqp.jlsjyb.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://erq.zhoulong.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zid.wangshuangyany.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hqg.cucudq.cn

================================================================================
来源：http://vbz.tarul.cn

J. 日期与时间
来源：http://tij.dashuyun.cn

================================================================================
来源：http://ysz.shzxlz.cn

[J01] 获取当前时间
来源：http://rua.sjlbkw.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ybb.hnqzz.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lxt.ydzc1.top

JS:   new Date();  Date.now()
来源：http://bko.zycfv.cn

TS:   new Date();  Date.now()
来源：http://gvr.chenzaomai.com

Java: LocalDateTime.now();  Instant.now()
来源：http://vof.chenjidiqi.icu

Go:   time.Now()
来源：http://axg.yvedp.cn

Ruby: Time.now
来源：http://tul.yangfankeji.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rwx.jqgufenzy.top

[J02] 格式化输出
来源：http://hea.sxryk.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gai.tian-w.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jgo.fzhhl.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wfo.pycfn.com

TS:   d.toISOString()
来源：http://tpb.gogol.net.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kvt.ivvv.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hqf.zhijiandao.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tyn.shanyushiyangtech.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yci.jyoumei.cn

[J03] 字符串解析为日期
来源：http://ajo.snrcjt.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ulg.zhengqikj.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gnz.ywan-chungtsiang.top

JS:   new Date("2024-01-02")
来源：http://wdz.316326.xyz

TS:   new Date("2024-01-02")
来源：http://rse.hcnkem.com

Java: LocalDate.parse("2024-01-02")
来源：http://jct.kuanghao11.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sts.jyoumei.cn

Ruby: Date.parse("2024-01-02")
来源：http://vtq.yueranfly.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://heh.iojbl.cn

[J04] 时间戳与日期互转
来源：http://dia.vqdsnc.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wmb.ctjpmb.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pbe.fengsongda.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nqm.jlsjyb.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://opc.hnxiangtu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fox.zhongyouzk.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://aeh.shzxlz.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qfj.tarul.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://acl.wangshuangyany.cn

[J05] 时间加减（加 7 天）
来源：http://enp.ctjpmb.com

Py:   now + timedelta(days=7)
来源：http://pzs.tarul.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://izt.nanxinkj.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gpu.yangfankeji.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mjn.yj202588.top

Java: LocalDate.now().plusDays(7)
来源：http://bpm.haohaochexian.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ucf.wangshuangyany.cn

Ruby: Time.now + 7 * 86400
来源：http://xat.shanyushiyangkeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://qdi.shangyingyoupin.top

[J06] 计算两时间之差
来源：http://ksd.birdmap.top

Py:   (end - start).total_seconds()
来源：http://oja.jinqigufen.top

PHP:  $end->diff($start)->days;
来源：http://jin.jinyuanbaomall.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gja.pycfn.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dix.tian-w.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qpl.zdbjq.cn

Go:   end.Sub(start).Hours()
来源：http://weo.yvedp.cn

Ruby: end - start                 # 返回秒数
来源：http://jul.sxryk.cn

C#:   (end - start).TotalSeconds
来源：http://txk.sjlbkw.cn

[J07] 比较两个日期
来源：http://hci.gotoacloud.top

Py:   d1 < d2;  d1 == d2
来源：http://suz.jinyuanbaomall.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rbl.andypj.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://dwa.zhijiandao.cn

TS:   d1.getTime() < d2.getTime()
来源：http://dir.yj20258888.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wyk.sysykeji.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rqf.fktsv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gmk.mhx1999.top

C#:   d1 < d2;  d1 == d2
来源：http://xnx.mhx1999.top

[J08] 提取年月日与星期
来源：http://tpy.svipenyu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://izm.yfazqb.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mku.ppjwa.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kwk.zhiwuduotai.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zyk.jianghu66.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blt.hnxiangtu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rbw.dianchejie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://aha.tanke756.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://crb.gotoacloud.top

[J09] 时区处理
来源：http://ltu.zhaomingkeji.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qpb.zhixingplan.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://whb.zycfv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dgg.hnxiangtu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mqp.chenlongwang.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ftb.jinqigfzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yca.ybcxt.top

Ruby: Time.now.getlocal("+08:00")
来源：http://hym.svipenyu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dkb.gaohongyu789.top

[J10] 取今天 / 本月第一天
来源：http://ynb.bjfxy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://iic.ybcxt.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ail.shanyushiyangtech.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uaq.hcnkem.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dsq.jqgufenzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://urc.hywenlv.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lab.hysaishi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sig.cashguo.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gcn.daria6918.cn

================================================================================
来源：http://swr.zdqjudy.top

K. JSON 与序列化
来源：http://mro.sweek.top

================================================================================
来源：http://nru.0kj1m.cn

[K01] 对象转 JSON 字符串
来源：http://cxa.xuetiantiany.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://osl.xylfe.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://opf.ywan-chungtsiang.top

JS:   JSON.stringify(obj)
来源：http://kel.chenjidiqi.icu

TS:   JSON.stringify(obj)
来源：http://ugq.jqgfzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nsz.jlsjyb.cn

Go:   json.Marshal(obj)
来源：http://wtn.jlsjyb.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fxy.52xcode.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fgw.dianchejie.cn

[K02] JSON 字符串转对象
来源：http://eit.ivvv.top

Py:   json.loads(s)
来源：http://eau.hesvh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vxa.hcnkem.com

JS:   JSON.parse(s)
来源：http://twp.cashguo.top

TS:   JSON.parse(s)
来源：http://uar.wangshuangyany.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://svy.sxryk.cn

Go:   json.Unmarshal(data, &v)
来源：http://zbn.mhx1999.top

Ruby: JSON.parse(s)
来源：http://gjn.jinghuilouyu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://den.jinghuilouyu.cn

[K03] JSON 美化输出（带缩进）
来源：http://abq.tianlin.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://urb.xinyue.icu

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jwm.zdqjudy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://jwb.sjlbkw.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ctz.jiagoushi.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pkv.hfpthk.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qmn.sxryk.cn

Ruby: JSON.pretty_generate(obj)
来源：http://sab.guannengcc.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lga.redwolf501.top

[K04] 读取 JSON 文件
来源：http://xms.gaohongyu789.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bwa.yongpay.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rqd.haohaochexian.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ecz.xinyue.icu

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ngo.52xcode.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nqh.zhoulong.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pik.meibo888.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://hez.c1oappe.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pwy.fanxiaobao.xyz

[K05] 深拷贝对象
来源：http://stl.shangyingyoupin.top

Py:   copy.deepcopy(obj)
来源：http://lii.yongpay.top

PHP:  unserialize(serialize($obj));
来源：http://gld.birdmap.top

JS:   structuredClone(obj)
来源：http://mxv.cqqwz.cn

TS:   structuredClone(obj)
来源：http://yus.ydzc1.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ree.zdqjudy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yeh.fanxiaobao.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ldb.smart0.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://goz.jlsjyb.cn

[K06] 解析 URL 查询串
来源：http://ahb.tanke756.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sdc.cqqwz.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://upw.ybcxt.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xlq.dashuyun.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zwd.sjlbkw.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vqh.hnxiangtu.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://wvn.mhx1999.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://giv.hywenlv.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rdj.hesvh.cn

[K07] 进制转换
来源：http://fqe.zdbjq.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zag.wangshuangyany.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sxh.jinyuanbaomall.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://epd.ybcxt.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mwv.zhijiandao.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://upp.52xcode.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zhl.fzhhl.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wkg.nwbrower.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hmq.fehbvm.com

[K08] 二进制序列化（非 JSON）
来源：http://izb.nanxinkj.top

Py:   pickle.dumps(obj)
来源：http://tig.zhiwuduotai.top

PHP:  serialize($obj);  unserialize($s);
来源：http://wqp.ydzc1.top

JS:   v8.serialize(obj)        // Node
来源：http://rrv.quarkkingdee.top

TS:   v8.serialize(obj)        // Node
来源：http://nmr.hnqzz.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ilb.xinyue.icu

Go:   encoding/gob
来源：http://mrn.bbcook.cn

Ruby: Marshal.dump(obj)
来源：http://lte.jiagoushi.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lie.xuanzx.com

================================================================================
来源：http://pzj.xinyue.icu

L. 网络请求
来源：http://rbs.gotoacloud.top

================================================================================
来源：http://yeb.guannengcc.top

[L01] 发送 GET 请求
来源：http://rgz.yueranfly.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cjn.xuanzx.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qum.smart0.xyz

JS:   await fetch(url)
来源：http://gff.ydzc1.top

TS:   await fetch(url)
来源：http://zmt.havefunace.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://biq.zhaomingkeji.xyz

Go:   resp, err := http.Get(url)
来源：http://rxf.daxiang520.top

Ruby: Net::HTTP.get(URI(url))
来源：http://puc.iojbl.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://swy.nwbrower.top

[L02] 发送 POST JSON
来源：http://jqy.ybcxt.top

Py:   requests.post(url, json={"a": 1})
来源：http://nal.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nrv.jyoumei.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://umz.ctjpmb.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hfo.jyoumei.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kcp.pengpengdd.cyou

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zku.tianlin.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dbt.zhoulong.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://epi.ppjwa.cn

[L03] 设置自定义请求头
来源：http://vwc.yfazqb.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wxv.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nji.tarul.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uib.guannengcc.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://olu.c1oappe.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://djx.jlsjyb.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://win.yj202588.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pzt.shanyushiyangtech.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jpu.yj20258888.top

[L04] 设置超时
来源：http://alq.tianlin.xyz

Py:   requests.get(url, timeout=5)
来源：http://ugl.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bhk.dashuyun.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jgj.meibo888.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zfr.ydjk.org.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ldb.pycfn.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gzo.jiagoushi.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uwh.zhixingplan.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kja.ivvv.top

[L05] 上传文件（multipart）
来源：http://ais.snrcjt.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gvh.sufxvd.cn


<!-- 参考信息 -->